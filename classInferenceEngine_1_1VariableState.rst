.. index:: pair: class; InferenceEngine::VariableState
.. _doxid-class_inference_engine_1_1_variable_state:

class InferenceEngine::VariableState
====================================



Overview
~~~~~~~~

:ref:`VariableState <doxid-class_inference_engine_1_1_variable_state>` class. :ref:`More...<details-class_inference_engine_1_1_variable_state>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_memory_state.hpp>
	
	class VariableState
	{
	public:
		// construction
	
		:ref:`VariableState<doxid-class_inference_engine_1_1_variable_state_1ad91a85a096393a8fbe5e05c2f410ffbd>`();
		:ref:`VariableState<doxid-class_inference_engine_1_1_variable_state_1aa73864db3e7123104716528a13f2c47f>`(const VariableState& other);
		:ref:`VariableState<doxid-class_inference_engine_1_1_variable_state_1a19265e1cd0770ae386fc9adfbcbf6362>`(VariableState&& other);

		// methods
	
		VariableState& :ref:`operator =<doxid-class_inference_engine_1_1_variable_state_1a01d54988b577917ef7c863c855bb6b63>` (const VariableState& other);
		VariableState& :ref:`operator =<doxid-class_inference_engine_1_1_variable_state_1a4b386be01c6f08051b62b3332caa5da7>` (VariableState&& other);
		void :ref:`Reset<doxid-class_inference_engine_1_1_variable_state_1ac7975e5e8d33bc0265ff100644a56f5f>`();
		std::string :ref:`GetName<doxid-class_inference_engine_1_1_variable_state_1a9f1f83899996d34ca65cb868b9a9fc3a>`() const;
		:ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>` :ref:`GetState<doxid-class_inference_engine_1_1_variable_state_1a16d0f4821e03aa6e34dc02e8f6fb36b4>`() const;
		void :ref:`SetState<doxid-class_inference_engine_1_1_variable_state_1ac1cfa3c905150773bbbdf1f6d5660c1a>`(:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` state);
	};
.. _details-class_inference_engine_1_1_variable_state:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`VariableState <doxid-class_inference_engine_1_1_variable_state>` class.

Construction
------------

.. _doxid-class_inference_engine_1_1_variable_state_1ad91a85a096393a8fbe5e05c2f410ffbd:
.. index:: pair: function; VariableState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableState()

Default constructor.

.. _doxid-class_inference_engine_1_1_variable_state_1aa73864db3e7123104716528a13f2c47f:
.. index:: pair: function; VariableState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableState(const VariableState& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`VariableState <doxid-class_inference_engine_1_1_variable_state>` object

.. _doxid-class_inference_engine_1_1_variable_state_1a19265e1cd0770ae386fc9adfbcbf6362:
.. index:: pair: function; VariableState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableState(VariableState&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`VariableState <doxid-class_inference_engine_1_1_variable_state>` object

Methods
-------

.. _doxid-class_inference_engine_1_1_variable_state_1a01d54988b577917ef7c863c855bb6b63:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableState& operator = (const VariableState& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`VariableState <doxid-class_inference_engine_1_1_variable_state>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-class_inference_engine_1_1_variable_state_1a4b386be01c6f08051b62b3332caa5da7:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableState& operator = (VariableState&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`VariableState <doxid-class_inference_engine_1_1_variable_state>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-class_inference_engine_1_1_variable_state_1ac7975e5e8d33bc0265ff100644a56f5f:
.. index:: pair: function; Reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void Reset()

Reset internal variable state for relevant infer request, to a value specified as default for according ReadValue node.

.. _doxid-class_inference_engine_1_1_variable_state_1a9f1f83899996d34ca65cb868b9a9fc3a:
.. index:: pair: function; GetName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string GetName() const

Gets name of current variable state, if length of array is not enough name is truncated by len, null terminator is inserted as well. As variable state name ``variable_id`` from according ``ReadValue`` used.



.. rubric:: Returns:

A string representing a state name

.. _doxid-class_inference_engine_1_1_variable_state_1a16d0f4821e03aa6e34dc02e8f6fb36b4:
.. index:: pair: function; GetState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>` GetState() const

Returns the value of the variable state.



.. rubric:: Returns:

A blob representing a state

.. _doxid-class_inference_engine_1_1_variable_state_1ac1cfa3c905150773bbbdf1f6d5660c1a:
.. index:: pair: function; SetState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetState(:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` state)

Sets the new state for the next inference.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- state

		- The current state to set


