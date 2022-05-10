.. index:: pair: struct; InferenceEngine::AsyncInferRequestThreadSafeDefault::ImmediateStreamsExecutor
.. _doxid-struct_inference_engine_1_1_async_infer_request_thread_safe_default_1_1_immediate_streams_executor:

struct InferenceEngine::AsyncInferRequestThreadSafeDefault::ImmediateStreamsExecutor
====================================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct ImmediateStreamsExecutor: public :ref:`InferenceEngine::ITaskExecutor<doxid-class_inference_engine_1_1_i_task_executor>`
	{
		// fields
	
		:ref:`IStreamsExecutor::Ptr<doxid-class_inference_engine_1_1_i_streams_executor_1aff6d8ddced217e4b062b194954c07497>` :target:`_streamsExecutor<doxid-struct_inference_engine_1_1_async_infer_request_thread_safe_default_1_1_immediate_streams_executor_1adb36e5745c8e6c82e7cad88f0fdfa7da>`;

		// construction
	
		:target:`ImmediateStreamsExecutor<doxid-struct_inference_engine_1_1_async_infer_request_thread_safe_default_1_1_immediate_streams_executor_1ac61abfcc560dae952a8dda6aa9385a1d>`(const :ref:`IStreamsExecutor::Ptr<doxid-class_inference_engine_1_1_i_streams_executor_1aff6d8ddced217e4b062b194954c07497>`& streamsExecutor);

		// methods
	
		void :target:`run<doxid-struct_inference_engine_1_1_async_infer_request_thread_safe_default_1_1_immediate_streams_executor_1ac4d861784f351a7de95962388ced2519>`(:ref:`InferenceEngine::Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`ITaskExecutor<doxid-class_inference_engine_1_1_i_task_executor>`> :ref:`Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`;

		// methods
	
		virtual void :ref:`run<doxid-class_inference_engine_1_1_i_task_executor_1a2cd274d70293c89f44d4ac9b44b9d916>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0;
		virtual void :ref:`runAndWait<doxid-class_inference_engine_1_1_i_task_executor_1ad890ea0431e41e18efd8b01d70f0550d>`(const std::vector<:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>`>& tasks);


