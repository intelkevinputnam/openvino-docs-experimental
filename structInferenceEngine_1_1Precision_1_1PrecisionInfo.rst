.. index:: pair: struct; InferenceEngine::Precision::PrecisionInfo
.. _doxid-struct_inference_engine_1_1_precision_1_1_precision_info:

struct InferenceEngine::Precision::PrecisionInfo
================================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct PrecisionInfo
	{
		// fields
	
		size_t :ref:`bitsSize<doxid-struct_inference_engine_1_1_precision_1_1_precision_info_1a139478e0a669be9b1dc8b0ddfb76e784>` = 0;
		const char \* :ref:`name<doxid-struct_inference_engine_1_1_precision_1_1_precision_info_1aa8f76b3a704241345ab19b9ecc1c69de>` = "UNSPECIFIED";
		bool :target:`isFloat<doxid-struct_inference_engine_1_1_precision_1_1_precision_info_1a4a9be5f550d072d22e23c4467daeca84>` = false;
		:ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` :target:`value<doxid-struct_inference_engine_1_1_precision_1_1_precision_info_1ab0f22bf1bfce4378a2deb64a3cd3eeb9>` = :ref:`Precision::UNSPECIFIED<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ae27ff65d395667d17067e83d932a2045>`;
	};
.. _details-struct_inference_engine_1_1_precision_1_1_precision_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Fields
------

.. _doxid-struct_inference_engine_1_1_precision_1_1_precision_info_1a139478e0a669be9b1dc8b0ddfb76e784:
.. index:: pair: variable; bitsSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t bitsSize = 0

Size of underlined element.

.. _doxid-struct_inference_engine_1_1_precision_1_1_precision_info_1aa8f76b3a704241345ab19b9ecc1c69de:
.. index:: pair: variable; name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const char \* name = "UNSPECIFIED"

Null terminated string with precision name.


