.. index:: pair: interface; InferenceEngine::ITaskExecutor
.. _doxid-class_inference_engine_1_1_i_task_executor:

interface InferenceEngine::ITaskExecutor
========================================



Overview
~~~~~~~~

Interface for Task Executor. Inference Engine uses ``:ref:`InferenceEngine::ITaskExecutor <doxid-class_inference_engine_1_1_i_task_executor>``` interface to run all asynchronous internal tasks. Different implementations of task executors can be used for different purposes: :ref:`More...<details-class_inference_engine_1_1_i_task_executor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_itask_executor.hpp>
	
	template ITaskExecutor
	{
		// typedefs
	
		typedef std::shared_ptr<ITaskExecutor> :ref:`Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`;

		// methods
	
		virtual void :ref:`run<doxid-class_inference_engine_1_1_i_task_executor_1a2cd274d70293c89f44d4ac9b44b9d916>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0;
		virtual void :ref:`runAndWait<doxid-class_inference_engine_1_1_i_task_executor_1ad890ea0431e41e18efd8b01d70f0550d>`(const std::vector<:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>`>& tasks);
	};

	// direct descendants

	class :ref:`ImmediateExecutor<doxid-class_inference_engine_1_1_immediate_executor>`;
	template :ref:`IStreamsExecutor<doxid-class_inference_engine_1_1_i_streams_executor>`;
.. _details-class_inference_engine_1_1_i_task_executor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Interface for Task Executor. Inference Engine uses ``:ref:`InferenceEngine::ITaskExecutor <doxid-class_inference_engine_1_1_i_task_executor>``` interface to run all asynchronous internal tasks. Different implementations of task executors can be used for different purposes:

* To improve cache locality of memory bound CPU tasks some executors can limit task's affinity and maximum concurrency.

* The executor with one worker thread can be used to serialize access to acceleration device.

* Immediate task executor can be used to satisfy ``:ref:`InferenceEngine::ITaskExecutor <doxid-class_inference_engine_1_1_i_task_executor>``` interface restrictions but run tasks in current thread. Implementation should guaranty thread safety of all methods



.. _doxid-class_inference_engine_1_1_i_task_executor_1Synchronization:

Synchronization
~~~~~~~~~~~~~~~

It is ``:ref:`InferenceEngine::ITaskExecutor <doxid-class_inference_engine_1_1_i_task_executor>``` user responsibility to wait for task execution completion. The ``c++11`` standard way to wait task completion is to use ``std::packaged_task`` or ``std::promise`` with ``std::future``. Here is an example of how to use ``std::promise`` to wait task completion and process task's exceptions:

.. ref-code-block:: cpp

	// std::promise is move only object so to satisfy copy callable constraint we use std::shared_ptr
	auto promise = std::make_shared<std::promise<void>>();
	// When the promise is created we can get std::future to wait the result
	auto future = promise->get_future();
	// Rather simple task
	:ref:`InferenceEngine::Task <doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task = [] {std::cout << "Some Output" << std::endl; };
	// Create an executor
	:ref:`InferenceEngine::ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>` taskExecutor = std::make_shared<InferenceEngine::CPUStreamsExecutor>();
	if (taskExecutor == nullptr) {
	    // ProcessError(e);
	    return;
	}
	// We capture the task and the promise. When the task is executed in the task executor context
	// we munually call std::promise::set_value() method
	taskExecutor->run([task, promise] {
	    std::exception_ptr currentException;
	    try {
	        task();
	    } catch(...) {
	        // If there is some exceptions store the pointer to current exception
	        currentException = std::current_exception();
	    }

	    if (nullptr == currentException) {
	        promise->set_value();  //  <-- If there is no problems just call std::promise::set_value()
	    } else {
	        promise->set_exception(currentException);    //  <-- If there is an exception forward it to std::future object
	    }
	});
	// To wait the task completion we call std::future::wait method
	future.wait();  //  The current thread will be blocked here and wait when std::promise::set_value()
	                //  or std::promise::set_exception() method will be called.

	// If the future store the exception it will be rethrown in std::future::get method
	try {
	    future.get();
	} catch(std::exception& /\*e\*/) {
	    // ProcessError(e);
	}

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ITaskExecutor> Ptr

A shared pointer to :ref:`ITaskExecutor <doxid-class_inference_engine_1_1_i_task_executor>` interface

Methods
-------

.. _doxid-class_inference_engine_1_1_i_task_executor_1a2cd274d70293c89f44d4ac9b44b9d916:
.. index:: pair: function; run

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void run(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0

Execute :ref:`InferenceEngine::Task <doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` inside task executor context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- task

		- A task to start

.. _doxid-class_inference_engine_1_1_i_task_executor_1ad890ea0431e41e18efd8b01d70f0550d:
.. index:: pair: function; runAndWait

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void runAndWait(const std::vector<:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>`>& tasks)

Execute all of the tasks and waits for its completion. Default :ref:`runAndWait() <doxid-class_inference_engine_1_1_i_task_executor_1ad890ea0431e41e18efd8b01d70f0550d>` method implementation uses :ref:`run() <doxid-class_inference_engine_1_1_i_task_executor_1a2cd274d70293c89f44d4ac9b44b9d916>` pure virtual method and higher level synchronization primitives from STL. The task is wrapped into std::packaged_task which returns std::future. std::packaged_task will call the task and signal to std::future that the task is finished or the exception is thrown from task Than std::future is used to wait for task execution completion and task exception extraction.

:ref:`runAndWait() <doxid-class_inference_engine_1_1_i_task_executor_1ad890ea0431e41e18efd8b01d70f0550d>` does not copy or capture tasks!



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tasks

		- A vector of tasks to execute


