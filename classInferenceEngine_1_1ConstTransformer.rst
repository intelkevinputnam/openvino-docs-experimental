.. index:: pair: class; InferenceEngine::ConstTransformer
.. _doxid-class_inference_engine_1_1_const_transformer:

class InferenceEngine::ConstTransformer
=======================================



Overview
~~~~~~~~

TBD. :ref:`More...<details-class_inference_engine_1_1_const_transformer>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <graph_transformer.h>
	
	class ConstTransformer
	{
	public:
		// construction
	
		:target:`ConstTransformer<doxid-class_inference_engine_1_1_const_transformer_1a37002ff125163d1ebbb2918a1f95c2c6>`(details::CNNNetworkImpl \* _network);

		// methods
	
		void :ref:`foldConstSubgraphs<doxid-class_inference_engine_1_1_const_transformer_1aeafc3582d64304db0548e88c88a5d4c2>`();
		void :ref:`fullTrim<doxid-class_inference_engine_1_1_const_transformer_1a8565611ccfa285c3a41dd3165d8f6e36>`();
	};
.. _details-class_inference_engine_1_1_const_transformer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

TBD.

Methods
-------

.. _doxid-class_inference_engine_1_1_const_transformer_1aeafc3582d64304db0548e88c88a5d4c2:
.. index:: pair: function; foldConstSubgraphs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void foldConstSubgraphs()

calculates const layers, combines const subgraph into a single const layers

.. _doxid-class_inference_engine_1_1_const_transformer_1a8565611ccfa285c3a41dd3165d8f6e36:
.. index:: pair: function; fullTrim

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void fullTrim()

folds Const Subgraphs and removes second input of Reshape-like layers (Interp, Gather, Resample, ...)


