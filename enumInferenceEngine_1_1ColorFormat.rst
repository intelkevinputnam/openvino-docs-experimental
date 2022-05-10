.. index:: pair: enum; ColorFormat
.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a:

enum InferenceEngine::ColorFormat
=================================

Overview
~~~~~~~~



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>

	enum ColorFormat
	{
	    :ref:`RAW<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa1af35e096785969a23b3048b2b0fc06b>`  = 0u,
	    :ref:`RGB<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aae2262afdcd9754598dbc87e4a4725246>`,
	    :ref:`BGR<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa0fb221afef06def7c25b82d6fa9efc1b>`,
	    :ref:`RGBX<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa7ae5805f878c77d92c277585c41df041>`,
	    :ref:`BGRX<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa7c8c993b330b43405bd10ad36f81ec0a>`,
	    :ref:`NV12<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa502b46f938a363e107246de8b1c90dc7>`,
	    :ref:`I420<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aaba5a454c78774eae8999448b33f91813>`,
	};

.. _details-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Enum Values
-----------

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa1af35e096785969a23b3048b2b0fc06b:
.. index:: pair: enumvalue; RAW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RAW

Plain blob (default), no extra color processing required.

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aae2262afdcd9754598dbc87e4a4725246:
.. index:: pair: enumvalue; RGB

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RGB

RGB color format.

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa0fb221afef06def7c25b82d6fa9efc1b:
.. index:: pair: enumvalue; BGR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BGR

BGR color format, default in DLDT.

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa7ae5805f878c77d92c277585c41df041:
.. index:: pair: enumvalue; RGBX

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RGBX

RGBX color format with X ignored during inference.

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa7c8c993b330b43405bd10ad36f81ec0a:
.. index:: pair: enumvalue; BGRX

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BGRX

BGRX color format with X ignored during inference.

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aa502b46f938a363e107246de8b1c90dc7:
.. index:: pair: enumvalue; NV12

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NV12

NV12 color format represented as compound Y+UV blob.

.. _doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558aaba5a454c78774eae8999448b33f91813:
.. index:: pair: enumvalue; I420

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I420

I420 color format represented as compound Y+U+V blob.

