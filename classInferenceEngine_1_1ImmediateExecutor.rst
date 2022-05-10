.. index:: pair: class; InferenceEngine::ImmediateExecutor
.. _doxid-class_inference_engine_1_1_immediate_executor:

class InferenceEngine::ImmediateExecutor
========================================



Overview
~~~~~~~~

Task executor implementation that just run tasks in current thread during calling of :ref:`run() <doxid-class_inference_engine_1_1_immediate_executor_1a384a7ce3534f76678be85062c6295f08>` method. :ref:`More...<details-class_inference_engine_1_1_immediate_executor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_immediate_executor.hpp>
	
	class ImmediateExecutor: public :ref:`InferenceEngine::ITaskExecutor<doxid-class_inference_engine_1_1_i_task_executor>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<ImmediateExecutor> :ref:`Ptr<doxid-class_inference_engine_1_1_immediate_executor_1a95f9d36ddad1ed2dccacd43494f9ed13>`;

		// methods
	
		virtual void :ref:`run<doxid-class_inference_engine_1_1_immediate_executor_1a384a7ce3534f76678be85062c6295f08>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task);
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

.. _details-class_inference_engine_1_1_immediate_executor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Task executor implementation that just run tasks in current thread during calling of :ref:`run() <doxid-class_inference_engine_1_1_immediate_executor_1a384a7ce3534f76678be85062c6295f08>` method.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_immediate_executor_1a95f9d36ddad1ed2dccacd43494f9ed13:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ImmediateExecutor> Ptr

A shared pointer to a :ref:`ImmediateExecutor <doxid-class_inference_engine_1_1_immediate_executor>` object.

Methods
-------

.. _doxid-class_inference_engine_1_1_immediate_executor_1a384a7ce3534f76678be85062c6295f08:
.. index:: pair: function; run

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void run(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task)

Execute :ref:`InferenceEngine::Task <doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` inside task executor context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- task

		- A task to start


