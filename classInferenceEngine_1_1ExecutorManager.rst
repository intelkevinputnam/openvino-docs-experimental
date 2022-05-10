.. index:: pair: interface; InferenceEngine::ExecutorManager
.. _doxid-class_inference_engine_1_1_executor_manager:

interface InferenceEngine::ExecutorManager
==========================================



Overview
~~~~~~~~

Interface for tasks execution manager. This is global point for getting task executor objects by string id. It's necessary in multiple asynchronous requests for having unique executors to avoid oversubscription. E.g. There 2 task executors for CPU device: one - in FPGA, another - in OneDNN. Parallel execution both of them leads to not optimal CPU usage. More efficient to run the corresponding tasks one by one via single executor. :ref:`More...<details-class_inference_engine_1_1_executor_manager>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_executor_manager.hpp>
	
	template ExecutorManager
	{
		// typedefs
	
		typedef std::shared_ptr<ExecutorManager> :ref:`Ptr<doxid-class_inference_engine_1_1_executor_manager_1a61cdb5158ef2e7ab36a3fbcaa87b546b>`;

		// methods
	
		virtual :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>` :ref:`getExecutor<doxid-class_inference_engine_1_1_executor_manager_1a392188acb1fe750fca913e2b5e0dc29c>`(const std::string& id) = 0;
		static ExecutorManager \* :ref:`getInstance<doxid-class_inference_engine_1_1_executor_manager_1a74c15cfdf9b645a58ff09f3aa8f908d7>`();
	};
.. _details-class_inference_engine_1_1_executor_manager:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Interface for tasks execution manager. This is global point for getting task executor objects by string id. It's necessary in multiple asynchronous requests for having unique executors to avoid oversubscription. E.g. There 2 task executors for CPU device: one - in FPGA, another - in OneDNN. Parallel execution both of them leads to not optimal CPU usage. More efficient to run the corresponding tasks one by one via single executor.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_executor_manager_1a61cdb5158ef2e7ab36a3fbcaa87b546b:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ExecutorManager> Ptr

A shared pointer to :ref:`ExecutorManager <doxid-class_inference_engine_1_1_executor_manager>` interface

Methods
-------

.. _doxid-class_inference_engine_1_1_executor_manager_1a392188acb1fe750fca913e2b5e0dc29c:
.. index:: pair: function; getExecutor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>` getExecutor(const std::string& id) = 0

Returns executor by unique identificator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- id

		- An unique identificator of device (Usually string representation of TargetDevice)



.. rubric:: Returns:

A shared pointer to existing or newly :ref:`ITaskExecutor <doxid-class_inference_engine_1_1_i_task_executor>`

.. _doxid-class_inference_engine_1_1_executor_manager_1a74c15cfdf9b645a58ff09f3aa8f908d7:
.. index:: pair: function; getInstance

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static ExecutorManager \* getInstance()

Returns a global instance of :ref:`ExecutorManager <doxid-class_inference_engine_1_1_executor_manager>`.



.. rubric:: Returns:

The instance.


