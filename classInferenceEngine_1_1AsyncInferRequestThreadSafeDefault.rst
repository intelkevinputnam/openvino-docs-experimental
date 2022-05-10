.. index:: pair: class; InferenceEngine::AsyncInferRequestThreadSafeDefault
.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default:

class InferenceEngine::AsyncInferRequestThreadSafeDefault
=========================================================

.. toctree::
	:hidden:

	DisableCallbackGuard <structInferenceEngine_1_1AsyncInferRequestThreadSafeDefault_1_1DisableCallbackGuard.rst>
	ImmediateStreamsExecutor <structInferenceEngine_1_1AsyncInferRequestThreadSafeDefault_1_1ImmediateStreamsExecutor.rst>

Overview
~~~~~~~~

Base class with default implementation of asynchronous multi staged inference request. To customize pipeline stages derived class should change the content of :ref:`AsyncInferRequestThreadSafeDefault::_pipeline <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ace49df30feb600773ef07fb080380ec6>` member container. It consists of pairs of tasks and executors which will run the task. The class is recommended to be used by plugins as a base class for asynchronous inference request implementation. :ref:`More...<details-class_inference_engine_1_1_async_infer_request_thread_safe_default>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_infer_async_request_thread_safe_default.hpp>
	
	class AsyncInferRequestThreadSafeDefault: public :ref:`InferenceEngine::IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<AsyncInferRequestThreadSafeDefault> :ref:`Ptr<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a39aef32e4145a9a755a2df1ca9c09bae>`;

		// structs
	
		struct :ref:`DisableCallbackGuard<doxid-struct_inference_engine_1_1_async_infer_request_thread_safe_default_1_1_disable_callback_guard>`;
		struct :ref:`ImmediateStreamsExecutor<doxid-struct_inference_engine_1_1_async_infer_request_thread_safe_default_1_1_immediate_streams_executor>`;

		// construction
	
		:ref:`AsyncInferRequestThreadSafeDefault<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a4de1e75c94a322839a0aa48d41b34003>`(
			const :ref:`IInferRequestInternal::Ptr<doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>`& request,
			const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& taskExecutor,
			const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& callbackExecutor
			);

		// methods
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Wait<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a146ee9027a2d2c44472e71efc429677f>`(int64_t millis_timeout);
		virtual void :ref:`StartAsync<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a93620dd73da915b3a2d53158ef722956>`();
		virtual void :ref:`Infer<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a3b98f918a8fb6180ea3f167f2137bc32>`();
		virtual std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`> :ref:`GetPerformanceCounts<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a16c0837c4f6f6a4bedc5063a37950337>`() const;
		virtual void :ref:`SetBlob<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a32610548fd783ff2835875e1df815868>`(const std::string& name, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data);
	
		virtual void :ref:`SetBlob<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1aa4d141581250971ada97b506943e55b4>`(
			const std::string& name,
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info
			);
	
		virtual void :ref:`SetBlobs<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a3595ab110716a90c006b293cec7ba86c>`(
			const std::string& name,
			const std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& blobs
			);
	
		virtual :ref:`BatchedBlob::Ptr<doxid-class_inference_engine_1_1_batched_blob_1ac66bc6bfae9ffc4be2de9c1d2f9e4208>` :ref:`GetBlobs<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a41da62beae65156a719d1150bebd729a>`(const std::string& name);
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`GetBlob<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a5b34292297524421d6756222178856a6>`(const std::string& name);
		virtual const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& :ref:`GetPreProcess<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ad5ea95b5687b3b5443c77b08e8a53298>`(const std::string& name) const;
		virtual void :ref:`SetBatch<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a46c22dbc3e654a701e1b426190716e5d>`(int batch);
		virtual void :ref:`SetCallback<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a4c4f1ad53d5fe14a4f3f5e32e08c468a>`(:ref:`Callback<doxid-class_inference_engine_1_1_i_infer_request_internal_1a705346c27474676ee28370ecc0cc99e9>` callback);
		virtual std::vector<std::shared_ptr<:ref:`InferenceEngine::IVariableStateInternal<doxid-class_inference_engine_1_1_i_variable_state_internal>`>> :ref:`QueryState<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ac90c7ad04aef96be77d1c11556867483>`();
		void :target:`ThrowIfCanceled<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ae29ba5feafc5641eba09f964fcb5d5eb>`() const;
		virtual void :ref:`Cancel<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a3a5904da5a3deb12ce8890964bb68fe8>`();
	
		virtual void :ref:`setModelInputsOutputs<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a9183e86d3516539bd11b72200518e264>`(
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& inputs,
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& outputs
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal>`> :ref:`Ptr<doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>`;
		typedef std::function<void(std::exception_ptr)> :ref:`Callback<doxid-class_inference_engine_1_1_i_infer_request_internal_1a705346c27474676ee28370ecc0cc99e9>`;

		// methods
	
		virtual void :ref:`Infer<doxid-class_inference_engine_1_1_i_infer_request_internal_1afb61e1de4ffb9927431085a91a40f352>`();
		virtual void :ref:`InferImpl<doxid-class_inference_engine_1_1_i_infer_request_internal_1a0ff052d969d599023769a8f5f3a75a56>`();
		virtual void :ref:`Cancel<doxid-class_inference_engine_1_1_i_infer_request_internal_1a23c9e992c9c4c94348bfc44f12e65148>`();
		virtual std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`> :ref:`GetPerformanceCounts<doxid-class_inference_engine_1_1_i_infer_request_internal_1a2eefb67a9766a29e032dc57bbf26d592>`() const;
		virtual void :ref:`SetBlob<doxid-class_inference_engine_1_1_i_infer_request_internal_1aaf6f8482fd4e8220edb8cb08558a4d6c>`(const std::string& name, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data);
	
		virtual void :ref:`SetBlobs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a0f1bb1a172ed84212ac1ead1ea131cd6>`(
			const std::string& name,
			const std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& blobs
			);
	
		virtual void :ref:`SetBlobsImpl<doxid-class_inference_engine_1_1_i_infer_request_internal_1a55ffc43c997b9e2034048523724a1a9a>`(
			const std::string& name,
			const :ref:`BatchedBlob::Ptr<doxid-class_inference_engine_1_1_batched_blob_1ac66bc6bfae9ffc4be2de9c1d2f9e4208>`& batched_blob
			);
	
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`GetBlob<doxid-class_inference_engine_1_1_i_infer_request_internal_1ad15f46c840f339ee2dd5e827ad003166>`(const std::string& name);
		virtual :ref:`BatchedBlob::Ptr<doxid-class_inference_engine_1_1_batched_blob_1ac66bc6bfae9ffc4be2de9c1d2f9e4208>` :ref:`GetBlobs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a5521c5aca27d7493a5f2ee64d80beeb3>`(const std::string& name);
	
		virtual void :ref:`SetBlob<doxid-class_inference_engine_1_1_i_infer_request_internal_1a7e7269ff954409b76f35f7c910bbd1a3>`(
			const std::string& name,
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info
			);
	
		virtual const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& :ref:`GetPreProcess<doxid-class_inference_engine_1_1_i_infer_request_internal_1a0e598a7f365c30131645efa621c06ef3>`(const std::string& name) const;
		virtual void :ref:`SetBatch<doxid-class_inference_engine_1_1_i_infer_request_internal_1a5c2bd4827dd9f2852cd7d9b5c45e4ed2>`(int batch);
		virtual std::vector<std::shared_ptr<:ref:`IVariableStateInternal<doxid-class_inference_engine_1_1_i_variable_state_internal>`>> :ref:`QueryState<doxid-class_inference_engine_1_1_i_infer_request_internal_1adba24bc7f20b0f104ae4f8015b39ad44>`();
		virtual void :ref:`StartAsync<doxid-class_inference_engine_1_1_i_infer_request_internal_1a9386941427f51f918d0b385398c576c2>`();
		virtual void :ref:`StartAsyncImpl<doxid-class_inference_engine_1_1_i_infer_request_internal_1a5d69abeffffb707beb1c1cd65630a03b>`();
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Wait<doxid-class_inference_engine_1_1_i_infer_request_internal_1a313dae76fabb6d73014129bf548291f0>`(int64_t millis_timeout);
		virtual void :ref:`SetCallback<doxid-class_inference_engine_1_1_i_infer_request_internal_1adb5b5d5bfc3fa74546ea2c85ff88fab8>`(:ref:`Callback<doxid-class_inference_engine_1_1_i_infer_request_internal_1a705346c27474676ee28370ecc0cc99e9>` callback);
	
		void :ref:`checkBlob<doxid-class_inference_engine_1_1_i_infer_request_internal_1a175d83da2b71b5c14f01fc242ec09e12>`(
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& blob,
			const std::string& name,
			bool isInput,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& refDims = {}
			) const;
	
		virtual void :ref:`checkBlobs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a19870e5b688afc41fd83c9c71841643c>`();
		void :ref:`setPointerToExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_infer_request_internal_1a9ad11a9ae33f3cf06318c804d1ccb73c>`(const std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`>& exeNetwork);
		std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`getPointerToExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_infer_request_internal_1a2176ee53c08047041a69dd9c11427198>`() const;
		void \* :ref:`GetUserData<doxid-class_inference_engine_1_1_i_infer_request_internal_1aa64164e3f73f98153c1bad633b2cbb56>`();
		void :ref:`SetUserData<doxid-class_inference_engine_1_1_i_infer_request_internal_1ab21acbb31b2311fd97e6b5f5a07538e6>`(void \* userData);
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`GetInputs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a26adee89d1055ab312823a233338c163>`() const;
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`GetOutputs<doxid-class_inference_engine_1_1_i_infer_request_internal_1acd330f10bb6539598c8d70832ebde7b9>`() const;
	
		virtual void :ref:`setModelInputsOutputs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a885d3bddecdaa0145adbebb6ad4ced1d>`(
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& inputs,
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& outputs
			);

