.. index:: pair: struct; InferenceEngine::PreProcessChannel
.. _doxid-struct_inference_engine_1_1_pre_process_channel:

struct InferenceEngine::PreProcessChannel
=========================================



Overview
~~~~~~~~

This structure stores info about pre-processing of network inputs (scale, mean image, ...) :ref:`More...<details-struct_inference_engine_1_1_pre_process_channel>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess.hpp>
	
	struct PreProcessChannel
	{
		// typedefs
	
		typedef std::shared_ptr<PreProcessChannel> :ref:`Ptr<doxid-struct_inference_engine_1_1_pre_process_channel_1abde989b919c44225ea30dbacb64f34b2>`;

		// fields
	
		float :ref:`stdScale<doxid-struct_inference_engine_1_1_pre_process_channel_1a9a9ca23fe117f2527353d149c4371d5f>` = 1;
		float :ref:`meanValue<doxid-struct_inference_engine_1_1_pre_process_channel_1aacce6a0fa2b43256b1793a6db08b4b01>` = 0;
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`meanData<doxid-struct_inference_engine_1_1_pre_process_channel_1a4c40c2ad85a101f7d4f3b1e739125c85>`;
	};
.. _details-struct_inference_engine_1_1_pre_process_channel:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This structure stores info about pre-processing of network inputs (scale, mean image, ...)

Typedefs
--------

.. _doxid-struct_inference_engine_1_1_pre_process_channel_1abde989b919c44225ea30dbacb64f34b2:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<PreProcessChannel> Ptr

Smart pointer to an instance.

Fields
------

.. _doxid-struct_inference_engine_1_1_pre_process_channel_1a9a9ca23fe117f2527353d149c4371d5f:
.. index:: pair: variable; stdScale

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float stdScale = 1

Scale parameter for a channel.

.. _doxid-struct_inference_engine_1_1_pre_process_channel_1aacce6a0fa2b43256b1793a6db08b4b01:
.. index:: pair: variable; meanValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float meanValue = 0

Mean value for a channel.

.. _doxid-struct_inference_engine_1_1_pre_process_channel_1a4c40c2ad85a101f7d4f3b1e739125c85:
.. index:: pair: variable; meanData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` meanData

Mean data for a channel.


