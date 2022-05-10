.. index:: pair: struct; InferenceEngine::InferRequest::SetCallback
.. _doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback:

struct InferenceEngine::InferRequest::SetCallback
=================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename T>
	struct SetCallback
	{
		// fields
	
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request>`& :target:`_this<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_1ade7eaeb7652f14882863e030ca62c44f>`;

		// methods
	
		void :target:`operator ()<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_1a47db57094eecf009ff07479c3c6b5cda>` (std::function<void()> f);
	};

.. index:: pair: struct; InferenceEngine::InferRequest::SetCallback<IInferRequest::CompletionCallback>
.. _doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01_i_infer_request_1_1_completion_callback_01_4:

struct InferenceEngine::InferRequest::SetCallback<IInferRequest::CompletionCallback>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <>
	struct SetCallback<IInferRequest::CompletionCallback>
	{
		// fields
	
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request>`& :target:`_this<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01_i_infer_request_1_1_completion_callback_01_4_1a9c8c1d8fb20e82d67548262562750deb>`;

		// methods
	
		void :target:`operator ()<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01_i_infer_request_1_1_completion_callback_01_4_1a5f0ddee8b27c8cd154a7e6e2e246a31b>` (:ref:`IInferRequest::CompletionCallback<doxid-class_inference_engine_1_1_i_infer_request_1a2a47e12b5e922df747d90a126de4ed78>` f);
	};

.. index:: pair: struct; InferenceEngine::InferRequest::SetCallback<std::function<void(InferRequest, StatusCode)>>
.. _doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01std_1_1function_3_01void_07_inferd36a10d7c08edcd1bda12bce9578bb66:

struct InferenceEngine::InferRequest::SetCallback<std::function<void(InferRequest, StatusCode)>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <>
	struct SetCallback<std::function<void(InferRequest, StatusCode)>>
	{
		// fields
	
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request>`& :target:`_this<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01std_1_1function_3_01void_07_inferd36a10d7c08edcd1bda12bce9578bb66_1a7b047f4b4ef7752e104499064eb6ce83>`;

		// methods
	
		void :target:`operator ()<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01std_1_1function_3_01void_07_inferd36a10d7c08edcd1bda12bce9578bb66_1ad1a42d95b1e9a8fb3a44e4cb77109a3f>` (std::function<void(:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request>`, :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>`)> f);
	};

