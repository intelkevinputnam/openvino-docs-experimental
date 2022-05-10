.. index:: pair: class; InferenceEngine::TBlob
.. _doxid-class_inference_engine_1_1_t_blob:

class InferenceEngine::TBlob
============================



Overview
~~~~~~~~

Represents real host memory allocated for a Tensor/Blob per C type. :ref:`More...<details-class_inference_engine_1_1_t_blob>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_blob.h>
	
	template <
		typename T,
		typename = std::enable_if<std::is_standard_layout<T>::value&& std::is_trivial<T>::value>
		>
	class TBlob: public :ref:`InferenceEngine::MemoryBlob<doxid-class_inference_engine_1_1_memory_blob>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<TBlob<T>> :ref:`Ptr<doxid-class_inference_engine_1_1_t_blob_1ae6e7f84f98e2fbb28204ac712237fabb>`;

		// construction
	
		:ref:`TBlob<doxid-class_inference_engine_1_1_t_blob_1a60ad3422771c2c4c79a07afecf12024a>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc);
		:ref:`TBlob<doxid-class_inference_engine_1_1_t_blob_1a8f896506b3571d808ca4c15b02971532>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc, T \* ptr, size_t data_size = 0);
		:ref:`TBlob<doxid-class_inference_engine_1_1_t_blob_1a3deab7611d156ac2004e1bf7b3cacefb>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc, const std::shared_ptr<:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>`>& alloc);
		:ref:`TBlob<doxid-class_inference_engine_1_1_t_blob_1ae8246ef1376103d4a002ddc3bccf5742>`(const TBlob<T>& blob);
		:ref:`TBlob<doxid-class_inference_engine_1_1_t_blob_1a237e2882d2885486864161d36f4284cf>`(TBlob<T>&& blob);

		// methods
	
		TBlob& :ref:`operator =<doxid-class_inference_engine_1_1_t_blob_1a050b4b25b2dff6b97b124d834d02d904>` (const TBlob& blob);
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<T> :ref:`data<doxid-class_inference_engine_1_1_t_blob_1ac90750dbeeb06ff2699e0d8ed8e800ed>`();
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T> :ref:`readOnly<doxid-class_inference_engine_1_1_t_blob_1a5ef3d0ddb36fe2aaeda3b3b3b568a15a>`() const;
		virtual void :ref:`allocate<doxid-class_inference_engine_1_1_t_blob_1a55e95d6fd89bf29e39376429467db0ed>`();
		virtual bool :ref:`deallocate<doxid-class_inference_engine_1_1_t_blob_1ab95a5e55215245df24e4857b13a516d7>`();
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> :ref:`rwmap<doxid-class_inference_engine_1_1_t_blob_1a5ff618c6c0576999d2a05572b4ae91a0>`();
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const void> :ref:`rmap<doxid-class_inference_engine_1_1_t_blob_1a66a2b29c2e42c2f7181baee072f60620>`() const;
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> :ref:`wmap<doxid-class_inference_engine_1_1_t_blob_1ac43d8f601532cece4a88f5b500d5a9db>`();
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`createROI<doxid-class_inference_engine_1_1_t_blob_1a495e1f1f4d50d8f50490620effb19a1c>`(const :ref:`ROI<doxid-struct_inference_engine_1_1_r_o_i>`& roi) const;
	
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`createROI<doxid-class_inference_engine_1_1_t_blob_1ae2a59463df9536e41f4f5c1a31a68504>`(
			const std::vector<std::size_t>& begin,
			const std::vector<std::size_t>& end
			) const;
	
		details::BlobIterator<T> :ref:`begin<doxid-class_inference_engine_1_1_t_blob_1a588f41c1af51c4fa48c4e7a0714886f1>`();
		details::BlobIterator<T> :ref:`end<doxid-class_inference_engine_1_1_t_blob_1a03c3c094dcf0765afedd12cb5156da95>`();
		details::BlobIterator<const T> :ref:`begin<doxid-class_inference_engine_1_1_t_blob_1adf6d6f90b068f0fbe8959b214471a30d>`() const;
		details::BlobIterator<const T> :ref:`end<doxid-class_inference_engine_1_1_t_blob_1a16dceb89e0b31f53b5d3ac2439295700>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Blob<doxid-class_inference_engine_1_1_blob>`> :ref:`Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`;
		typedef std::shared_ptr<const :ref:`Blob<doxid-class_inference_engine_1_1_blob>`> :ref:`CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`;
		typedef std::shared_ptr<:ref:`MemoryBlob<doxid-class_inference_engine_1_1_memory_blob>`> :ref:`Ptr<doxid-class_inference_engine_1_1_memory_blob_1a294bf7449b6181f29ac05636a5968e1d>`;
		typedef std::shared_ptr<const :ref:`MemoryBlob<doxid-class_inference_engine_1_1_memory_blob>`> :ref:`CPtr<doxid-class_inference_engine_1_1_memory_blob_1adae370cdc2fa2649928498f9e25dec9e>`;

		// methods
	
		static :ref:`Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`CreateFromData<doxid-class_inference_engine_1_1_blob_1ae81db862104a25e3fb41f57d94dd41a6>`(const :ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`& data);
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
			>
		bool :ref:`is<doxid-class_inference_engine_1_1_blob_1aa07152ba7c9910abab46a7e8e58323bc>`();
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
			>
		bool :ref:`is<doxid-class_inference_engine_1_1_blob_1a74f56a3007a5dbabd8acda5e11d9568c>`() const;
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
			>
		T \* :ref:`as<doxid-class_inference_engine_1_1_blob_1abc7e63536f5f3811ba2b01455ad06954>`();
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
			>
		const T \* :ref:`as<doxid-class_inference_engine_1_1_blob_1aa7f7eef35f32cf11c76f3db57bd555f6>`() const;
	
		virtual const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& :ref:`getTensorDesc<doxid-class_inference_engine_1_1_blob_1accdd939c62592f28a0ceb64cd60eb62e>`() const;
		virtual :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& :ref:`getTensorDesc<doxid-class_inference_engine_1_1_blob_1aaa14e36bf31d98a9c9db1054811201f0>`();
		virtual size_t :ref:`size<doxid-class_inference_engine_1_1_blob_1a2b5686fa129fdbe3d4ccc44210d911f7>`() const;
		virtual size_t :ref:`byteSize<doxid-class_inference_engine_1_1_blob_1a9f2049e262cea015e7640a82e4d70ccb>`() const;
		virtual size_t :ref:`element_size<doxid-class_inference_engine_1_1_blob_1a25690a7dd30e0c07abbf32f09c5f8735>`() const = 0;
		virtual void :ref:`allocate<doxid-class_inference_engine_1_1_blob_1a88866d4156b7936e2d60d7fff8c9f230>`() = 0;
		virtual bool :ref:`deallocate<doxid-class_inference_engine_1_1_blob_1af9ccc77bec5dbebd179291bbd88af881>`() = 0;
		void :ref:`setShape<doxid-class_inference_engine_1_1_blob_1abdce9a4dc4319da76b283ac68f9c0283>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims);
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`createROI<doxid-class_inference_engine_1_1_blob_1a81168f9425c1d7c5fdb6f52210213a39>`(const :ref:`ROI<doxid-struct_inference_engine_1_1_r_o_i>`& roi) const;
	
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`createROI<doxid-class_inference_engine_1_1_blob_1a39d758fa25f8268c32af77379b062fbb>`(
			const std::vector<std::size_t>& begin,
			const std::vector<std::size_t>& end
			) const;
	
		virtual const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& :ref:`getTensorDesc<doxid-class_inference_engine_1_1_memory_blob_1a359897a812bf64603a67e4fc92b71aae>`() const;
		virtual :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& :ref:`getTensorDesc<doxid-class_inference_engine_1_1_memory_blob_1ac86c87548512f03bebf72c47cde4cc65>`();
		virtual size_t :ref:`size<doxid-class_inference_engine_1_1_memory_blob_1a733d578f1a002e9f84b65229a61b05d6>`() const;
		virtual size_t :ref:`byteSize<doxid-class_inference_engine_1_1_memory_blob_1a4c1e80abfbca64b8c1d3d8918b7af084>`() const;
		virtual size_t :ref:`element_size<doxid-class_inference_engine_1_1_memory_blob_1a9b2f80180ea50adcbcab1cd68932209f>`() const;
		virtual void :ref:`allocate<doxid-class_inference_engine_1_1_memory_blob_1a6b8605e3863617c5985d21bc91837b8f>`() = 0;
		virtual bool :ref:`deallocate<doxid-class_inference_engine_1_1_memory_blob_1ad462f247d8dffc1e525f51899448a60c>`() = 0;
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> :ref:`rwmap<doxid-class_inference_engine_1_1_memory_blob_1a715863b45d88b97937e770d866bf1784>`() = 0;
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const void> :ref:`rmap<doxid-class_inference_engine_1_1_memory_blob_1a055940ba42eb270f348bedea9726cf12>`() const = 0;
		virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> :ref:`wmap<doxid-class_inference_engine_1_1_memory_blob_1ac5c6b1ecf54a69f98a06df6d05187a7f>`() = 0;

.. _details-class_inference_engine_1_1_t_blob:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents real host memory allocated for a Tensor/Blob per C type.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_t_blob_1ae6e7f84f98e2fbb28204ac712237fabb:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<TBlob<T>> Ptr

Smart Pointer to this :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_t_blob_1a60ad3422771c2c4c79a07afecf12024a:
.. index:: pair: function; TBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TBlob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc)

Creates a :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object with the specified dimensions and layout but does not allocate the memory.

Use the :ref:`allocate() <doxid-class_inference_engine_1_1_t_blob_1a55e95d6fd89bf29e39376429467db0ed>` method to allocate memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Tensor description

.. _doxid-class_inference_engine_1_1_t_blob_1a8f896506b3571d808ca4c15b02971532:
.. index:: pair: function; TBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TBlob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc, T \* ptr, size_t data_size = 0)

The constructor creates a :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object with the specified dimensions and layout on the pre-allocated memory.

The :ref:`allocate() <doxid-class_inference_engine_1_1_t_blob_1a55e95d6fd89bf29e39376429467db0ed>` call is not required.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Tensor description

	*
		- ptr

		- Pointer to the pre-allocated memory

	*
		- data_size

		- Length of the pre-allocated array. If not set, size is assumed equal to the dot product of dims.

.. _doxid-class_inference_engine_1_1_t_blob_1a3deab7611d156ac2004e1bf7b3cacefb:
.. index:: pair: function; TBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TBlob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc, const std::shared_ptr<:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>`>& alloc)

