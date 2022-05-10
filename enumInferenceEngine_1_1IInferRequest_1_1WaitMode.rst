.. index:: pair: enum; WaitMode
.. _doxid-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848:

enum InferenceEngine::IInferRequest::WaitMode
=============================================

Overview
~~~~~~~~

Enumeration to hold wait mode for :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>`. :ref:`More...<details-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iinfer_request.hpp>

	enum WaitMode
	{
	    :ref:`RESULT_READY<doxid-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848aaf5018bbb6697150c76024689c52dfc9>` = -1,
	    :ref:`STATUS_ONLY<doxid-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848a20d3cbd0ec08c92f859e830d5dad8cb4>`  = 0,
	};

.. _details-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enumeration to hold wait mode for :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>`.

Enum Values
-----------

.. _doxid-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848aaf5018bbb6697150c76024689c52dfc9:
.. index:: pair: enumvalue; RESULT_READY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RESULT_READY

Wait until inference result becomes available

.. _doxid-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848a20d3cbd0ec08c92f859e830d5dad8cb4:
.. index:: pair: enumvalue; STATUS_ONLY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	STATUS_ONLY

:ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` doesn't block or interrupt current thread and immediately returns inference status

