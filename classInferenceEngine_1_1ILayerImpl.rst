.. index:: pair: interface; InferenceEngine::ILayerImpl
.. _doxid-class_inference_engine_1_1_i_layer_impl:

interface InferenceEngine::ILayerImpl
=====================================



Overview
~~~~~~~~

This class provides interface for extension implementations. :ref:`More...<details-class_inference_engine_1_1_i_layer_impl>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iextension.h>
	
	template ILayerImpl
	{
		// typedefs
	
		typedef std::shared_ptr<ILayerImpl> :ref:`Ptr<doxid-class_inference_engine_1_1_i_layer_impl_1a83cfc1d50968aa3dbdd05fac0a55c28d>`;
	};

	// direct descendants

	template :ref:`ILayerExecImpl<doxid-class_inference_engine_1_1_i_layer_exec_impl>`;
.. _details-class_inference_engine_1_1_i_layer_impl:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class provides interface for extension implementations.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_layer_impl_1a83cfc1d50968aa3dbdd05fac0a55c28d:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ILayerImpl> Ptr

A shared pointer to the :ref:`ILayerImpl <doxid-class_inference_engine_1_1_i_layer_impl>` interface.