Creates a :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object with the specified dimensions, layout and custom memory allocator but does not allocate the memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Tensor description

	*
		- alloc

		- An allocator

.. _doxid-class_inference_engine_1_1_t_blob_1ae8246ef1376103d4a002ddc3bccf5742:
.. index:: pair: function; TBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TBlob(const TBlob<T>& blob)

The copy constructor data is reallocated and copied from the source to the target blob.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blob

		- Source blob

.. _doxid-class_inference_engine_1_1_t_blob_1a237e2882d2885486864161d36f4284cf:
.. index:: pair: function; TBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TBlob(TBlob<T>&& blob)

A move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blob

		- rvalue to make a move from

Methods
-------

.. _doxid-class_inference_engine_1_1_t_blob_1a050b4b25b2dff6b97b124d834d02d904:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TBlob& operator = (const TBlob& blob)

Copy operator for the :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blob

		- object reference to copy from



.. rubric:: Returns:

Newly copied object

.. _doxid-class_inference_engine_1_1_t_blob_1ac90750dbeeb06ff2699e0d8ed8e800ed:
.. index:: pair: function; data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<T> data()

Creates an new empty rvalue :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object.



.. rubric:: Returns:

rvalue for the empty locked object of type T

.. _doxid-class_inference_engine_1_1_t_blob_1a5ef3d0ddb36fe2aaeda3b3b3b568a15a:
.. index:: pair: function; readOnly

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T> readOnly() const

