.. index:: pair: struct; InferenceEngine::TensorIterator::Body
.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body:

struct InferenceEngine::TensorIterator::Body
============================================



Overview
~~~~~~~~

Describes a tensor iterator body. :ref:`More...<details-struct_inference_engine_1_1_tensor_iterator_1_1_body>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	struct Body
	{
		// fields
	
		std::vector<:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`> :ref:`inputs<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body_1aa214dc368906f0aaa913430d7588120b>`;
		std::vector<:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`> :ref:`outputs<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body_1ab053ff1a6d9bf0fa34e668998edf66b2>`;
	};
.. _details-struct_inference_engine_1_1_tensor_iterator_1_1_body:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Describes a tensor iterator body.

Fields
------

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body_1aa214dc368906f0aaa913430d7588120b:
.. index:: pair: variable; inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`> inputs

Inputs data.

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body_1ab053ff1a6d9bf0fa34e668998edf66b2:
.. index:: pair: variable; outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`> outputs

Outputs data.


