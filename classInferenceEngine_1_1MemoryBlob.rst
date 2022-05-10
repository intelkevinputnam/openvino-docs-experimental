.. index:: pair: class; InferenceEngine::MemoryBlob
.. _doxid-class_inference_engine_1_1_memory_blob:

class InferenceEngine::MemoryBlob
=================================



Overview
~~~~~~~~

This class implements a container object that represents a tensor in memory (host and remote/accelerated) :ref:`More...<details-class_inference_engine_1_1_memory_blob>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_blob.h>
	
	class MemoryBlob: public :ref:`InferenceEngine::Blob<doxid-class_inference_engine_1_1_blob>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<MemoryBlob> :ref:`Ptr<doxid-class_inference_engine_1_1_memory_blob_1a294bf7449b6181f29ac05636a5968e1d>`;
		typedef std::shared_ptr<const MemoryBlob> :ref:`CPtr<doxid-class_inference_engine_1_1_memory_blob_1adae370cdc2fa2649928498f9e25dec9e>`;

		// construction
	
		:ref:`MemoryBlob<doxid-class_inference_engine_1_1_memory_blob_1ab1d851868f45acfbb7b5a0288cddd9d5>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc);

		// methods
	
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
	};

	// direct descendants

	class :ref:`RemoteBlob<doxid-class_inference_engine_1_1_remote_blob>`;

	template <
		typename T,
		typename = std::enable_if<std::is_standard_layout<T>::value&& std::is_trivial<T>::value>
		>
	class :ref:`TBlob<doxid-class_inference_engine_1_1_t_blob>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Blob<doxid-class_inference_engine_1_1_blob>`> :ref:`Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`;
		typedef std::shared_ptr<const :ref:`Blob<doxid-class_inference_engine_1_1_blob>`> :ref:`CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`;

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

.. _details-class_inference_engine_1_1_memory_blob:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class implements a container object that represents a tensor in memory (host and remote/accelerated)

Any :ref:`Blob <doxid-class_inference_engine_1_1_blob>` implementation that represents a concept of a tensor in memory (for example, :ref:`TBlob <doxid-class_inference_engine_1_1_t_blob>`) must be a subclass of :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` instead of :ref:`Blob <doxid-class_inference_engine_1_1_blob>`

Typedefs
--------

.. _doxid-class_inference_engine_1_1_memory_blob_1a294bf7449b6181f29ac05636a5968e1d:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<MemoryBlob> Ptr

A smart pointer to the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` object.

.. _doxid-class_inference_engine_1_1_memory_blob_1adae370cdc2fa2649928498f9e25dec9e:
.. index:: pair: typedef; CPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<const MemoryBlob> CPtr

A smart pointer to the const :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_memory_blob_1ab1d851868f45acfbb7b5a0288cddd9d5:
.. index:: pair: function; MemoryBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MemoryBlob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc)

Constructor. Creates an empty :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` object with the specified precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Defines the layout and dims of the blob

Methods
-------

.. _doxid-class_inference_engine_1_1_memory_blob_1a359897a812bf64603a67e4fc92b71aae:
.. index:: pair: function; getTensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& getTensorDesc() const

Returns the tensor description.



.. rubric:: Returns:

A tensor description

.. _doxid-class_inference_engine_1_1_memory_blob_1ac86c87548512f03bebf72c47cde4cc65:
.. index:: pair: function; getTensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& getTensorDesc()

Returns the tensor description.



.. rubric:: Returns:

A tensor description

.. _doxid-class_inference_engine_1_1_memory_blob_1a733d578f1a002e9f84b65229a61b05d6:
.. index:: pair: function; size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t size() const

Returns the total number of elements, which is a product of all the dimensions.



.. rubric:: Returns:

The total number of elements

.. _doxid-class_inference_engine_1_1_memory_blob_1a4c1e80abfbca64b8c1d3d8918b7af084:
.. index:: pair: function; byteSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t byteSize() const

Returns the size of the current :ref:`Blob <doxid-class_inference_engine_1_1_blob>` in bytes calculated as ``:ref:`size() <doxid-class_inference_engine_1_1_memory_blob_1a733d578f1a002e9f84b65229a61b05d6>` \* :ref:`element_size() <doxid-class_inference_engine_1_1_memory_blob_1a9b2f80180ea50adcbcab1cd68932209f>```.



.. rubric:: Returns:

:ref:`Blob <doxid-class_inference_engine_1_1_blob>` 's size in bytes

.. _doxid-class_inference_engine_1_1_memory_blob_1a9b2f80180ea50adcbcab1cd68932209f:
.. index:: pair: function; element_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t element_size() const

Provides the number of bytes per element.

