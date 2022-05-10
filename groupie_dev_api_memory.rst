.. index:: pair: group; Blob creation and memory utilities
.. _doxid-group__ie__dev__api__memory:

Blob creation and memory utilities
==================================



Overview
~~~~~~~~

An extension for public :ref:`Blob <doxid-class_inference_engine_1_1_blob>` API allowing to create blobs in uniform manner. :ref:`More...<details-group__ie__dev__api__memory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	void :ref:`InferenceEngine::blob_copy<doxid-group__ie__dev__api__memory_1ga06433bc8b79745acf299bd81a2ef203a>`(:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` src, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` dst);
	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1gaadd202fa37fcc6b9d70730a234dd4462>`(const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1ga10da7f895f6cd2913584bde98b086efb>`(
		const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		void \* ptr
		);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1ga4abc8b57f26279d43b011a1a854f5409>`(
		const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		const std::shared_ptr<:ref:`InferenceEngine::IAllocator<doxid-class_inference_engine_1_1_i_allocator>`>& alloc
		);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_plain_blob<doxid-group__ie__dev__api__memory_1ga1129ba1b599e4c0c8c781332bd67b681>`(
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` prec,
		const :ref:`InferenceEngine::SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>` dims
		);

	template <class... Args>
	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1ga8f4ac3993c12237c05c69d374d6bc724>`(
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` precision,
		Args&&... args
		);

	template <typename T>
	void :ref:`CopyVectorToBlob<doxid-group__ie__dev__api__memory_1gae5d15938c3ed40428c2611eed62ed5f9>`(
		const :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` outputBlob,
		const std::vector<T>& inputVector
		);

	int :ref:`ie_memcpy<doxid-group__ie__dev__api__memory_1gabe0c99cd9de11e89f0bdebc3023e6083>`(void \* dest, size_t destsz, void const \* src, size_t count);

.. _details-group__ie__dev__api__memory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An extension for public :ref:`Blob <doxid-class_inference_engine_1_1_blob>` API allowing to create blobs in uniform manner.

Global Functions
----------------

.. _doxid-group__ie__dev__api__memory_1ga06433bc8b79745acf299bd81a2ef203a:
.. index:: pair: function; blob_copy

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void InferenceEngine::blob_copy(:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` src, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` dst)

Copies data with taking into account layout and precision params.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- src

		- The source :ref:`Blob::Ptr <doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`

	*
		- dst

		- The destination :ref:`Blob::Ptr <doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`

.. _doxid-group__ie__dev__api__memory_1gaadd202fa37fcc6b9d70730a234dd4462:
.. index:: pair: function; make_blob_with_precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_blob_with_precision(const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc)

Creates Blob::Ptr with precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- The TensorDesc object



.. rubric:: Returns:

A Blob::Ptr pointer

.. _doxid-group__ie__dev__api__memory_1ga10da7f895f6cd2913584bde98b086efb:
.. index:: pair: function; make_blob_with_precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_blob_with_precision(
		const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		void \* ptr
		)

Makes a blob with precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- The TensorDesc object

	*
		- ptr

		- The pointer to a raw memory



.. rubric:: Returns:

A Blob::Ptr pointer

.. _doxid-group__ie__dev__api__memory_1ga4abc8b57f26279d43b011a1a854f5409:
.. index:: pair: function; make_blob_with_precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_blob_with_precision(
		const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		const std::shared_ptr<:ref:`InferenceEngine::IAllocator<doxid-class_inference_engine_1_1_i_allocator>`>& alloc
		)

Makes a blob with precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- The description

	*
		- alloc

		- The IAllocator object



.. rubric:: Returns:

A Blob::Ptr pointer

.. _doxid-group__ie__dev__api__memory_1ga1129ba1b599e4c0c8c781332bd67b681:
.. index:: pair: function; make_plain_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_plain_blob(
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` prec,
		const :ref:`InferenceEngine::SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>` dims
		)

Creates a plain Blob::Ptr.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prec

		- The Precision value

	*
		- dims

		- The dims



.. rubric:: Returns:

A Blob::Ptr pointer

.. _doxid-group__ie__dev__api__memory_1ga8f4ac3993c12237c05c69d374d6bc724:
.. index:: pair: function; make_blob_with_precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class... Args>
	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_blob_with_precision(
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` precision,
		Args&&... args
		)

Creates Blob::Ptr with precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- precision

		- The precision

	*
		- args

		- The arguments

	*
		- Args

		- Variadic template arguments



.. rubric:: Returns:

A Blob::Ptr pointer

.. _doxid-group__ie__dev__api__memory_1gae5d15938c3ed40428c2611eed62ed5f9:
.. index:: pair: function; CopyVectorToBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void CopyVectorToBlob(
		const :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` outputBlob,
		const std::vector<T>& inputVector
		)

Copy data from std::vector to Blob.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type of data in std::vector

	*
		- outputBlob

		- An output blob to copy to

	*
		- inputVector

		- An input std::vector to copy from

.. _doxid-group__ie__dev__api__memory_1gabe0c99cd9de11e89f0bdebc3023e6083:
.. index:: pair: function; ie_memcpy

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int ie_memcpy(void \* dest, size_t destsz, void const \* src, size_t count)

Copies bytes between buffers with security enhancements Copies count bytes from src to dest. If the source and destination overlap, the behavior is undefined.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dest

		- A Pointer to the object to copy to

	*
		- destsz

		- A max number of bytes to modify in the destination (typically the size of the destination object)

	*
		- src

		- A pointer to the object to copy from

	*
		- count

		- A number of bytes to copy



.. rubric:: Returns:

zero on success and non-zero value on error.

