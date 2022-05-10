.. index:: pair: class; InferenceEngine::IInferRequest
.. _doxid-class_inference_engine_1_1_i_infer_request:

class InferenceEngine::IInferRequest
====================================

.. toctree::
	:hidden:

	WaitMode <enumInferenceEngine_1_1IInferRequest_1_1WaitMode.rst>

Overview
~~~~~~~~

This is an interface of asynchronous infer request. :ref:`More...<details-class_inference_engine_1_1_i_infer_request>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iinfer_request.hpp>
	
	class IInferRequest: public std::enable_shared_from_this< IInferRequest >
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<IInferRequest> :ref:`Ptr<doxid-class_inference_engine_1_1_i_infer_request_1a3a97a4462a185eed9e86c1f0f0261ab3>`;
		typedef std::weak_ptr<IInferRequest> :ref:`WeakPtr<doxid-class_inference_engine_1_1_i_infer_request_1a14e179aa2e72142202dea6d45a9cf8be>`;
	
		typedef void(\* :ref:`CompletionCallback<doxid-class_inference_engine_1_1_i_infer_request_1a2a47e12b5e922df747d90a126de4ed78>`)(
			InferenceEngine::IInferRequest::Ptr context,
			InferenceEngine::StatusCode code
			);

		// enums
	
		enum :ref:`WaitMode<doxid-class_inference_engine_1_1_i_infer_request_1a5f403eaa522c38611d152399b616a848>`;

		// methods
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`SetBlob<doxid-class_inference_engine_1_1_i_infer_request_1a3f5656de410fada90478d3c89db085e1>`(
			const char \* name,
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetBlob<doxid-class_inference_engine_1_1_i_infer_request_1af885a8b36fa184ec403f2b7790a26f25>`(
			const char \* name,
			:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`SetBlob<doxid-class_inference_engine_1_1_i_infer_request_1aa4652872ae24daa5c2f3fb312b6297c5>`(
			const char \* name,
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetPreProcess<doxid-class_inference_engine_1_1_i_infer_request_1a6c21884f7259c1a32deb3cc1f53b3c3e>`(
			const char \* name,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>` \*\* info,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Infer<doxid-class_inference_engine_1_1_i_infer_request_1a797f06ce79f87c5ff7091a2570a44e0c>`(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Cancel<doxid-class_inference_engine_1_1_i_infer_request_1ae6e8c89c7a4e2bbb4c7bab48b03342fc>`(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetPerformanceCounts<doxid-class_inference_engine_1_1_i_infer_request_1aaf9fb9249d3a1697e511b6a97f3beeb9>`(
			std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`>& perfMap,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`InferenceEngine::StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Wait<doxid-class_inference_engine_1_1_i_infer_request_1a35459d31f6c739de6318d5b4b291a97d>`(
			int64_t millis_timeout,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`StartAsync<doxid-class_inference_engine_1_1_i_infer_request_1ada6ad3b909f96b4f760bfdb13e770a96>`(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`SetCompletionCallback<doxid-class_inference_engine_1_1_i_infer_request_1a8ee2d284f122e424e6e4da24db07b199>`(:ref:`CompletionCallback<doxid-class_inference_engine_1_1_i_infer_request_1a2a47e12b5e922df747d90a126de4ed78>` callback) = 0;
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetUserData<doxid-class_inference_engine_1_1_i_infer_request_1a0ee74b5a44ae3020f323bdc97ce325cd>`(void \*\* data, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`SetUserData<doxid-class_inference_engine_1_1_i_infer_request_1a6e2acc4da191a169a99024209a11db37>`(void \* data, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
	
		virtual :ref:`InferenceEngine::StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`SetBatch<doxid-class_inference_engine_1_1_i_infer_request_1ab4ff47c62921b6ce16587f40b983896e>`(
			int batch_size,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;

	protected:
	};
.. _details-class_inference_engine_1_1_i_infer_request:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is an interface of asynchronous infer request.

Deprecated Use :ref:`InferenceEngine::InferRequest <doxid-class_inference_engine_1_1_infer_request>` C++ wrapper

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_infer_request_1a3a97a4462a185eed9e86c1f0f0261ab3:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IInferRequest> Ptr

A shared pointer to the :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` object.

.. _doxid-class_inference_engine_1_1_i_infer_request_1a14e179aa2e72142202dea6d45a9cf8be:
.. index:: pair: typedef; WeakPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::weak_ptr<IInferRequest> WeakPtr

A smart pointer to the :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` object.

.. _doxid-class_inference_engine_1_1_i_infer_request_1a2a47e12b5e922df747d90a126de4ed78:
.. index:: pair: typedef; CompletionCallback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef void(\* CompletionCallback)(
		InferenceEngine::IInferRequest::Ptr context,
		InferenceEngine::StatusCode code
		)

Completion callback definition as pointer to a function.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- context

		- Pointer to request for providing context inside callback

	*
		- code

		- Completion result status: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

Methods
-------

.. _doxid-class_inference_engine_1_1_i_infer_request_1a3f5656de410fada90478d3c89db085e1:
.. index:: pair: function; SetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` SetBlob(
		const char \* name,
		const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

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

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1af885a8b36fa184ec403f2b7790a26f25:
.. index:: pair: function; GetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetBlob(
		const char \* name,
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Gets input/output data for inference.

Memory allocation does not happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input or output blob.

	*
		- data

		- Reference to input or output blob. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must match the network input precision and size.

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1aa4652872ae24daa5c2f3fb312b6297c5:
.. index:: pair: function; SetBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` SetBlob(
		const char \* name,
		const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& data,
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Sets pre-process for input data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of input blob.

	*
		- data

		- Reference to input or output blob. The type of :ref:`Blob <doxid-class_inference_engine_1_1_blob>` must match the network input precision and size.

	*
		- info

		- Preprocess info for blob.

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: OK (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1a6c21884f7259c1a32deb3cc1f53b3c3e:
.. index:: pair: function; GetPreProcess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetPreProcess(
		const char \* name,
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>` \*\* info,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

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

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: OK (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1a797f06ce79f87c5ff7091a2570a44e0c:
.. index:: pair: function; Infer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Infer(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Infers specified input(s) in synchronous mode.

blocks all methods of :ref:`IInferRequest <doxid-class_inference_engine_1_1_i_infer_request>` while request is ongoing (running or waiting in queue)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1ae6e8c89c7a4e2bbb4c7bab48b03342fc:
.. index:: pair: function; Cancel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Cancel(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Cancels current async inference request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1aaf9fb9249d3a1697e511b6a97f3beeb9:
.. index:: pair: function; GetPerformanceCounts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetPerformanceCounts(
		std::map<std::string, :ref:`InferenceEngineProfileInfo<doxid-struct_inference_engine_1_1_inference_engine_profile_info>`>& perfMap,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Queries performance measures per layer to get feedback of what is the most time consuming layer.

not all plugins provide meaningful data



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- perfMap

		- Map of layer names to profiling information for that layer

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1a35459d31f6c739de6318d5b4b291a97d:
.. index:: pair: function; Wait

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`InferenceEngine::StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Wait(
		int64_t millis_timeout,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

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

	*
		- resp

		- Optional: a pointer to an already allocated object to contain extra information of a failure (if occurred)



.. rubric:: Returns:

Enumeration of the resulted action: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1ada6ad3b909f96b4f760bfdb13e770a96:
.. index:: pair: function; StartAsync

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` StartAsync(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Starts inference of specified input(s) in asynchronous mode.

It returns immediately. Inference starts also immediately



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- resp

		- Optional: a pointer to an already allocated object to contain extra information of a failure (if occurred)



.. rubric:: Returns:

Enumeration of the resulted action: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1a8ee2d284f122e424e6e4da24db07b199:
.. index:: pair: function; SetCompletionCallback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` SetCompletionCallback(:ref:`CompletionCallback<doxid-class_inference_engine_1_1_i_infer_request_1a2a47e12b5e922df747d90a126de4ed78>` callback) = 0

Sets a callback function that will be called on success or failure of asynchronous request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- callback

		- A function to be called



.. rubric:: Returns:

Enumeration of the resulted action: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1a0ee74b5a44ae3020f323bdc97ce325cd:
.. index:: pair: function; GetUserData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetUserData(void \*\* data, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Gets arbitrary data for the request and stores a pointer to a pointer to the obtained data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- data

		- Pointer to a pointer to the gotten arbitrary data

	*
		- resp

		- Optional: a pointer to an already allocated object to contain extra information of a failure (if occurred)



.. rubric:: Returns:

Enumeration of the resulted action: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1a6e2acc4da191a169a99024209a11db37:
.. index:: pair: function; SetUserData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` SetUserData(void \* data, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Sets arbitrary data for the request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- data

		- Pointer to a pointer to arbitrary data to set

	*
		- resp

		- Optional: a pointer to an already allocated object to contain extra information of a failure (if occurred)



.. rubric:: Returns:

Enumeration of the resulted action: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_infer_request_1ab4ff47c62921b6ce16587f40b983896e:
.. index:: pair: function; SetBatch

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`InferenceEngine::StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` SetBatch(
		int batch_size,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Sets new batch size when dynamic batching is enabled in executable network that created this request.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- batch_size

		- new batch size to be used by all the following inference calls for this request.

	*
		- resp

		- Optional: a pointer to an already allocated object to contain extra information of a failure (if occurred)



.. rubric:: Returns:

Enumeration of the resulted action: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success


