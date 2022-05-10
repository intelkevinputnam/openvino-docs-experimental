.. index:: pair: interface; InferenceEngine::IStreamsExecutor
.. _doxid-class_inference_engine_1_1_i_streams_executor:

interface InferenceEngine::IStreamsExecutor
===========================================

.. toctree::
	:hidden:

	ThreadBindingType <enumInferenceEngine_1_1IStreamsExecutor_1_1ThreadBindingType.rst>
	Config <structInferenceEngine_1_1IStreamsExecutor_1_1Config.rst>

Overview
~~~~~~~~

Interface for Streams Task Executor. This executor groups worker threads into so-called ``streams``. :ref:`More...<details-class_inference_engine_1_1_i_streams_executor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_istreams_executor.hpp>
	
	template IStreamsExecutor: public :ref:`InferenceEngine::ITaskExecutor<doxid-class_inference_engine_1_1_i_task_executor>`
	{
		// typedefs
	
		typedef std::shared_ptr<IStreamsExecutor> :ref:`Ptr<doxid-class_inference_engine_1_1_i_streams_executor_1aff6d8ddced217e4b062b194954c07497>`;

		// enums
	
		enum :ref:`ThreadBindingType<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>`;

		// structs
	
		struct :ref:`Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`;

		// methods
	
		virtual int :ref:`GetStreamId<doxid-class_inference_engine_1_1_i_streams_executor_1a557bdceaa533ea8991e3c5d894ef4636>`() = 0;
		virtual int :ref:`GetNumaNodeId<doxid-class_inference_engine_1_1_i_streams_executor_1a11e9552c9e1ae1aebacb15f8f58517f9>`() = 0;
		virtual void :ref:`Execute<doxid-class_inference_engine_1_1_i_streams_executor_1a55622043692017e8c6002d0bec344f0d>`(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0;
	};

	// direct descendants

	class :ref:`CPUStreamsExecutor<doxid-class_inference_engine_1_1_c_p_u_streams_executor>`;
	class :ref:`TBBStreamsExecutor<doxid-class_inference_engine_1_1_t_b_b_streams_executor>`;

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

.. _details-class_inference_engine_1_1_i_streams_executor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Interface for Streams Task Executor. This executor groups worker threads into so-called ``streams``.

The executor executes all parallel tasks using threads from one stream. With proper pinning settings it should reduce cache misses for memory bound workloads.

On NUMA hosts :ref:`GetNumaNodeId() <doxid-class_inference_engine_1_1_i_streams_executor_1a11e9552c9e1ae1aebacb15f8f58517f9>` method can be used to define the NUMA node of current stream

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_streams_executor_1aff6d8ddced217e4b062b194954c07497:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IStreamsExecutor> Ptr

A shared pointer to :ref:`IStreamsExecutor <doxid-class_inference_engine_1_1_i_streams_executor>` interface

Methods
-------

.. _doxid-class_inference_engine_1_1_i_streams_executor_1a557bdceaa533ea8991e3c5d894ef4636:
.. index:: pair: function; GetStreamId

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int GetStreamId() = 0

Return the index of current stream.



.. rubric:: Returns:

An index of current stream. Or throw exceptions if called not from stream thread

.. _doxid-class_inference_engine_1_1_i_streams_executor_1a11e9552c9e1ae1aebacb15f8f58517f9:
.. index:: pair: function; GetNumaNodeId

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int GetNumaNodeId() = 0

Return the id of current NUMA Node.



.. rubric:: Returns:

``ID`` of current NUMA Node, or throws exceptions if called not from stream thread

.. _doxid-class_inference_engine_1_1_i_streams_executor_1a55622043692017e8c6002d0bec344f0d:
.. index:: pair: function; Execute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Execute(:ref:`Task<doxid-group__ie__dev__api__threading_1gaa8e60514bef064f9ff4374919cffe1f3>` task) = 0

Execute the task in the current thread using streams executor configuration and constraints.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- task

		- A task to start


