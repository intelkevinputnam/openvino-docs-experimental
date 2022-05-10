.. index:: pair: interface; InferenceEngine::IInferRequestInternal
.. _doxid-class_inference_engine_1_1_i_infer_request_internal:

interface InferenceEngine::IInferRequestInternal
================================================



Overview
~~~~~~~~

An internal API of synchronous inference request to be implemented by plugin, which is used in InferRequestBase forwarding mechanism. :ref:`More...<details-class_inference_engine_1_1_i_infer_request_internal>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iinfer_request_internal.hpp>
	
	template IInferRequestInternal: public std::enable_shared_from_this< IInferRequestInternal >
	{
		// typedefs
	
		typedef std::shared_ptr<IInferRequestInternal> :ref:`Ptr<doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558>`;
		typedef std::function<void(std::exception_ptr)> :ref:`Callback<doxid-class_inference_engine_1_1_i_infer_request_internal_1a705346c27474676ee28370ecc0cc99e9>`;

		// construction
	
		:target:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal_1aa40da5188854ebad98fe8d6a82c11836>`();
	
		:ref:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal_1ae16f11221cf9e94a80b8a9382f153ce1>`(
			const :ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& networkInputs,
			const :ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& networkOutputs
			);
	
		:ref:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal_1a5173ff0e6b01f0cf580bb694df646119>`(
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& networkInputs,
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& networkOutputs
			);

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
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :target:`GetInputs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a26adee89d1055ab312823a233338c163>`() const;
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :target:`GetOutputs<doxid-class_inference_engine_1_1_i_infer_request_internal_1acd330f10bb6539598c8d70832ebde7b9>`() const;
	
		virtual void :ref:`setModelInputsOutputs<doxid-class_inference_engine_1_1_i_infer_request_internal_1a885d3bddecdaa0145adbebb6ad4ced1d>`(
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& inputs,
			const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& outputs
			);

	protected:
	};

	// direct descendants

	class :ref:`AsyncInferRequestThreadSafeDefault<doxid-class_inference_engine_1_1_async_infer_request_thread_safe_default>`;
.. _details-class_inference_engine_1_1_i_infer_request_internal:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An internal API of synchronous inference request to be implemented by plugin, which is used in InferRequestBase forwarding mechanism.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a50c614e7a30e1e8ee58e984f210a1558:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IInferRequestInternal> Ptr

A shared pointer to a :ref:`IInferRequestInternal <doxid-class_inference_engine_1_1_i_infer_request_internal>` interface.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a705346c27474676ee28370ecc0cc99e9:
.. index:: pair: typedef; Callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<void(std::exception_ptr)> Callback

Alias for callback type.

Construction
------------

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1ae16f11221cf9e94a80b8a9382f153ce1:
.. index:: pair: function; IInferRequestInternal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	IInferRequestInternal(
		const :ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& networkInputs,
		const :ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& networkOutputs
		)

Constructs a new instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkInputs

		- The network inputs info

	*
		- networkOutputs

		- The network outputs data

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a5173ff0e6b01f0cf580bb694df646119:
.. index:: pair: function; IInferRequestInternal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	IInferRequestInternal(
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& networkInputs,
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& networkOutputs
		)

Constructs a new instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- The network inputs

	*
		- outputs

		- The network outputs

Methods
-------

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1afb61e1de4ffb9927431085a91a40f352:
.. index:: pair: function; Infer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Infer()

Infers specified input(s) in synchronous mode.

blocks all method of :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` while request is ongoing (running or waiting in queue)

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a0ff052d969d599023769a8f5f3a75a56:
.. index:: pair: function; InferImpl

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void InferImpl()

The minimal infer function to be implemented by plugins. It infers specified input(s) in synchronous mode.

* This method is used in :ref:`IInferRequestInternal::Infer <doxid-class_inference_engine_1_1_i_infer_request_internal_1afb61e1de4ffb9927431085a91a40f352>`, which calls the common code first and after uses this plugin dependent implementation.

* Blocks all method of :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` while request is ongoing (running or waiting in queue)

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a23c9e992c9c4c94348bfc44f12e65148:
.. index:: pair: function; Cancel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Cancel()

