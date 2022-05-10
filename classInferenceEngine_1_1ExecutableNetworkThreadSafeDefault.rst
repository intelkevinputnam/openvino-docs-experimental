.. index:: pair: class; InferenceEngine::ExecutableNetworkThreadSafeDefault
.. _doxid-class_inference_engine_1_1_executable_network_thread_safe_default:

class InferenceEngine::ExecutableNetworkThreadSafeDefault
=========================================================



Overview
~~~~~~~~

This class provides optimal thread safe default implementation. The class is recommended to be used as a base class for Executable Network impleentation during plugin development. :ref:`More...<details-class_inference_engine_1_1_executable_network_thread_safe_default>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_executable_network_thread_safe_default.hpp>
	
	class ExecutableNetworkThreadSafeDefault: public :ref:`InferenceEngine::IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<ExecutableNetworkThreadSafeDefault> :ref:`Ptr<doxid-class_inference_engine_1_1_executable_network_thread_safe_default_1a25bd3e0bdd759b05ee3318f87535bc17>`;

		// construction
	
		:ref:`ExecutableNetworkThreadSafeDefault<doxid-class_inference_engine_1_1_executable_network_thread_safe_default_1a999361ff119c0288c51884af4ba3b807>`(
			const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& taskExecutor = std::make_shared<:ref:`CPUStreamsExecutor<doxid-class_inference_engine_1_1_c_p_u_streams_executor>`>(:ref:`IStreamsExecutor::Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`{ "Default"}),
			const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& callbackExecutor = std::make_shared<:ref:`CPUStreamsExecutor<doxid-class_inference_engine_1_1_c_p_u_streams_executor>`>(:ref:`IStreamsExecutor::Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`{ "Callback"})
			);

		// methods
	
		virtual :ref:`IInferRequestInternal::Ptr<doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>` :ref:`CreateInferRequest<doxid-class_inference_engine_1_1_executable_network_thread_safe_default_1ab16d0cad93d2838b44acd261fd6ce367>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`Ptr<doxid-class_inference_engine_1_1_i_executable_network_internal_1a264e3e04130a2e44d0b257ae63c9feae>`;

		// methods
	
		virtual void :ref:`setNetworkInputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a516604bd1cedd1072d82eb82170aed18>`(const :ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& networkInputs);
		virtual void :ref:`setNetworkOutputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a6b795c8f85fe7acc1819e230bce6e4da>`(const :ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& networkOutputs);
		virtual void :ref:`setInputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a9417aa5772082d01cee2b19185835ad1>`(const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& params);
		virtual const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`getInputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1af02e0a16bf01c39514b005edd9743d7a>`() const;
		virtual void :ref:`setOutputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1ae529d59d4e19a45f60ea03af93e32fb9>`(const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& results);
		virtual const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`getOutputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a153bdd4f0da982ada15e257e2fd8d620>`() const;
		virtual :ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` :ref:`GetOutputsInfo<doxid-class_inference_engine_1_1_i_executable_network_internal_1ac6fbce66b52b33bb62709803b25f2a6e>`() const;
		virtual :ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` :ref:`GetInputsInfo<doxid-class_inference_engine_1_1_i_executable_network_internal_1a1529cab4d8385e21ef394b817f8c2230>`() const;
		virtual std::shared_ptr<:ref:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal>`> :ref:`CreateInferRequest<doxid-class_inference_engine_1_1_i_executable_network_internal_1ab5d5797a7ef239eeb20d1c3eadf1bd73>`();
		virtual void :ref:`Export<doxid-class_inference_engine_1_1_i_executable_network_internal_1a057bca9b0f955c03190bdf77635e9516>`(const std::string& modelFileName);
		virtual void :ref:`Export<doxid-class_inference_engine_1_1_i_executable_network_internal_1a2b5e212158cd5bf3a2f903cd405fdd3d>`(std::ostream& networkModel);
		virtual std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`GetExecGraphInfo<doxid-class_inference_engine_1_1_i_executable_network_internal_1aeb29d9f35b340496272f785d7be4f097>`();
		virtual void :ref:`SetPointerToPlugin<doxid-class_inference_engine_1_1_i_executable_network_internal_1a13df5cff9daf69a68365509ad11a5b1f>`(const std::shared_ptr<:ref:`IInferencePlugin<doxid-class_inference_engine_1_1_i_inference_plugin>`>& plugin);
		virtual void :ref:`SetConfig<doxid-class_inference_engine_1_1_i_executable_network_internal_1a66bc34d51b798322d29ec1b1a8332faa>`(const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config);
		virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-class_inference_engine_1_1_i_executable_network_internal_1aab6b3c29e3fec7400548b0af1808a772>`(const std::string& name) const;
		virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetMetric<doxid-class_inference_engine_1_1_i_executable_network_internal_1abff44a61825a0da77a4a329225431708>`(const std::string& name) const;
		virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`GetContext<doxid-class_inference_engine_1_1_i_executable_network_internal_1a3a14f4c13bf0ba5470278d762cefc356>`() const;

.. _details-class_inference_engine_1_1_executable_network_thread_safe_default:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class provides optimal thread safe default implementation. The class is recommended to be used as a base class for Executable Network impleentation during plugin development.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_executable_network_thread_safe_default_1a25bd3e0bdd759b05ee3318f87535bc17:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ExecutableNetworkThreadSafeDefault> Ptr

A shared pointer to a :ref:`ExecutableNetworkThreadSafeDefault <doxid-class_inference_engine_1_1_executable_network_thread_safe_default>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_executable_network_thread_safe_default_1a999361ff119c0288c51884af4ba3b807:
.. index:: pair: function; ExecutableNetworkThreadSafeDefault

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ExecutableNetworkThreadSafeDefault(
		const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& taskExecutor = std::make_shared<:ref:`CPUStreamsExecutor<doxid-class_inference_engine_1_1_c_p_u_streams_executor>`>(:ref:`IStreamsExecutor::Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`{ "Default"}),
		const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& callbackExecutor = std::make_shared<:ref:`CPUStreamsExecutor<doxid-class_inference_engine_1_1_c_p_u_streams_executor>`>(:ref:`IStreamsExecutor::Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config>`{ "Callback"})
		)

Constructs a new instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- taskExecutor

		- The task executor used

	*
		- callbackExecutor

		- The callback executor

Methods
-------

.. _doxid-class_inference_engine_1_1_executable_network_thread_safe_default_1ab16d0cad93d2838b44acd261fd6ce367:
.. index:: pair: function; CreateInferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`IInferRequestInternal::Ptr<doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>` CreateInferRequest()

Given optional implementation of creating asynchronous inference request to avoid need for it to be implemented by plugin.



.. rubric:: Returns:

shared_ptr for the created asynchronous inference request


