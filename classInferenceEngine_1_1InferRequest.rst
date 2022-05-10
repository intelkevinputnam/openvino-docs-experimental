.. index:: pair: class; InferenceEngine::InferRequest
.. _doxid-class_inference_engine_1_1_infer_request:

class InferenceEngine::InferRequest
===================================

.. toctree::
	:hidden:

	WaitMode <enumInferenceEngine_1_1InferRequest_1_1WaitMode.rst>
	SetCallback <structInferenceEngine_1_1InferRequest_1_1SetCallback.rst>

Overview
~~~~~~~~

This is an interface of asynchronous infer request. :ref:`More...<details-class_inference_engine_1_1_infer_request>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_infer_request.hpp>
	
	class InferRequest
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<InferRequest> :ref:`Ptr<doxid-class_inference_engine_1_1_infer_request_1aa725364c5565a1cbe4d0e9245a4cb055>`;

		// enums
	
		enum :ref:`WaitMode<doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45a>`;

		// structs
	
		template <typename T>
		struct :ref:`SetCallback<doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback>`;
		template <>
		struct :ref:`SetCallback<IInferRequest::CompletionCallback><doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01_i_infer_request_1_1_completion_callback_01_4>`;
		template <>
		struct :ref:`SetCallback<std::function<void(InferRequest, StatusCode)>><doxid-struct_inference_engine_1_1_infer_request_1_1_set_callback_3_01std_1_1function_3_01void_07_inferd36a10d7c08edcd1bda12bce9578bb66>`;

		// construction
	
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request_1a47c1d4d15e66d7923e59551d70f8ca74>`();
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request_1a927f91204d9477f67433b60230464026>`(const InferRequest& other);
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request_1a212108576a6bf2952aff41244cc50f95>`(InferRequest&& other);

		// methods
	
		InferRequest& :ref:`operator =<doxid-class_inference_engine_1_1_infer_request_1a2720ae2b8a6b9eb08601a5f4bdb95182>` (const InferRequest& other);
		InferRequest& :ref:`operator =<doxid-class_inference_engine_1_1_infer_request_1acd5a742453fa744713bcb55db7040227>` (InferRequest&& other);
		void :ref:`SetBlob<doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`(const std::string& name, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data);
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`GetBlob<doxid-class_inference_engine_1_1_infer_request_1a9601a4cda3f309181af34feedf1b914c>`(const std::string& name);
	
		void :ref:`SetBlob<doxid-class_inference_engine_1_1_infer_request_1a21472d80ed86e65230d6d97f334c9da6>`(
			const std::string& name,
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info
			);
	
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& :ref:`GetPreProcess<doxid-class_inference_engine_1_1_infer_request_1a3bfb3002dc1374cc63b9b50b3b230521>`(const std::string& name) const;
		void :ref:`Infer<doxid-class_inference_engine_1_1_infer_request_1a3391ce30894abde730523e9ca9371ce8>`();
		void :ref:`Cancel<doxid-class_inference_engine_1_1_infer_request_1ad4b36d13349db2c9985e4174d7e10ce9>`();
		std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`> :ref:`GetPerformanceCounts<doxid-class_inference_engine_1_1_infer_request_1a1aa33a2377a38ecf708abf352079154d>`() const;
		void :ref:`SetInput<doxid-class_inference_engine_1_1_infer_request_1a1d84744a6b08a2ace4041ff81519c946>`(const :ref:`BlobMap<doxid-namespace_inference_engine_1ad1c63c694d34358a748f591ffa74a9d0>`& inputs);
		void :ref:`SetOutput<doxid-class_inference_engine_1_1_infer_request_1a8a0ea625862861f5fc71f4b6ab9ca587>`(const :ref:`BlobMap<doxid-namespace_inference_engine_1ad1c63c694d34358a748f591ffa74a9d0>`& results);
		void :ref:`SetBatch<doxid-class_inference_engine_1_1_infer_request_1a2f2e7ae0a8ae7dda6e7b4099eed9d183>`(const int batch);
		void :ref:`StartAsync<doxid-class_inference_engine_1_1_infer_request_1a405293e8423d82a5b45f642a3bef0d24>`();
		:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Wait<doxid-class_inference_engine_1_1_infer_request_1a7e54bb6699e0df0b88445be9eeb71948>`(int64_t millis_timeout = :ref:`RESULT_READY<doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45aaa71f7b3aaba799f92c75c52ac56897d8>`);
	
		template <typename F>
		void :ref:`SetCompletionCallback<doxid-class_inference_engine_1_1_infer_request_1a3d37c50e3762862f29af78d1b0e5a435>`(F callbackToSet);
	
		std::vector<:ref:`VariableState<doxid-class_inference_engine_1_1_variable_state>`> :ref:`QueryState<doxid-class_inference_engine_1_1_infer_request_1a15068890ee92c7c681dff99b25ce22ec>`();
		:ref:`operator std::shared_ptr< IInferRequest ><doxid-class_inference_engine_1_1_infer_request_1a78b8f13d6b648e4826a9cf4c4fb32f1f>` ();
		bool :ref:`operator !<doxid-class_inference_engine_1_1_infer_request_1a64d1c42b9e12a1af040ecf2b255f4222>` () const;
		:ref:`operator bool<doxid-class_inference_engine_1_1_infer_request_1ae09af4862c4db17651dad2a98afd557e>` () const;
		bool :ref:`operator !=<doxid-class_inference_engine_1_1_infer_request_1a2159a92894f4aa89501d08dd6d30dce6>` (const InferRequest&) const;
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_infer_request_1a9dda456c316adffee2f6213acb43b80d>` (const InferRequest&) const;
	};
.. _details-class_inference_engine_1_1_infer_request:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is an interface of asynchronous infer request.

Wraps :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` It can throw exceptions safely for the application, where it is properly handled.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_infer_request_1aa725364c5565a1cbe4d0e9245a4cb055:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<InferRequest> Ptr