.. _details-class_inference_engine_1_1_async_infer_request_thread_safe_default:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Base class with default implementation of asynchronous multi staged inference request. To customize pipeline stages derived class should change the content of :ref:`AsyncInferRequestThreadSafeDefault::_pipeline <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ace49df30feb600773ef07fb080380ec6>` member container. It consists of pairs of tasks and executors which will run the task. The class is recommended to be used by plugins as a base class for asynchronous inference request implementation.

To synchronize derived context with stages derived class should call :ref:`AsyncInferRequestThreadSafeDefault::StopAndWait() <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ad09f77f1467a13083e5f1a0eba1948b6>` function in destructor.

Here is an example of asynchronous inference request implementation for some accelerator device. It uses 5 different executors to run different stages of a synchronous inference request.



.. ref-code-block:: cpp

	// Inherits from AsyncInferRequestThreadSafeDefault
	class AcceleratorAsyncInferRequest : public :ref:`AsyncInferRequestThreadSafeDefault <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a4de1e75c94a322839a0aa48d41b34003>` {
	    // Store the pointer to the synchronous request and five executors
	    AcceleratorAsyncInferRequest(const AcceleratorSyncRequest::Ptr& syncRequest,
	                                 const :ref:`ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& preprocessExecutor,
	                                 const :ref:`ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& writeToDeviceExecutor,
	                                 const :ref:`ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& runOnDeviceExecutor,
	                                 const :ref:`ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& readFromDeviceExecutor,
	                                 const :ref:`ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& postProcessExecutor) :
	    :ref:`AsyncInferRequestThreadSafeDefault <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a4de1e75c94a322839a0aa48d41b34003>`(syncRequest, nullptr, nullptr),
	    _accSyncRequest{syncRequest},
	    _preprocessExecutor{preprocessExecutor},
	    _writeToDeviceExecutor{writeToDeviceExecutor},
	    _runOnDeviceExecutor{runOnDeviceExecutor},
	    _readFromDeviceExecutor{readFromDeviceExecutor},
	    _postProcessExecutor{postProcessExecutor}
	    {
	        // Five pipeline stages of synchronous infer request are run by different executors
	        :ref:`_pipeline <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ace49df30feb600773ef07fb080380ec6>` = {
	            { _preprocessExecutor , [this] {
	                _accSyncRequest->preprocess();
	            }},
	            { _writeToDeviceExecutor , [this] {
	                _accSyncRequest->write_to_device();
	            }},
	            { _runOnDeviceExecutor , [this] {
	                _accSyncRequest->run_on_device();
	            }},
	            { _readFromDeviceExecutor , [this] {
	                _accSyncRequest->read_from_device();
	            }},
	            { _postProcessExecutor , [this] {
	                _accSyncRequest->post_process();
	            }},
	        };
	    }
	
	    // As all stages use _accSyncRequest member we should wait for all stages tasks before the destructor destroy this member.
	    ~AcceleratorAsyncInferRequest() {
	        :ref:`StopAndWait <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ad09f77f1467a13083e5f1a0eba1948b6>`();
	    }
	
	    AcceleratorSyncRequest::Ptr _accSyncRequest;
	    :ref:`ITaskExecutor::Ptr <doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>` _preprocessExecutor, _writeToDeviceExecutor, _runOnDeviceExecutor, _readFromDeviceExecutor, _postProcessExecutor;
	};

Typedefs
--------

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a39aef32e4145a9a755a2df1ca9c09bae:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<AsyncInferRequestThreadSafeDefault> Ptr

A shared pointer to :ref:`AsyncInferRequestThreadSafeDefault <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default>`.

Construction
------------

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a4de1e75c94a322839a0aa48d41b34003:
.. index:: pair: function; AsyncInferRequestThreadSafeDefault

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	AsyncInferRequestThreadSafeDefault(
		const :ref:`IInferRequestInternal::Ptr<doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>`& request,
		const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& taskExecutor,
		const :ref:`ITaskExecutor::Ptr<doxid-class_inference_engine_1_1_i_task_executor_1a8ba60f739a36331eb8ed3492ffc55eb5>`& callbackExecutor
		)

Wraps a :ref:`IInferRequestInternal::Ptr <doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>` implementation and constructs a :ref:`AsyncInferRequestThreadSafeDefault::_pipeline <doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ace49df30feb600773ef07fb080380ec6>` where ``taskExecutor`` is used to run :ref:`IInferRequestInternal::Infer <doxid-class_inference_engine_1_1_i_infer_request_internal_1afb61e1de4ffb9927431085a91a40f352>` asynchronously.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- request

		- The synchronous request

	*
		- taskExecutor

		- The task executor

	*
		- callbackExecutor

		- The callback executor

Methods
-------

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a146ee9027a2d2c44472e71efc429677f:
.. index:: pair: function; Wait

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Wait(int64_t millis_timeout)

Waits for completion of all pipeline stages If the pipeline raises an exception it will be rethrown here.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- millis_timeout

		- A timeout is ``ms`` to wait or special enum value of :ref:`InferRequest::WaitMode <doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45a>`



.. rubric:: Returns:

A status code

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a93620dd73da915b3a2d53158ef722956:
.. index:: pair: function; StartAsync

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void StartAsync()

Start inference of specified input(s) in asynchronous mode.

The method returns immediately. Inference starts also immediately.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a3b98f918a8fb6180ea3f167f2137bc32:
.. index:: pair: function; Infer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Infer()

Infers specified input(s) in synchronous mode.

blocks all method of :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` while request is ongoing (running or waiting in queue)

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a16c0837c4f6f6a4bedc5063a37950337:
.. index:: pair: function; GetPerformanceCounts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`> GetPerformanceCounts() const

Queries performance measures per layer to get feedback of what is the most time consuming layer. Note: not all plugins may provide meaningful data.



.. rubric:: Returns:

- a map of layer names to profiling information for that layer.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a32610548fd783ff2835875e1df815868:
.. index:: pair: function; SetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetBlob(const std::string& name, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data)

Set input/output data to infer.

Memory allocation doesn't happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - a name of input or output blob.

	*
		- data

		- - a reference to input or output blob. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the network input precision and size.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1aa4d141581250971ada97b506943e55b4:
.. index:: pair: function; SetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetBlob(
		const std::string& name,
		const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info
		)

Sets pre-process for input data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input blob.

	*
		- data

		- - a reference to input or output blob. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the network input precision and size.

	*
		- info

		- Preprocess info for blob.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a3595ab110716a90c006b293cec7ba86c:
.. index:: pair: function; SetBlobs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetBlobs(
		const std::string& name,
		const std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& blobs
		)

Set batch of input data to infer. Default implementation performs basic validation and checks that all tensors are not remote. Plugin-specific implementations may override this behavior to handle remote tensors case. If plugin expects only memory blobs (not remote blobs), consider to override only SetBlobsImpl and reuse basic existing implementation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - an operation name of input or output blob.

	*
		- blobs

		- - input blobs. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the model's input precision and size.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a41da62beae65156a719d1150bebd729a:
.. index:: pair: function; GetBlobs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`BatchedBlob::Ptr<doxid-class_inference_engine_1_1_batched_blob_1ac66bc6bfae9ffc4be2de9c1d2f9e4208>` GetBlobs(const std::string& name)

Get input/output data to infer.

Memory allocation doesn't happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - a name of input or output blob.



.. rubric:: Returns:

data - a reference to input batched blob.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a5b34292297524421d6756222178856a6:
.. index:: pair: function; GetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` GetBlob(const std::string& name)

Get input/output data to infer.

Memory allocation doesn't happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - a name of input or output blob.

	*
		- data

		- - a reference to input or output blob. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the network input precision and size.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ad5ea95b5687b3b5443c77b08e8a53298:
.. index:: pair: function; GetPreProcess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& GetPreProcess(const std::string& name) const

Gets pre-process for input data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input blob.

	*
		- info

		- pointer to a pointer to :ref:`PreProcessInfo <doxid-class_inference_engine_1_1_pre_process_info>` structure

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a46c22dbc3e654a701e1b426190716e5d:
.. index:: pair: function; SetBatch

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetBatch(int batch)

Sets new batch size when dynamic batching is enabled in executable network that created this request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- batch

		- - new batch size to be used by all the following inference calls for this request.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a4c4f1ad53d5fe14a4f3f5e32e08c468a:
.. index:: pair: function; SetCallback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetCallback(:ref:`Callback<doxid-class_inference_engine_1_1_i_infer_request_internal_1a705346c27474676ee28370ecc0cc99e9>` callback)

Set callback function which will be called on success or failure of asynchronous request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- callback

		- - function to be called with the following description:

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1ac90c7ad04aef96be77d1c11556867483:
.. index:: pair: function; QueryState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::shared_ptr<:ref:`InferenceEngine::IVariableStateInternal<doxid-class_inference_engine_1_1_i_variable_state_internal>`>> QueryState()

Queries memory states.



.. rubric:: Returns:

Returns memory states

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a3a5904da5a3deb12ce8890964bb68fe8:
.. index:: pair: function; Cancel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Cancel()

Cancel current inference request execution.

.. _doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default_1a9183e86d3516539bd11b72200518e264:
.. index:: pair: function; setModelInputsOutputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setModelInputsOutputs(
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& inputs,
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& outputs
		)

Sets inputs/outputs from :ref:`ov::Model <doxid-classov_1_1_model>`.


