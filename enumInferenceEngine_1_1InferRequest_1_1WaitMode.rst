.. index:: pair: enum; WaitMode
.. _doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45a:

enum InferenceEngine::InferRequest::WaitMode
============================================

Overview
~~~~~~~~

Enumeration to hold wait mode for :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>`. :ref:`More...<details-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45a>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_infer_request.hpp>

	enum WaitMode
	{
	    :ref:`RESULT_READY<doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45aaa71f7b3aaba799f92c75c52ac56897d8>` = -1,
	    :ref:`STATUS_ONLY<doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45aa50110aaf0c2f26c0cc71acf022d91698>`  = 0,
	};

.. _details-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45a:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enumeration to hold wait mode for :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>`.

Enum Values
-----------

.. _doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45aaa71f7b3aaba799f92c75c52ac56897d8:
.. index:: pair: enumvalue; RESULT_READY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RESULT_READY

Wait until inference result becomes available

.. _doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45aa50110aaf0c2f26c0cc71acf022d91698:
.. index:: pair: enumvalue; STATUS_ONLY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	STATUS_ONLY

:ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` doesn't block or interrupt current thread and immediately returns inference status

