.. index:: pair: class; ov::pass::Manager
.. _doxid-classov_1_1pass_1_1_manager:

class ov::pass::Manager
=======================



Overview
~~~~~~~~

:ref:`Manager <doxid-classov_1_1pass_1_1_manager>` class allows to manage transformation passes. :ref:`More...<details-classov_1_1pass_1_1_manager>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <manager.hpp>
	
	class Manager
	{
	public:
		// construction
	
		:target:`Manager<doxid-classov_1_1pass_1_1_manager_1a3aa21b0a13075c34d6dc554cc091055f>`();
		:target:`Manager<doxid-classov_1_1pass_1_1_manager_1a341653d14cacd4acd6b8aeb9c324fbc7>`(std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> pass_config);

		// methods
	
		template <typename T, bool Enable = true, class... Args>
		std::shared_ptr<T> :ref:`register_pass<doxid-classov_1_1pass_1_1_manager_1affc722b2463a786b66398472141d45f2>`(Args&&... args);
	
		std::shared_ptr<:ref:`PassBase<doxid-classov_1_1pass_1_1_pass_base>`> :target:`register_pass_instance<doxid-classov_1_1pass_1_1_manager_1a03e96522f8b8ee8ebc68e364d4bafc4d>`(std::shared_ptr<:ref:`PassBase<doxid-classov_1_1pass_1_1_pass_base>`> pass);
		void :target:`run_passes<doxid-classov_1_1pass_1_1_manager_1a8b155191130f2c15e294cfd259d4ca0d>`(std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>);
		void :target:`set_pass_visualization<doxid-classov_1_1pass_1_1_manager_1a333c30e226f23d51f7c726be90a8ebff>`(bool new_state);
		void :ref:`set_per_pass_validation<doxid-classov_1_1pass_1_1_manager_1a4efe949a17dd14d02888540b2586d411>`(bool new_state);
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_manager_1af258d01df16d855da7854bf73773726e>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
		std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> :ref:`get_pass_config<doxid-classov_1_1pass_1_1_manager_1a79d596fda6b8726043751c4de7b30885>`();
	};
.. _details-classov_1_1pass_1_1_manager:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Manager <doxid-classov_1_1pass_1_1_manager>` class allows to manage transformation passes.

Methods
-------

.. _doxid-classov_1_1pass_1_1_manager_1affc722b2463a786b66398472141d45f2:
.. index:: pair: function; register_pass

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, bool Enable = true, class... Args>
	std::shared_ptr<T> register_pass(Args&&... args)

Register given transformation class type to execution list Example below show the basic usage of :ref:`pass::Manager <doxid-classov_1_1pass_1_1_manager>`.

.. code-block:: cpp

	pass::Manager manager;
	manager.register_pass<MyTransformation>(/\*transformation constructor ars\*&zwj;/);
	manager.run_passes(f);

For some purposes transformation can be registered and disabled by default.

.. code-block:: cpp

	manager.register_pass<MyTransformation, false>();



.. rubric:: Returns:

shared_ptr to the transformation instance

.. _doxid-classov_1_1pass_1_1_manager_1a4efe949a17dd14d02888540b2586d411:
.. index:: pair: function; set_per_pass_validation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_per_pass_validation(bool new_state)

Set flag to enable/disable running :ref:`Validate <doxid-classov_1_1pass_1_1_validate>` pass after executing each registered pass.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- new_state

		- Value "true" enables :ref:`Validate <doxid-classov_1_1pass_1_1_validate>` pass run; "false", otherwise

.. _doxid-classov_1_1pass_1_1_manager_1af258d01df16d855da7854bf73773726e:
.. index:: pair: function; set_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_callback(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback)

Callback is a lambda function that can be used by registered transformations. The main purpose of this callback is to provide a way for plugins to disable/enable transformations based on some conditions. In some cases plugins may want not to execute some transformations. For example plugin can disable unpleasant decompositions because of performance reasons for some cases. Callback example: auto callback = [](const std::shared_ptr<const ov::Node> & node) -> bool { return std::dynamic_pointer_cast<const ov::opset3::DepthToSpace>(node) != nullptr; }; This callback returns true in case of DepthToSpace operation. So when execution DepthToSpace decomposition pass will check is this decomposition needed or plugin can execute this operation directly. And of course on transformation side we need to have a response for this callback. if (transformation_callback(batch_to_space)) { return false; }.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- callback

		- lamda function that returns true in case if node is supported by plugin and transformation is not needed

.. _doxid-classov_1_1pass_1_1_manager_1a79d596fda6b8726043751c4de7b30885:
.. index:: pair: function; get_pass_config

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> get_pass_config()



.. rubric:: Returns:

:ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` shared object. This object is used for transformations pipeline configuration. This object allows to disable/enable transformations execution, set callback to particular transformation. For mo details see :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` class.