Deprecated Cast to :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` and use its API instead. :ref:`Blob <doxid-class_inference_engine_1_1_blob>` class can represent compound blob, which do not refer to the only solid memory.

The overall :ref:`Blob <doxid-class_inference_engine_1_1_blob>` capacity is :ref:`size() <doxid-class_inference_engine_1_1_memory_blob_1a733d578f1a002e9f84b65229a61b05d6>` \* :ref:`element_size() <doxid-class_inference_engine_1_1_memory_blob_1a9b2f80180ea50adcbcab1cd68932209f>`. Abstract method.



.. rubric:: Returns:

Returns the number of bytes per element

.. _doxid-class_inference_engine_1_1_memory_blob_1a6b8605e3863617c5985d21bc91837b8f:
.. index:: pair: function; allocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void allocate() = 0

Allocates memory to store the data.

Abstract method.

.. _doxid-class_inference_engine_1_1_memory_blob_1ad462f247d8dffc1e525f51899448a60c:
.. index:: pair: function; deallocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool deallocate() = 0

Releases previously allocated data.

Abstract method.



.. rubric:: Returns:

``True`` if deallocation happens successfully, ``false`` otherwise.

.. _doxid-class_inference_engine_1_1_memory_blob_1a715863b45d88b97937e770d866bf1784:
.. index:: pair: function; rwmap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> rwmap() = 0

Gets read/write access to the memory in virtual space of the process. The function returns object which retains mapped memory. The memory been addressed in the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` in general case can be allocated on remote device. This function maps remote memory to the memory in the virtual process space and after destruction of the :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` will upload changed content to the accelerator.

To avoid extra copy of data, you can use :ref:`rmap() <doxid-class_inference_engine_1_1_memory_blob_1a055940ba42eb270f348bedea9726cf12>` and :ref:`wmap() <doxid-class_inference_engine_1_1_memory_blob_1ac5c6b1ecf54a69f98a06df6d05187a7f>` functions.

In case of memory originally allocated on the host, this function returns :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` which will transparently refer to original memory address. No extra copy will happen

In general case, pointer received from that :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` becomes invalid just after destruction of :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` instance. Keep Locked memory alive while you need to address memory in the process on the host.

Abstract method.



.. rubric:: Returns:

A :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object

.. _doxid-class_inference_engine_1_1_memory_blob_1a055940ba42eb270f348bedea9726cf12:
.. index:: pair: function; rmap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const void> rmap() const = 0

Gets read only access to the memory in virtual space of the process. The function returns object which retains mapped memory.

The memory been addressed in the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` in general case can be allocated on remote device. This function copies remote memory to the memory in the virtual process space and after destruction of the :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` it will not upload host memory back, because it is expected that content is not changed.

To have an ability change content, you can use :ref:`rwmap() <doxid-class_inference_engine_1_1_memory_blob_1a715863b45d88b97937e770d866bf1784>` and :ref:`wmap() <doxid-class_inference_engine_1_1_memory_blob_1ac5c6b1ecf54a69f98a06df6d05187a7f>` functions.

In case of memory originally allocated on the host, this function returns :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` which will transparently refer to original memory address. No extra copy will happen

In general case, pointer received from that :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` becomes invalid just after destruction of :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` instance. Keep Locked memory alive while you need to address memory in the process on the host.

Abstract method.



.. rubric:: Returns:

A :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object

.. _doxid-class_inference_engine_1_1_memory_blob_1ac5c6b1ecf54a69f98a06df6d05187a7f:
.. index:: pair: function; wmap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void> wmap() = 0

Gets "write only direction" access to the memory in virtual space of the process. The function returns object which retains memory to be uploaded on device.

The memory been addressed in the :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` in general case can be allocated on remote device. This function does not copy of the content from the device to the memory in the virtual process space, the content of the memory just after calling of this function is not specified. After destruction of the :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>`, content will be upload host memory. In the same time there is no abilities to restrict reading from the memory, you need to care of reading from memory got by :ref:`wmap() <doxid-class_inference_engine_1_1_memory_blob_1ac5c6b1ecf54a69f98a06df6d05187a7f>`, it might have sense in some cases like filling of content and before uploading to device

To access data stored in the blob, you can use :ref:`rwmap() <doxid-class_inference_engine_1_1_memory_blob_1a715863b45d88b97937e770d866bf1784>` and :ref:`rmap() <doxid-class_inference_engine_1_1_memory_blob_1a055940ba42eb270f348bedea9726cf12>` functions.

In case of memory originally allocated on the host, this function returns :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` which will transparently refer to original memory address. No extra copy will happen

In general case, pointer received from that :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` becomes invalid just after destruction of :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` instance. Keep Locked memory alive while you need to address memory in the process on the host.

Abstract method.



.. rubric:: Returns:

A :ref:`LockedMemory <doxid-class_inference_engine_1_1_locked_memory>` object


