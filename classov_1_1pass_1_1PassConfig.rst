.. index:: pair: class; ov::pass::PassConfig
.. _doxid-classov_1_1pass_1_1_pass_config:

class ov::pass::PassConfig
==========================



Overview
~~~~~~~~

Class representing a transformations config that is used for disabling/enabling transformations registered inside :ref:`pass::Manager <doxid-classov_1_1pass_1_1_manager>` and also allows to set callback for all transformations or for particular transformation. :ref:`More...<details-classov_1_1pass_1_1_pass_config>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <pass_config.hpp>
	
	class PassConfig
	{
	public:
		// methods
	
		void :ref:`disable<doxid-classov_1_1pass_1_1_pass_config_1a7c12a2223af7725477eb08fc17fb8b0d>`(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info);
	
		template <
			class T,
			typename std::enable_if<!ngraph::HasTypeInfoMember<T>::value, bool>::type = true
			>
		void :ref:`disable<doxid-classov_1_1pass_1_1_pass_config_1a21d4e6aa1832339360a654b8ed690481>`();
	
		void :ref:`enable<doxid-classov_1_1pass_1_1_pass_config_1ac95c582a2e8417abf241d03d86f697db>`(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info);
	
		template <
			class T,
			typename std::enable_if<!ngraph::HasTypeInfoMember<T>::value, bool>::type = true
			>
		void :ref:`enable<doxid-classov_1_1pass_1_1_pass_config_1a0f0f9a4570ec1222ce7ef41422c499c5>`();
	
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_config_1a8905ae9f43e0b09d3f370f0bee9a3ccb>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
	
		template <typename... Args>
		std::enable_if<sizeof...(Args)==0>::type :target:`set_callback<doxid-classov_1_1pass_1_1_pass_config_1a81ac0f0ee4ddbdc7907cc92410105ef0>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
	
		template <
			typename T,
			class... Args,
			typename std::enable_if<!ngraph::HasTypeInfoMember<T>::value, bool>::type = true
			>
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_config_1a297f189f84de82b1e0c2448ab697f4df>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
	
		:ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>` :ref:`get_callback<doxid-classov_1_1pass_1_1_pass_config_1af32c584827740dad7b96ea3d3872cb0a>`(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info) const;
	
		template <
			class T,
			typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
			>
		:ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>` :ref:`get_callback<doxid-classov_1_1pass_1_1_pass_config_1a3e2527f427c34903afedf35c0e81cce9>`() const;
	
		bool :ref:`is_disabled<doxid-classov_1_1pass_1_1_pass_config_1a31818182bac8be9d5d323cbb884b0684>`(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info) const;
	
		template <
			class T,
			typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
			>
		bool :ref:`is_disabled<doxid-classov_1_1pass_1_1_pass_config_1a9cb080488263648fe066c9cbed488f84>`() const;
	
		bool :ref:`is_enabled<doxid-classov_1_1pass_1_1_pass_config_1aa416e5d2b20aa3afe104c74ec39d8521>`(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info) const;
	
		template <
			class T,
			typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
			>
		bool :ref:`is_enabled<doxid-classov_1_1pass_1_1_pass_config_1a1780d39192f1e5d5b08c3b8f98ddd292>`() const;
	
		void :target:`add_disabled_passes<doxid-classov_1_1pass_1_1_pass_config_1a5ac8d28c1553feba480cafc360dd2ae4>`(const PassConfig& rhs);
	};
.. _details-classov_1_1pass_1_1_pass_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class representing a transformations config that is used for disabling/enabling transformations registered inside :ref:`pass::Manager <doxid-classov_1_1pass_1_1_manager>` and also allows to set callback for all transformations or for particular transformation.

When :ref:`pass::Manager <doxid-classov_1_1pass_1_1_manager>` is created all passes registered inside this manager including nested passes will share the same instance of :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` class. To work with this class first you need to get shared instance of this class by calling manager.get_pass_config() method. Then you will be able to disable/enable passes based on transformations type_info. For example:

.. code-block:: cpp

	pass::Manager manager;
	manager.register_pass<CommonOptimizations>();
	auto pass_config = manager.get_pass_config();
	pass_config->disable<ConvertGELU>(); // this will disable nested pass inside
	                                     // CommonOptimizations pipeline
	manager.run_passes(f);

Sometimes it is needed to call transformation inside other transformation manually. And for that case before running transformation you need manually check that this pass is not disabled and then you need to set current :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` instance to this transformation. For example:

