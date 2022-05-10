.. index:: pair: class; InferenceEngine::RemoteBlob
.. _doxid-class_inference_engine_1_1_remote_blob:

class InferenceEngine::RemoteBlob
=================================



Overview
~~~~~~~~

This class represents an Inference Engine abstraction to the memory allocated on the remote (non-CPU) accelerator device. :ref:`More...<details-class_inference_engine_1_1_remote_blob>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_remote_blob.hpp>
	
	class RemoteBlob: public :ref:`InferenceEngine::MemoryBlob<doxid-class_inference_engine_1_1_memory_blob>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<RemoteBlob> :ref:`Ptr<doxid-class_inference_engine_1_1_remote_blob_1a495fd7cc9fbb55b2e0b6bc8b8790197b>`;
		typedef std::shared_ptr<const RemoteBlob> :ref:`CPtr<doxid-class_inference_engine_1_1_remote_blob_1ac9b3ea19eb8864a1655b7ad8bb507521>`;

		// construction
	
		:ref:`RemoteBlob<doxid-class_inference_engine_1_1_remote_blob_1aa660897f19de20a3fd0f232ef200079f>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc);

		// methods
	
		virtual :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>` :ref:`getParams<doxid-class_inference_engine_1_1_remote_blob_1a505189408daf040db661b9aa3165e9fe>`() const = 0;
		virtual std::string :ref:`getDeviceName<doxid-class_inference_engine_1_1_remote_blob_1a73fe7479d1226ad52b68ea1bdba71336>`() const = 0;
		virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`getContext<doxid-class_inference_engine_1_1_remote_blob_1afbce14019dbc6cbb3916606133f2df7c>`() const = 0;
	};

	// direct descendants

	class :ref:`ClBlob<doxid-class_inference_engine_1_1gpu_1_1_cl_blob>`;

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

.. _details-class_inference_engine_1_1_remote_blob:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an Inference Engine abstraction to the memory allocated on the remote (non-CPU) accelerator device.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_remote_blob_1a495fd7cc9fbb55b2e0b6bc8b8790197b:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<RemoteBlob> Ptr

A smart pointer to the :ref:`RemoteBlob <doxid-class_inference_engine_1_1_remote_blob>` object.

.. _doxid-class_inference_engine_1_1_remote_blob_1ac9b3ea19eb8864a1655b7ad8bb507521:
.. index:: pair: typedef; CPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<const RemoteBlob> CPtr

A smart pointer to the const :ref:`RemoteBlob <doxid-class_inference_engine_1_1_remote_blob>` object.

Construction
------------

.. _doxid-class_inference_engine_1_1_remote_blob_1aa660897f19de20a3fd0f232ef200079f:
.. index:: pair: function; RemoteBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RemoteBlob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc)

Constructor. Creates an empty :ref:`RemoteBlob <doxid-class_inference_engine_1_1_remote_blob>` object with the specified precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Defines the layout and dims of the blob

Methods
-------

.. _doxid-class_inference_engine_1_1_remote_blob_1a505189408daf040db661b9aa3165e9fe:
.. index:: pair: function; getParams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>` getParams() const = 0

Returns a map of device-specific parameters required for low-level operations with underlying object. Parameters include device/context/surface/buffer handles, access flags, etc. Contents of the map returned depend on remote execution context that is currently set on the device (working scenario). Abstract method.



.. rubric:: Returns:

A map of name/parameter elements.

.. _doxid-class_inference_engine_1_1_remote_blob_1a73fe7479d1226ad52b68ea1bdba71336:
.. index:: pair: function; getDeviceName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getDeviceName() const = 0

Returns name of the device on which underlying object is allocated. Abstract method.



.. rubric:: Returns:

A device name string in the same format as that in plugin metric.

.. _doxid-class_inference_engine_1_1_remote_blob_1afbce14019dbc6cbb3916606133f2df7c:
.. index:: pair: function; getContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> getContext() const = 0

Returns device context which underlying object belongs to. Abstract method.



.. rubric:: Returns:

Pointer to plugin-specific context class object, which is derived from :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>`. Dynamic casting should be used if it is necessary to retrieve a pointer to original class.


