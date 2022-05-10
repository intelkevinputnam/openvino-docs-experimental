.. index:: pair: class; InferenceEngine::TBBStreamsExecutor
.. _doxid-class_inference_engine_1_1_t_b_b_streams_executor:

class InferenceEngine::TBBStreamsExecutor
=========================================



Overview
~~~~~~~~

CPU Streams executor implementation. Use TBB thread pool to run tasks. :ref:`More...<details-class_inference_engine_1_1_t_b_b_streams_executor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_tbb_streams_executor.hpp>
	
	class TBBStreamsExecutor: public :ref:`InferenceEngine::IStreamsExecutor<doxid-class_inference_engine_1_1_i_streams_executor>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<TBBStreamsExecutor> :target:`Ptr<doxid-class_inference_engine_1_1_t_b_b_streams_executor_1a287b450625bd060e3649f80c1eb95ffd>`;

		// construction
	
		:target:`TBBStreamsExecutor<doxid-class_inference_engine_1_1_t_b_b_streams_executor_1a9e68d85247db57caeab4c3cd5c6f8518>`(const :ref:`Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`& config = {});

		// methods
	
		virtual void :ref:`run<doxid-class_inference_engine_1_1_t_b_b_streams_executor_1ac2ce4451149f06dc68fd0165a817d3a5>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task);
		virtual void :ref:`Execute<doxid-class_inference_engine_1_1_t_b_b_streams_executor_1aec33ce110f23e8ff352473232f70ede5>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task);
		virtual int :ref:`GetStreamId<doxid-class_inference_engine_1_1_t_b_b_streams_executor_1ab5ad40cb4be8b821eb228c084738da15>`();
		virtual int :ref:`GetNumaNodeId<doxid-class_inference_engine_1_1_t_b_b_streams_executor_1a1b83bfa815832e16586a1522d5eb01be>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`ITaskExecutor<doxid-class_inference_engine_1_1_i_task_executor>`> :ref:`Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`;
		typedef std::shared_ptr<:ref:`IStreamsExecutor<doxid-class_inference_engine_1_1_i_streams_executor>`> :ref:`Ptr<doxid-class_inference_engine_1_1_i_streams_executor_1aff6d8ddced217e4b062b194954c07497>`;

		// enums
	
		enum :ref:`ThreadBindingType<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>`;

		// structs
	
		struct :ref:`Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`;

		// methods
	
		virtual void :ref:`run<doxid-class_inference_engine_1_1_i_task_executor_1a2cd274d70293c89f44d4ac9b44b9d916>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0;
		virtual void :ref:`runAndWait<doxid-class_inference_engine_1_1_i_task_executor_1ad890ea0431e41e18efd8b01d70f0550d>`(const std::vector<:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>`>& tasks);
		virtual int :ref:`GetStreamId<doxid-class_inference_engine_1_1_i_streams_executor_1a557bdceaa533ea8991e3c5d894ef4636>`() = 0;
		virtual int :ref:`GetNumaNodeId<doxid-class_inference_engine_1_1_i_streams_executor_1a11e9552c9e1ae1aebacb15f8f58517f9>`() = 0;
		virtual void :ref:`Execute<doxid-class_inference_engine_1_1_i_streams_executor_1a55622043692017e8c6002d0bec344f0d>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0;

.. _details-class_inference_engine_1_1_t_b_b_streams_executor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

CPU Streams executor implementation. Use TBB thread pool to run tasks.

Methods
-------

.. _doxid-class_inference_engine_1_1_t_b_b_streams_executor_1ac2ce4451149f06dc68fd0165a817d3a5:
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

.. _doxid-class_inference_engine_1_1_t_b_b_streams_executor_1aec33ce110f23e8ff352473232f70ede5:
.. index:: pair: function; Execute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Execute(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task)

Execute the task in the current thread using streams executor configuration and constraints.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- task

		- A task to start

.. _doxid-class_inference_engine_1_1_t_b_b_streams_executor_1ab5ad40cb4be8b821eb228c084738da15:
.. index:: pair: function; GetStreamId

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int GetStreamId()

Return the index of current stream.



.. rubric:: Returns:

An index of current stream. Or throw exceptions if called not from stream thread

.. _doxid-class_inference_engine_1_1_t_b_b_streams_executor_1a1b83bfa815832e16586a1522d5eb01be:
.. index:: pair: function; GetNumaNodeId

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int GetNumaNodeId()

Return the id of current NUMA Node.



.. rubric:: Returns:

``ID`` of current NUMA Node, or throws exceptions if called not from stream thread