.. code-block:: cpp

	// Inside MatcherPass callback or inside FunctionPass run_on_function() method
	// you need to call get_pass_config() method to get shared instance of PassConfig
	auto pass_config = get_pass_config();
	
	// Before running nested transformation you need to check is it disabled or not
	if (!pass_config->is_disabled<ConvertGELU>()) {
	    auto pass = ConvertGELU();
	    pass->set_pass_config(pass_config);
	    pass.apply(node);
	}

Following this logic inside your transformations you will guaranty that transformations will be executed in a right way.

Methods
-------

.. _doxid-classov_1_1pass_1_1_pass_config_1a7c12a2223af7725477eb08fc17fb8b0d:
.. index:: pair: function; disable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void disable(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info)

Disable transformation by its type_info.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type_info

		- Transformation type_info

.. _doxid-classov_1_1pass_1_1_pass_config_1a21d4e6aa1832339360a654b8ed690481:
.. index:: pair: function; disable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<!ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	void disable()

Disable transformation by its class type (based on type_info)

.. _doxid-classov_1_1pass_1_1_pass_config_1ac95c582a2e8417abf241d03d86f697db:
.. index:: pair: function; enable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void enable(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info)

Enable transformation by its type_info.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type_info

		- Transformation type_info

.. _doxid-classov_1_1pass_1_1_pass_config_1a0f0f9a4570ec1222ce7ef41422c499c5:
.. index:: pair: function; enable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<!ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	void enable()

Enable transformation by its class type (based on type_info)

.. _doxid-classov_1_1pass_1_1_pass_config_1a8905ae9f43e0b09d3f370f0bee9a3ccb:
.. index:: pair: function; set_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_callback(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback)

Set callback for all kind of transformations.

.. _doxid-classov_1_1pass_1_1_pass_config_1a297f189f84de82b1e0c2448ab697f4df:
.. index:: pair: function; set_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		class... Args,
		typename std::enable_if<!ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	void set_callback(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback)

Set callback for particular transformation class types.

Example below show how to set callback for one or multiple passes using this method.

.. code-block:: cpp

	pass_config->set_callback<ov::pass::ConvertBatchToSpace,
	                          ov::pass::ConvertSpaceToBatch>(
	         [](const_node_ptr &node) -> bool {
	              // Disable transformations for cases when input shape rank is not
	              equal to 4
	              const auto input_shape_rank =
	              node->get_output_partial_shape(0).rank().get_length();
	              if (input_shape_rank != 4) {
	                  return false;
	              }
	              return true;
	          });

Note that inside transformations you must provide code that work with this callback. See example below:

.. code-block:: cpp

	if (transformation_callback(node)) {
	    return false; // exit from transformation
	}

.. _doxid-classov_1_1pass_1_1_pass_config_1af32c584827740dad7b96ea3d3872cb0a:
.. index:: pair: function; get_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>` get_callback(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info) const

Get callback for given transformation type_info.

In case if callback wasn't set for given transformation type then global callback will be returned. But if even global callback wasn't set then default callback will be returned.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type_info

		- Transformation type_info

.. _doxid-classov_1_1pass_1_1_pass_config_1a3e2527f427c34903afedf35c0e81cce9:
.. index:: pair: function; get_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	:ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>` get_callback() const

Get callback for given transformation class type.



.. rubric:: Returns:

callback lambda function

.. _doxid-classov_1_1pass_1_1_pass_config_1a31818182bac8be9d5d323cbb884b0684:
.. index:: pair: function; is_disabled

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_disabled(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info) const

Check either transformation type is disabled or not.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type_info

		- Transformation type_info



.. rubric:: Returns:

true if transformation type was disabled and false otherwise

.. _doxid-classov_1_1pass_1_1_pass_config_1a9cb080488263648fe066c9cbed488f84:
.. index:: pair: function; is_disabled

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	bool is_disabled() const

Check either transformation class type is disabled or not.



.. rubric:: Returns:

true if transformation type was disabled and false otherwise

.. _doxid-classov_1_1pass_1_1_pass_config_1aa416e5d2b20aa3afe104c74ec39d8521:
.. index:: pair: function; is_enabled

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_enabled(const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& type_info) const

Check either transformation type is force enabled or not.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type_info

		- Transformation type_info



.. rubric:: Returns:

true if transformation type was force enabled and false otherwise

.. _doxid-classov_1_1pass_1_1_pass_config_1a1780d39192f1e5d5b08c3b8f98ddd292:
.. index:: pair: function; is_enabled

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	bool is_enabled() const

Check either transformation class type is force enabled or not.



.. rubric:: Returns:

true if transformation type was force enabled and false otherwise