Creates a new empty rvalue read-only :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object.



.. rubric:: Returns:

rvalue for the empty locked const object of type T.

.. _doxid-class_inference_engine_1_1_t_blob_1a55e95d6fd89bf29e39376429467db0ed:
.. index:: pair: function; allocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void allocate()

Allocates memory to store the data.

Abstract method.

.. _doxid-class_inference_engine_1_1_t_blob_1ab95a5e55215245df24e4857b13a516d7:
.. index:: pair: function; deallocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool deallocate()

Releases previously allocated data.

Abstract method.



.. rubric:: Returns:

``True`` if deallocation happens successfully, ``false`` otherwise.

.. _doxid-class_inference_engine_1_1_t_blob_1a5ff618c6c0576999d2a05572b4ae91a0:
.. index:: pair: function; rwmap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> rwmap()

Gets read/write access to the memory in virtual space of the process. The function returns object which retains mapped memory. The memory been addressed in the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` in general case can be allocated on remote device. This function maps remote memory to the memory in the virtual process space and after destruction of the :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` will upload changed content to the accelerator.

To avoid extra copy of data, you can use :ref:`rmap() <doxid-class_inference_engine_1_1_t_blob_1a66a2b29c2e42c2f7181baee072f60620>` and :ref:`wmap() <doxid-class_inference_engine_1_1_t_blob_1ac43d8f601532cece4a88f5b500d5a9db>` functions.

