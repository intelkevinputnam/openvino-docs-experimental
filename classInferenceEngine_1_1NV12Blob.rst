.. index:: pair: class; InferenceEngine::NV12Blob
.. _doxid-class_inference_engine_1_1_n_v12_blob:

class InferenceEngine::NV12Blob
===============================



Overview
~~~~~~~~

Represents a blob that contains two planes (Y and UV) in NV12 color format. :ref:`More...<details-class_inference_engine_1_1_n_v12_blob>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_compound_blob.h>
	
	class NV12Blob: public :ref:`InferenceEngine::CompoundBlob<doxid-class_inference_engine_1_1_compound_blob>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<NV12Blob> :ref:`Ptr<doxid-class_inference_engine_1_1_n_v12_blob_1ac260e7305ce71fdd838301e9dcd53ec7>`;
		typedef std::shared_ptr<const NV12Blob> :ref:`CPtr<doxid-class_inference_engine_1_1_n_v12_blob_1ae2720f95df88ab1ef4ccce1611bfe424>`;

		// construction
	
		:ref:`NV12Blob<doxid-class_inference_engine_1_1_n_v12_blob_1a337054872ece1e3199d362fda614a1f5>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& y, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& uv);
		:ref:`NV12Blob<doxid-class_inference_engine_1_1_n_v12_blob_1a8a34496f2aef2e04ad70ce8c1acd4d7a>`(:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`&& y, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`&& uv);

		// methods
	
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& :ref:`y<doxid-class_inference_engine_1_1_n_v12_blob_1af4d389bbe16ee548929a2e1c1a44e1d4>`();
		virtual const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& :ref:`y<doxid-class_inference_engine_1_1_n_v12_blob_1aab2a22a8678e9210ff7ea27d7490c020>`() const;
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& :ref:`uv<doxid-class_inference_engine_1_1_n_v12_blob_1a79955bd3c230a6e5bbb74e8bd8f47aff>`();
		virtual const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& :ref:`uv<doxid-class_inference_engine_1_1_n_v12_blob_1af75f88db2eeb6b1615df39df4707ed65>`() const;
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`createROI<doxid-class_inference_engine_1_1_n_v12_blob_1ac4cb3a08ad6841948e5b15638f126b79>`(const :ref:`ROI<doxid-struct_inference_engine_1_1_r_o_i>`& roi) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Blob<doxid-class_inference_engine_1_1_blob>`> :ref:`Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`;
		typedef std::shared_ptr<const :ref:`Blob<doxid-class_inference_engine_1_1_blob>`> :ref:`CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`;
		typedef std::shared_ptr<:ref:`CompoundBlob<doxid-class_inference_engine_1_1_compound_blob>`> :ref:`Ptr<doxid-class_inference_engine_1_1_compound_blob_1a221e3df953582193b6ed368a77289a98>`;
		typedef std::shared_ptr<const :ref:`CompoundBlob<doxid-class_inference_engine_1_1_compound_blob>`> :ref:`CPtr<doxid-class_inference_engine_1_1_compound_blob_1a0a27941cd30b935e883c508bb9afaaa8>`;

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
	
		virtual size_t :ref:`byteSize<doxid-class_inference_engine_1_1_compound_blob_1a44991841b0c5e0c4d59cb67863ff6c8d>`() const;
		virtual size_t :ref:`element_size<doxid-class_inference_engine_1_1_compound_blob_1a25b096472d5585e82d047591da90b0c2>`() const;
		virtual void :ref:`allocate<doxid-class_inference_engine_1_1_compound_blob_1ab49e22966230d1e137c63bca61cd775a>`();
		virtual bool :ref:`deallocate<doxid-class_inference_engine_1_1_compound_blob_1a65307d800fa94e7de5a7cb0bb28a8c8d>`();
		virtual size_t :ref:`size<doxid-class_inference_engine_1_1_compound_blob_1ac347042740c87baf7983b5b5e16c4b84>`() const;
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`getBlob<doxid-class_inference_engine_1_1_compound_blob_1a2cf2bc882a75a0512ba9d246da2e8e54>`(size_t i) const;
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`createROI<doxid-class_inference_engine_1_1_compound_blob_1a6c5316072ad7f16b9e6d99487b6ccdec>`(const :ref:`ROI<doxid-struct_inference_engine_1_1_r_o_i>`& roi) const;

.. _details-class_inference_engine_1_1_n_v12_blob:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents a blob that contains two planes (Y and UV) in NV12 color format.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_n_v12_blob_1ac260e7305ce71fdd838301e9dcd53ec7:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<NV12Blob> Ptr

A smart pointer to the :ref:`NV12Blob <doxid-class_inference_engine_1_1_n_v12_blob>` object.

.. _doxid-class_inference_engine_1_1_n_v12_blob_1ae2720f95df88ab1ef4ccce1611bfe424:
.. index:: pair: typedef; CPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<const NV12Blob> CPtr

A smart pointer to the const :ref:`NV12Blob <doxid-class_inference_engine_1_1_n_v12_blob>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_n_v12_blob_1a337054872ece1e3199d362fda614a1f5:
.. index:: pair: function; NV12Blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NV12Blob(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& y, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& uv)

Constructs NV12 blob from two planes Y and UV.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- y

		- :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object that represents Y plane in NV12 color format

	*
		- uv

		- :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object that represents UV plane in NV12 color format

.. _doxid-class_inference_engine_1_1_n_v12_blob_1a8a34496f2aef2e04ad70ce8c1acd4d7a:
.. index:: pair: function; NV12Blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NV12Blob(:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`&& y, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`&& uv)

Constructs NV12 blob from two planes Y and UV.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- y

		- :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object that represents Y plane in NV12 color format

	*
		- uv

		- :ref:`Blob <doxid-class_inference_engine_1_1_blob>` object that represents UV plane in NV12 color format

Methods
-------

.. _doxid-class_inference_engine_1_1_n_v12_blob_1af4d389bbe16ee548929a2e1c1a44e1d4:
.. index:: pair: function; y

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& y()

Returns a shared pointer to Y plane.



.. rubric:: Returns:

Y plane

.. _doxid-class_inference_engine_1_1_n_v12_blob_1aab2a22a8678e9210ff7ea27d7490c020:
.. index:: pair: function; y

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& y() const

Returns a shared pointer to Y plane.



.. rubric:: Returns:

Y plane

.. _doxid-class_inference_engine_1_1_n_v12_blob_1a79955bd3c230a6e5bbb74e8bd8f47aff:
.. index:: pair: function; uv

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& uv()

Returns a shared pointer to UV plane.



.. rubric:: Returns:

UV plane

.. _doxid-class_inference_engine_1_1_n_v12_blob_1af75f88db2eeb6b1615df39df4707ed65:
.. index:: pair: function; uv

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& uv() const

Returns a shared pointer to UV plane.



.. rubric:: Returns:

UV plane

.. _doxid-class_inference_engine_1_1_n_v12_blob_1ac4cb3a08ad6841948e5b15638f126b79:
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