A smart pointer to the :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_infer_request_1a47c1d4d15e66d7923e59551d70f8ca74:
.. index:: pair: function; InferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest()

Default constructor.

.. _doxid-class_inference_engine_1_1_infer_request_1a927f91204d9477f67433b60230464026:
.. index:: pair: function; InferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest(const InferRequest& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object

.. _doxid-class_inference_engine_1_1_infer_request_1a212108576a6bf2952aff41244cc50f95:
.. index:: pair: function; InferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest(InferRequest&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object

Methods
-------

.. _doxid-class_inference_engine_1_1_infer_request_1a2720ae2b8a6b9eb08601a5f4bdb95182:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest& operator = (const InferRequest& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-class_inference_engine_1_1_infer_request_1acd5a742453fa744713bcb55db7040227:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest& operator = (InferRequest&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653:
.. index:: pair: function; SetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetBlob(const std::string& name, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data)

Sets input/output data to infer.

Memory allocation does not happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input or output blob.

	*
		- data

		- Reference to input or output blob. The type of a blob must match the network input precision and size.

.. _doxid-class_inference_engine_1_1_infer_request_1a9601a4cda3f309181af34feedf1b914c:
.. index:: pair: function; GetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` GetBlob(const std::string& name)

Gets input/output data for inference.

Memory allocation does not happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- A name of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` to get



.. rubric:: Returns:

A shared pointer to a :ref:`Blob <doxid-class_inference_engine_1_1_blob>` with a name ``name``. If a blob is not found, an exception is thrown.

.. _doxid-class_inference_engine_1_1_infer_request_1a21472d80ed86e65230d6d97f334c9da6:
.. index:: pair: function; SetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetBlob(
		const std::string& name,
		const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info
		)

Sets blob with a pre-process information.

Returns an error in case if data blob is output



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input blob.

	*
		- data

		- A reference to input. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the network input precision and size.

	*
		- info

		- Preprocess info for blob.

.. _doxid-class_inference_engine_1_1_infer_request_1a3bfb3002dc1374cc63b9b50b3b230521:
.. index:: pair: function; GetPreProcess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& GetPreProcess(const std::string& name) const

Gets pre-process for input data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input blob.



.. rubric:: Returns:

pointer to pre-process info of blob with name

.. _doxid-class_inference_engine_1_1_infer_request_1a3391ce30894abde730523e9ca9371ce8:
.. index:: pair: function; Infer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void Infer()

Infers specified input(s) in synchronous mode.

blocks all methods of :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` while request is ongoing (running or waiting in queue)

.. _doxid-class_inference_engine_1_1_infer_request_1ad4b36d13349db2c9985e4174d7e10ce9:
.. index:: pair: function; Cancel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void Cancel()

Cancels inference request.

.. _doxid-class_inference_engine_1_1_infer_request_1a1aa33a2377a38ecf708abf352079154d:
.. index:: pair: function; GetPerformanceCounts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`> GetPerformanceCounts() const

Queries performance measures per layer to get feedback of what is the most time consuming layer.

not all plugins provide meaningful data



.. rubric:: Returns:

Map of layer names to profiling information for that layer

.. _doxid-class_inference_engine_1_1_infer_request_1a1d84744a6b08a2ace4041ff81519c946:
.. index:: pair: function; SetInput

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetInput(const :ref:`BlobMap<doxid-namespace_inference_engine_1ad1c63c694d34358a748f591ffa74a9d0>`& inputs)

Sets input data to infer.

Memory allocation doesn't happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- A reference to a map of input blobs accessed by input names. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the network input precision and size.

.. _doxid-class_inference_engine_1_1_infer_request_1a8a0ea625862861f5fc71f4b6ab9ca587:
.. index:: pair: function; SetOutput

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetOutput(const :ref:`BlobMap<doxid-namespace_inference_engine_1ad1c63c694d34358a748f591ffa74a9d0>`& results)

Sets data that will contain result of the inference.

Memory allocation doesn't happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- results

		- - a reference to a map of result blobs accessed by output names. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must correspond to the network output precision and size.

.. _doxid-class_inference_engine_1_1_infer_request_1a2f2e7ae0a8ae7dda6e7b4099eed9d183:
.. index:: pair: function; SetBatch

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetBatch(const int batch)

Sets new batch size when dynamic batching is enabled in executable network that created this request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- batch

		- new batch size to be used by all the following inference calls for this request.

.. _doxid-class_inference_engine_1_1_infer_request_1a405293e8423d82a5b45f642a3bef0d24:
.. index:: pair: function; StartAsync

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void StartAsync()

Start inference of specified input(s) in asynchronous mode.

It returns immediately. Inference starts also immediately.

.. _doxid-class_inference_engine_1_1_infer_request_1a7e54bb6699e0df0b88445be9eeb71948:
.. index:: pair: function; Wait

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Wait(int64_t millis_timeout = :ref:`RESULT_READY<doxid-class_inference_engine_1_1_infer_request_1ac52c77df62b93f2f40b47ea232fde45aaa71f7b3aaba799f92c75c52ac56897d8>`)

Waits for the result to become available. Blocks until specified millis_timeout has elapsed or the result becomes available, whichever comes first.

There are special cases when millis_timeout is equal some value of the WaitMode enum:

* STATUS_ONLY - immediately returns inference status (IInferRequest::RequestStatus). It does not block or interrupt current thread

* RESULT_READY - waits until inference result becomes available



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- millis_timeout

		- Maximum duration in milliseconds to block for



.. rubric:: Returns:

A status code of operation

.. _doxid-class_inference_engine_1_1_infer_request_1a3d37c50e3762862f29af78d1b0e5a435:
.. index:: pair: function; SetCompletionCallback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename F>
	void SetCompletionCallback(F callbackToSet)

Sets a callback function that will be called on success or failure of asynchronous request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- callbackToSet

		- callback object which will be called on when inference finish.

.. _doxid-class_inference_engine_1_1_infer_request_1a15068890ee92c7c681dff99b25ce22ec:
.. index:: pair: function; QueryState

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`VariableState<doxid-class_inference_engine_1_1_variable_state>`> QueryState()

Gets state control interface for given infer request.

State control essential for recurrent networks



.. rubric:: Returns:

A vector of Memory State objects

.. _doxid-class_inference_engine_1_1_infer_request_1a78b8f13d6b648e4826a9cf4c4fb32f1f:
.. index:: pair: function; operator std::shared_ptr< IInferRequest >

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator std::shared_ptr< IInferRequest > ()

:ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` pointer to be used directly in CreateInferRequest functions.



.. rubric:: Returns:

A shared pointer to :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` interface

.. _doxid-class_inference_engine_1_1_infer_request_1a64d1c42b9e12a1af040ecf2b255f4222:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Checks if current :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object is not initialized.



.. rubric:: Returns:

true if current :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object is not initialized, false - otherwise

.. _doxid-class_inference_engine_1_1_infer_request_1ae09af4862c4db17651dad2a98afd557e:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Checks if current :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object is initialized.



.. rubric:: Returns:

true if current :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object is initialized, false - otherwise

.. _doxid-class_inference_engine_1_1_infer_request_1a2159a92894f4aa89501d08dd6d30dce6:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const InferRequest&) const

Compares whether this request wraps the same impl underneath.



.. rubric:: Returns:

true if current :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object doesn't wrap the same impl as the operator's arg

.. _doxid-class_inference_engine_1_1_infer_request_1a9dda456c316adffee2f6213acb43b80d:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const InferRequest&) const

Compares whether this request wraps the same impl underneath.



.. rubric:: Returns:

true if current :ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object wraps the same impl as the operator's arg