In case of memory originally allocated on the host, this function returns :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` which will transparently refer to original memory address. No extra copy will happen

In general case, pointer received from that :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` becomes invalid just after destruction of :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` instance. Keep Locked memory alive while you need to address memory in the process on the host.

Abstract method.



.. rubric:: Returns:

A :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object

.. _doxid-class_inference_engine_1_1_t_blob_1a66a2b29c2e42c2f7181baee072f60620:
.. index:: pair: function; rmap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const void> rmap() const

Gets read only access to the memory in virtual space of the process. The function returns object which retains mapped memory.

The memory been addressed in the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` in general case can be allocated on remote device. This function copies remote memory to the memory in the virtual process space and after destruction of the :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` it will not upload host memory back, because it is expected that content is not changed.

To have an ability change content, you can use :ref:`rwmap() <doxid-class_inference_engine_1_1_t_blob_1a5ff618c6c0576999d2a05572b4ae91a0>` and :ref:`wmap() <doxid-class_inference_engine_1_1_t_blob_1ac43d8f601532cece4a88f5b500d5a9db>` functions.

In case of memory originally allocated on the host, this function returns :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` which will transparently refer to original memory address. No extra copy will happen

In general case, pointer received from that :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` becomes invalid just after destruction of :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` instance. Keep Locked memory alive while you need to address memory in the process on the host.

Abstract method.



.. rubric:: Returns:

A :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object

.. _doxid-class_inference_engine_1_1_t_blob_1ac43d8f601532cece4a88f5b500d5a9db:
.. index:: pair: function; wmap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> wmap()

Gets "write only direction" access to the memory in virtual space of the process. The function returns object which retains memory to be uploaded on device.

The memory been addressed in the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` in general case can be allocated on remote device. This function does not copy of the content from the device to the memory in the virtual process space, the content of the memory just after calling of this function is not specified. After destruction of the :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>`, content will be upload host memory. In the same time there is no abilities to restrict reading from the memory, you need to care of reading from memory got by :ref:`wmap() <doxid-class_inference_engine_1_1_t_blob_1ac43d8f601532cece4a88f5b500d5a9db>`, it might have sense in some cases like filling of content and before uploading to device

To access data stored in the blob, you can use :ref:`rwmap() <doxid-class_inference_engine_1_1_t_blob_1a5ff618c6c0576999d2a05572b4ae91a0>` and :ref:`rmap() <doxid-class_inference_engine_1_1_t_blob_1a66a2b29c2e42c2f7181baee072f60620>` functions.

In case of memory originally allocated on the host, this function returns :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` which will transparently refer to original memory address. No extra copy will happen

In general case, pointer received from that :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` becomes invalid just after destruction of :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` instance. Keep Locked memory alive while you need to address memory in the process on the host.

Abstract method.



.. rubric:: Returns:

A :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object

.. _doxid-class_inference_engine_1_1_t_blob_1a495e1f1f4d50d8f50490620effb19a1c:
.. index:: pair: function; createROI

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` createROI(const :ref:`ROI<doxid-struct_inference_engine_1_1_r_o_i>`& roi) const

Creates a blob describing given :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` object based on the current blob with memory sharing.

Note: default implementation throws "not implemented" exception.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- roi

		- A :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` object inside of the current blob.



.. rubric:: Returns:

A shared pointer to the newly created :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` blob.

.. _doxid-class_inference_engine_1_1_t_blob_1ae2a59463df9536e41f4f5c1a31a68504:
.. index:: pair: function; createROI

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` createROI(
		const std::vector<std::size_t>& begin,
		const std::vector<std::size_t>& end
		) const

Creates a blob describing given :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` object based on the current blob with memory sharing.

Note: default implementation may throws "not implemented" exception.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- begin

		- A :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` start coordinate

	*
		- end

		- A :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` end coordinate



.. rubric:: Returns:

A shared pointer to the newly created :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` blob.

.. _doxid-class_inference_engine_1_1_t_blob_1a588f41c1af51c4fa48c4e7a0714886f1:
.. index:: pair: function; begin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	details::BlobIterator<T> begin()

Gets BlobIterator for the data.

Enables a ranged loop support for the :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object.



.. rubric:: Returns:

BlobIterator object of type T

.. _doxid-class_inference_engine_1_1_t_blob_1a03c3c094dcf0765afedd12cb5156da95:
.. index:: pair: function; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	details::BlobIterator<T> end()

Gets BlobIterator for the end of data.

Enables a ranged loop support for the :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object.



.. rubric:: Returns:

BlobIterator object of type T representing end of the data

.. _doxid-class_inference_engine_1_1_t_blob_1adf6d6f90b068f0fbe8959b214471a30d:
.. index:: pair: function; begin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	details::BlobIterator<const T> begin() const

Gets a const BlobIterator for the read-only data.

Enables a ranged loop support for the :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object.



.. rubric:: Returns:

BlobIterator object of type const T

.. _doxid-class_inference_engine_1_1_t_blob_1a16dceb89e0b31f53b5d3ac2439295700:
.. index:: pair: function; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	details::BlobIterator<const T> end() const

Gets a const BlobIterator for the end of read-only data.

Enables a ranged loop support for the :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>` object.



.. rubric:: Returns:

BlobIterator object of type const T representing end of data


