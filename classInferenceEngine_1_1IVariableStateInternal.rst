.. index:: pair: interface; InferenceEngine::IVariableStateInternal
.. _doxid-class_inference_engine_1_1_i_variable_state_internal:

interface InferenceEngine::IVariableStateInternal
=================================================



Overview
~~~~~~~~

Minimal interface for variable state implementation. :ref:`More...<details-class_inference_engine_1_1_i_variable_state_internal>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_ivariable_state_internal.hpp>
	
	template IVariableStateInternal: public std::enable_shared_from_this< IVariableStateInternal >
	{
		// typedefs
	
		typedef std::shared_ptr<IVariableStateInternal> :ref:`Ptr<doxid-class_inference_engine_1_1_i_variable_state_internal_1a9a3d9ff1e78f317d3a24df6775d6aa79>`;

		// construction
	
		:target:`IVariableStateInternal<doxid-class_inference_engine_1_1_i_variable_state_internal_1a30aaf3e662d440b686cd85ee05f5e3ac>`(const std::string& name);

		// methods
	
		virtual std::string :ref:`GetName<doxid-class_inference_engine_1_1_i_variable_state_internal_1a83c6412acb733db83a1388f2c0a486e1>`() const;
		virtual void :ref:`Reset<doxid-class_inference_engine_1_1_i_variable_state_internal_1a2d270872005af11e32feef4b977742b0>`();
		virtual void :ref:`SetState<doxid-class_inference_engine_1_1_i_variable_state_internal_1ac2ac35061fd017e2790d5c5f8073aa6d>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& newState);
		virtual :ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>` :ref:`GetState<doxid-class_inference_engine_1_1_i_variable_state_internal_1aa2e23d399dc894181b5621941076a1cc>`() const;

	protected:
	};
.. _details-class_inference_engine_1_1_i_variable_state_internal:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimal interface for variable state implementation.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_variable_state_internal_1a9a3d9ff1e78f317d3a24df6775d6aa79:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IVariableStateInternal> Ptr

A shared pointer to a :ref:`IVariableStateInternal <doxid-class_inference_engine_1_1_i_variable_state_internal>` interface.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_variable_state_internal_1a83c6412acb733db83a1388f2c0a486e1:
.. index:: pair: function; GetName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string GetName() const

Gets a variable state name.



.. rubric:: Returns:

A string representing variable state name

.. _doxid-class_inference_engine_1_1_i_variable_state_internal_1a2d270872005af11e32feef4b977742b0:
.. index:: pair: function; Reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Reset()

Reset internal variable state for relevant infer request, to a value specified as default for according ``ReadValue`` node.

.. _doxid-class_inference_engine_1_1_i_variable_state_internal_1ac2ac35061fd017e2790d5c5f8073aa6d:
.. index:: pair: function; SetState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetState(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& newState)

Sets the new state for the next inference.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- newState

		- A new state

.. _doxid-class_inference_engine_1_1_i_variable_state_internal_1aa2e23d399dc894181b5621941076a1cc:
.. index:: pair: function; GetState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>` GetState() const

Returns the value of the variable state.



.. rubric:: Returns:

The value of the variable state


