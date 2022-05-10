.. index:: pair: class; InferenceEngine::Blob
.. _doxid-class_inference_engine_1_1_blob:

class InferenceEngine::Blob
===========================



Overview
~~~~~~~~

This class represents a universal container in the Inference Engine. :ref:`More...<details-class_inference_engine_1_1_blob>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_blob.h>
	
	class Blob
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Blob> :ref:`Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`;
		typedef std::shared_ptr<const Blob> :ref:`CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`;

		// construction
	
		:ref:`Blob<doxid-class_inference_engine_1_1_blob_1ae66c8ccdfa63fd8554c431437fcf15d1>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc);

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
	};

	// direct descendants

	class :ref:`CompoundBlob<doxid-class_inference_engine_1_1_compound_blob>`;
	class :ref:`MemoryBlob<doxid-class_inference_engine_1_1_memory_blob>`;
.. _details-class_inference_engine_1_1_blob:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents a universal container in the Inference Engine.

Each :ref:`Blob <doxid-class_inference_engine_1_1_blob>` implementation must be derived from this :ref:`Blob <doxid-class_inference_engine_1_1_blob>` class directly or indirectly

Typedefs
--------

.. _doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<Blob> Ptr

A smart pointer containing :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object.

.. _doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092:
.. index:: pair: typedef; CPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<const Blob> CPtr

A smart pointer to the const :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_blob_1ae66c8ccdfa63fd8554c431437fcf15d1:
.. index:: pair: function; Blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Blob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc)

Constructor. Creates an empty :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object with the specified precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Defines the layout and dims of the blob

Methods
-------

.. _doxid-class_inference_engine_1_1_blob_1ae81db862104a25e3fb41f57d94dd41a6:
.. index:: pair: function; CreateFromData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` CreateFromData(const :ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`& data)

Creates a TBlob<> object from a :ref:`Data <doxid-class_inference_engine_1_1_data>` node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- data

		- A reference to a smart pointer of the :ref:`Data <doxid-class_inference_engine_1_1_data>` node



.. rubric:: Returns:

Smart pointer to TBlob<> with the relevant C type to the precision of the data node

.. _doxid-class_inference_engine_1_1_blob_1aa07152ba7c9910abab46a7e8e58323bc:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
		>
	bool is()

Checks if the :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object can be cast to the type T\*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to be checked. Must represent a class derived from the :ref:`Blob <doxid-class_inference_engine_1_1_blob>`



.. rubric:: Returns:

true if this object can be dynamically cast to the type T\*. Otherwise, false

.. _doxid-class_inference_engine_1_1_blob_1a74f56a3007a5dbabd8acda5e11d9568c:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
		>
	bool is() const

Checks if the :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object can be cast to the type const T\*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to be checked. Must represent a class derived from the :ref:`Blob <doxid-class_inference_engine_1_1_blob>`



.. rubric:: Returns:

true if this object can be dynamically cast to the type const T\*. Otherwise, false

.. _doxid-class_inference_engine_1_1_blob_1abc7e63536f5f3811ba2b01455ad06954:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
		>
	T \* as()

Casts this :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object to the type T\*.

Use :ref:`InferenceEngine::as() <doxid-namespace_inference_engine_1a2221ba6e6a6337f6b40fb6e1d49f0a8c>` to operate with shared :ref:`Blob <doxid-class_inference_engine_1_1_blob>` objects instead of raw pointers



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to cast to. Must represent a class derived from the :ref:`Blob <doxid-class_inference_engine_1_1_blob>`



.. rubric:: Returns:

Raw pointer to the object of the type T or nullptr on error

.. _doxid-class_inference_engine_1_1_blob_1aa7f7eef35f32cf11c76f3db57bd555f6:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<Blob, T>::value, int>::type = 0
		>
	const T \* as() const

Casts this :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object to the type const T\*.

Use :ref:`InferenceEngine::as() <doxid-namespace_inference_engine_1a2221ba6e6a6337f6b40fb6e1d49f0a8c>` to operate with shared :ref:`Blob <doxid-class_inference_engine_1_1_blob>` objects instead of raw pointers



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to cast to. Must represent a class derived from the :ref:`Blob <doxid-class_inference_engine_1_1_blob>`



.. rubric:: Returns:

Raw pointer to the object of the type const T or nullptr on error

.. _doxid-class_inference_engine_1_1_blob_1accdd939c62592f28a0ceb64cd60eb62e:
.. index:: pair: function; getTensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& getTensorDesc() const

Returns the tensor description.



.. rubric:: Returns:

A const reference to a tensor descriptor

.. _doxid-class_inference_engine_1_1_blob_1aaa14e36bf31d98a9c9db1054811201f0:
.. index:: pair: function; getTensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& getTensorDesc()

Returns the tensor description.



.. rubric:: Returns:

A reference to a tensor descriptor

.. _doxid-class_inference_engine_1_1_blob_1a2b5686fa129fdbe3d4ccc44210d911f7:
.. index:: pair: function; size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t size() const

By default, returns the total number of elements (a product of all the dims or 1 for scalar)

Return value and its interpretation heavily depend on the blob type



.. rubric:: Returns:

The total number of elements

.. _doxid-class_inference_engine_1_1_blob_1a9f2049e262cea015e7640a82e4d70ccb:
.. index:: pair: function; byteSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t byteSize() const

Returns the size of the current :ref:`Blob <doxid-class_inference_engine_1_1_blob>` in bytes.



.. rubric:: Returns:

:ref:`Blob <doxid-class_inference_engine_1_1_blob>` 's size in bytes

.. _doxid-class_inference_engine_1_1_blob_1a25690a7dd30e0c07abbf32f09c5f8735:
.. index:: pair: function; element_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t element_size() const = 0

Provides the number of bytes per element.

Deprecated Cast to :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` and use its API instead. :ref:`Blob <doxid-class_inference_engine_1_1_blob>` class can represent compound blob, which do not refer to the only solid memory.

The overall :ref:`Blob <doxid-class_inference_engine_1_1_blob>` capacity is :ref:`size() <doxid-class_inference_engine_1_1_blob_1a2b5686fa129fdbe3d4ccc44210d911f7>` \* :ref:`element_size() <doxid-class_inference_engine_1_1_blob_1a25690a7dd30e0c07abbf32f09c5f8735>`. Abstract method.



.. rubric:: Returns:

Returns the number of bytes per element

.. _doxid-class_inference_engine_1_1_blob_1a88866d4156b7936e2d60d7fff8c9f230:
.. index:: pair: function; allocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void allocate() = 0

Allocates memory to store the data.

Abstract method.

.. _doxid-class_inference_engine_1_1_blob_1af9ccc77bec5dbebd179291bbd88af881:
.. index:: pair: function; deallocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool deallocate() = 0

Releases previously allocated data.

Abstract method.



.. rubric:: Returns:

``True`` if deallocation happens successfully, ``false`` otherwise.

.. _doxid-class_inference_engine_1_1_blob_1abdce9a4dc4319da76b283ac68f9c0283:
.. index:: pair: function; setShape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setShape(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims)

Set new shape for blob, deallocate/allocate if new total size is bigger than previous one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- new shape

.. _doxid-class_inference_engine_1_1_blob_1a81168f9425c1d7c5fdb6f52210213a39:
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

.. _doxid-class_inference_engine_1_1_blob_1a39d758fa25f8268c32af77379b062fbb:
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


