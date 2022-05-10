.. index:: pair: class; ov::pass::PassBase
.. _doxid-classov_1_1pass_1_1_pass_base:

class ov::pass::PassBase
========================



Overview
~~~~~~~~

Base class for transformation passes. :ref:`More...<details-classov_1_1pass_1_1_pass_base>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <pass.hpp>
	
	class PassBase
	{
	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :target:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`;

		// methods
	
		bool :ref:`get_property<doxid-classov_1_1pass_1_1_pass_base_1a3107964f6c4d4bf1d3fbc2bf97ccc0b8>`(const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& prop_mask) const;
		void :target:`set_name<doxid-classov_1_1pass_1_1_pass_base_1a78ddde2a8770041d2f23ce59af908f5d>`(const std::string& name);
		std::string :target:`get_name<doxid-classov_1_1pass_1_1_pass_base_1a6cd527d2176f1350dd999dc4632a576b>`() const;
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_base_1a6a56827a1cf76be99289bab703982869>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_pass_base_1abe74bba4b563ad367f2fdc7836016391>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);
		std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> :ref:`get_pass_config<doxid-classov_1_1pass_1_1_pass_base_1a4902f6ed9322e0fd38810d701f4409df>`();
		bool :ref:`m_transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1a568e5b1f0e01f221d36dffabbf156b3d>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		bool :ref:`transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		virtual const :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`& :target:`get_type_info<doxid-classov_1_1pass_1_1_pass_base_1ab7020db2fcebc9b6e0741a451778fb0c>`() const = 0;
	};

	// direct descendants

	class :ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`;
	class :ref:`ModelPass<doxid-classov_1_1pass_1_1_model_pass>`;
.. _details-classov_1_1pass_1_1_pass_base:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Base class for transformation passes.

Methods
-------

.. _doxid-classov_1_1pass_1_1_pass_base_1a3107964f6c4d4bf1d3fbc2bf97ccc0b8:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_property(const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& prop_mask) const

Check if this pass has all the pass properties.

.. _doxid-classov_1_1pass_1_1_pass_base_1a6a56827a1cf76be99289bab703982869:
.. index:: pair: function; set_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_callback(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback)

Set callback for particular transformation type. This method set global callback. For more details see :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` class documentation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- callback

		- lambda function that takes node and returns bool

.. _doxid-classov_1_1pass_1_1_pass_base_1abe74bba4b563ad367f2fdc7836016391:
.. index:: pair: function; set_pass_config

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_pass_config(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config)

Set :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` for particular transformation instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pass_config

		- is a :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` shared_ptr

.. _doxid-classov_1_1pass_1_1_pass_base_1a4902f6ed9322e0fd38810d701f4409df:
.. index:: pair: function; get_pass_config

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> get_pass_config()

Allows to access :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` shared instance.



.. rubric:: Returns:

Shared instance of :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` class

.. _doxid-classov_1_1pass_1_1_pass_base_1a568e5b1f0e01f221d36dffabbf156b3d:
.. index:: pair: function; m_transformation_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool m_transformation_callback(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node)

Applies callback for given node. By default callback returns false. This method remains here only for backward compatibility and will be removed after all transformations are moved to :ref:`transformation_callback() <doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab>` method.



.. rubric:: Returns:

result of callback execution for given node

.. _doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab:
.. index:: pair: function; transformation_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool transformation_callback(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node)

Applies callback for given node. By default callback returns false.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- which will be used inside callback



.. rubric:: Returns:

result of callback execution for given node