Cancel current inference request execution.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a2eefb67a9766a29e032dc57bbf26d592:
.. index:: pair: function; GetPerformanceCounts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`> GetPerformanceCounts() const

Queries performance measures per layer to get feedback of what is the most time consuming layer. Note: not all plugins may provide meaningful data.



.. rubric:: Returns:

- a map of layer names to profiling information for that layer.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1aaf6f8482fd4e8220edb8cb08558a4d6c:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a0f1bb1a172ed84212ac1ead1ea131cd6:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a55ffc43c997b9e2034048523724a1a9a:
.. index:: pair: function; SetBlobsImpl

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetBlobsImpl(
		const std::string& name,
		const :ref:`BatchedBlob::Ptr<doxid-class_inference_engine_1_1_batched_blob_1ac66bc6bfae9ffc4be2de9c1d2f9e4208>`& batched_blob
		)

Set batch of input data to infer. Default implementation throws "Not implemented" exception To support 'set_input_tensors'/'set_tensors' plugin-specific implementations shall:

* Inside SetBlobsImpl: update 'InferenceEngine::IInferRequestInternal::batched_inputs' map

* Inside 'SetBlob': erase appropriate ' :ref:`InferenceEngine::IInferRequestInternal::_batched_inputs <doxid-class_inference_engine_1_1_i_infer_request_internal_1a576a7411bac4b411ded6a748344f2045>` [name]' item

* Inside 'InferImpl': call 'convertBatchedInputBlobs' on the beginning to convert many user blobs into single one

* If needed, override 'convertBatchedInputBlob' to perform custom concatenation and data copy to input blob



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - an operation name of input or output blob.

	*
		- batched_blob

		- - input blobs combined in batched blob. Called only if number of blobs > 1 precision and size.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1ad15f46c840f339ee2dd5e827ad003166:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a5521c5aca27d7493a5f2ee64d80beeb3:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a7e7269ff954409b76f35f7c910bbd1a3:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a0e598a7f365c30131645efa621c06ef3:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a5c2bd4827dd9f2852cd7d9b5c45e4ed2:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1adba24bc7f20b0f104ae4f8015b39ad44:
.. index:: pair: function; QueryState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::shared_ptr<:ref:`IVariableStateInternal<doxid-class_inference_engine_1_1_i_variable_state_internal>`>> QueryState()

Queries memory states.



.. rubric:: Returns:

Returns memory states

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a9386941427f51f918d0b385398c576c2:
.. index:: pair: function; StartAsync

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void StartAsync()

Start inference of specified input(s) in asynchronous mode.

The method returns immediately. Inference starts also immediately.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a5d69abeffffb707beb1c1cd65630a03b:
.. index:: pair: function; StartAsyncImpl

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void StartAsyncImpl()

The minimal asynchronous inference function to be implemented by plugins. It starts inference of specified input(s) in asynchronous mode.

* The methos is used in AsyncInferRequestInternal::StartAsync which performs common steps first and calls plugin dependent implementation of this method after.

* It returns immediately. Inference starts also immediately.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a313dae76fabb6d73014129bf548291f0:
.. index:: pair: function; Wait

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Wait(int64_t millis_timeout)

Waits for the result to become available. Blocks until specified millis_timeout has elapsed or the result becomes available, whichever comes first.

There are special cases when millis_timeout is equal some value of WaitMode enum:

* STATUS_ONLY - immediately returns request status (InferRequest::StatusCode). It doesn't block or interrupt current thread.

* RESULT_READY - waits until inference result becomes available



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- millis_timeout

		- - maximum duration in milliseconds to block for



.. rubric:: Returns:

A status code

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1adb5b5d5bfc3fa74546ea2c85ff88fab8:
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

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a175d83da2b71b5c14f01fc242ec09e12:
.. index:: pair: function; checkBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void checkBlob(
		const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& blob,
		const std::string& name,
		bool isInput,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& refDims = {}
		) const

Check that ``blob`` is valid. Throws an exception if it's not.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blob

		- The blob to check

	*
		- name

		- The name of input or output depending of if the ``blob`` is input or output

	*
		- isInput

		- Indicates if ``is`` input

	*
		- refDims

		- The reference dims, empty if not specified

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a19870e5b688afc41fd83c9c71841643c:
.. index:: pair: function; checkBlobs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void checkBlobs()

Check that all of the blobs is valid. Throws an exception if it's not.

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a9ad11a9ae33f3cf06318c804d1ccb73c:
.. index:: pair: function; setPointerToExecutableNetworkInternal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setPointerToExecutableNetworkInternal(const std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`>& exeNetwork)

Sets the pointer to executable network internal.

Needed to correctly handle ownership between objects.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- exeNetwork

		- The executable network

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a2176ee53c08047041a69dd9c11427198:
.. index:: pair: function; getPointerToExecutableNetworkInternal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> getPointerToExecutableNetworkInternal() const

Returns the pointer to executable network internal.



.. rubric:: Returns:

The executable network

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1aa64164e3f73f98153c1bad633b2cbb56:
.. index:: pair: function; GetUserData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void \* GetUserData()

Gets the pointer to userData.



.. rubric:: Returns:

Pointer to user data

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1ab21acbb31b2311fd97e6b5f5a07538e6:
.. index:: pair: function; SetUserData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetUserData(void \* userData)

Sets the pointer to userData.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Pointer

		- to user data

.. _doxid-class_inference_engine_1_1_i_infer_request_internal_1a885d3bddecdaa0145adbebb6ad4ced1d:
.. index:: pair: function; setModelInputsOutputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setModelInputsOutputs(
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& inputs,
		const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& outputs
		)

Sets inputs/outputs from :ref:`ov::Model <doxid-classov_1_1_model>`.


