.. index:: pair: group; Threading utilities
.. _doxid-group__ie__dev__api__threading:

Threading utilities
===================

.. toctree::
	:hidden:

	ExecutorManager <classInferenceEngine_1_1ExecutorManager.rst>
	IStreamsExecutor <classInferenceEngine_1_1IStreamsExecutor.rst>
	ITaskExecutor <classInferenceEngine_1_1ITaskExecutor.rst>
	CPUStreamsExecutor <classInferenceEngine_1_1CPUStreamsExecutor.rst>
	ImmediateExecutor <classInferenceEngine_1_1ImmediateExecutor.rst>

Overview
~~~~~~~~

Threading API providing task executors for asynchronous operations. :ref:`More...<details-group__ie__dev__api__threading>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// typedefs

	typedef std::function<void()> :ref:`InferenceEngine::Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>`;
	typedef tbb::enumerable_thread_specific<T> :ref:`InferenceEngine::ThreadLocal<doxid-group__ie__dev__api__threading_1ga022081ac7bfdb2af060389c78eaa7f64>`;

	// templates

	template :ref:`InferenceEngine::ExecutorManager<doxid-class_inference_engine_1_1_executor_manager>`;
	template :ref:`InferenceEngine::IStreamsExecutor<doxid-class_inference_engine_1_1_i_streams_executor>`;
	template :ref:`InferenceEngine::ITaskExecutor<doxid-class_inference_engine_1_1_i_task_executor>`;

	// classes

	class :ref:`InferenceEngine::CPUStreamsExecutor<doxid-class_inference_engine_1_1_c_p_u_streams_executor>`;
	class :ref:`InferenceEngine::ImmediateExecutor<doxid-class_inference_engine_1_1_immediate_executor>`;

.. _details-group__ie__dev__api__threading:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Threading API providing task executors for asynchronous operations.

Typedefs
--------

.. _doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3:
.. index:: pair: typedef; Task

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<void()> InferenceEngine::Task

Inference Engine Task Executor can use any copyable callable without parameters and output as a task. It would be wrapped into std::function object.

.. _doxid-group__ie__dev__api__threading_1ga022081ac7bfdb2af060389c78eaa7f64:
.. index:: pair: typedef; ThreadLocal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef tbb::enumerable_thread_specific<T> InferenceEngine::ThreadLocal

A wrapper class to keep object to be thread local.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- A type of object to keep thread local.

