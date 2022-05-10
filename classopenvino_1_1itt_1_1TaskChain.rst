.. index:: pair: class; openvino::itt::TaskChain
.. _doxid-classopenvino_1_1itt_1_1_task_chain:

class openvino::itt::TaskChain
==============================



Overview
~~~~~~~~

Used to annotate a sequence of sections of code which would be named at runtime. :ref:`More...<details-classopenvino_1_1itt_1_1_task_chain>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <itt.hpp>
	
	template <domain_t(\*)() domain>
	class TaskChain
	{
	public:
		// construction
	
		:ref:`TaskChain<doxid-classopenvino_1_1itt_1_1_task_chain_1a8d63c2fa04dcd96a41a295fe8a466abb>`(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` taskHandle, std::string&& prefix);

		// methods
	
		void :ref:`next<doxid-classopenvino_1_1itt_1_1_task_chain_1aec36425d44c51a574c4dd355907c8785>`(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` taskHandle);
		std::string :target:`taskName<doxid-classopenvino_1_1itt_1_1_task_chain_1ae63160dc4221f3a2d8f48ca66f11a720>`() const;
		std::string :target:`taskNameOrHandle<doxid-classopenvino_1_1itt_1_1_task_chain_1a93aa7b881ebbe801d58ab71893c0c668>`(const std::string& name) const;
		:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` :target:`taskNameOrHandle<doxid-classopenvino_1_1itt_1_1_task_chain_1a883607b0ff149e19c8dbe412822adfab>`(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` handle) const;
		void :target:`skip<doxid-classopenvino_1_1itt_1_1_task_chain_1a3e08565c58a699bfff85c64b21b4f4d1>`();
	};
.. _details-classopenvino_1_1itt_1_1_task_chain:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Used to annotate a sequence of sections of code which would be named at runtime.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- The

		- ``domain`` parameter is domain type which shoud be defined with :ref:`OV_ITT_DOMAIN() <doxid-group__ie__dev__profiling_1ga83ad6f539c8e1aef944160e37fcfcb4d>` macro.

Construction
------------

.. _doxid-classopenvino_1_1itt_1_1_task_chain_1a8d63c2fa04dcd96a41a295fe8a466abb:
.. index:: pair: function; TaskChain

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TaskChain(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` taskHandle, std::string&& prefix)

Construct :ref:`TaskChain <doxid-classopenvino_1_1itt_1_1_task_chain>` with defined annotation handle.

Methods
-------

.. _doxid-classopenvino_1_1itt_1_1_task_chain_1aec36425d44c51a574c4dd355907c8785:
.. index:: pair: function; next

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void next(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` taskHandle)

Ends the previous task from the chain and starts a new one with the given annotation handle.


