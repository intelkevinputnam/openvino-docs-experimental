.. index:: pair: class; InferenceEngine::gpu::D3DContext
.. _doxid-class_inference_engine_1_1gpu_1_1_d3_d_context:

class InferenceEngine::gpu::D3DContext
======================================



Overview
~~~~~~~~

This class represents an abstraction for GPU plugin remote context which is shared with Direct3D 11 device. The plugin object derived from this class can be obtained either with GetContext() method of Executable network or using CreateContext() :ref:`Core <doxid-class_inference_engine_1_1_core>` call. :ref:`More...<details-class_inference_engine_1_1gpu_1_1_d3_d_context>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <gpu_context_api_dx.hpp>
	
	class D3DContext: public :ref:`InferenceEngine::gpu::ClContext<doxid-class_inference_engine_1_1gpu_1_1_cl_context>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<D3DContext> :ref:`Ptr<doxid-class_inference_engine_1_1gpu_1_1_d3_d_context_1a1ece9eae5ddc8fa89bfe29f8e693b83e>`;

		// methods
	
		:ref:`operator ID3D11Device \*<doxid-class_inference_engine_1_1gpu_1_1_d3_d_context_1abe837ad0a05b08d331a38a7925cf497c>` ();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`;
		typedef std::shared_ptr<const :ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`CPtr<doxid-class_inference_engine_1_1_remote_context_1a67424c5e4360db20e621ced6fbd406be>`;
		typedef std::shared_ptr<:ref:`ClContext<doxid-class_inference_engine_1_1gpu_1_1_cl_context>`> :ref:`Ptr<doxid-class_inference_engine_1_1gpu_1_1_cl_context_1a7c6b73b0d487f9a35644e696d89eca3a>`;

		// methods
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		bool :ref:`is<doxid-class_inference_engine_1_1_remote_context_1acf2f061a42ddb6678ef6e04df868a9b8>`();
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		bool :ref:`is<doxid-class_inference_engine_1_1_remote_context_1a7101e3faa737b9fa6c4d69e5d89358ef>`() const;
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		T \* :ref:`as<doxid-class_inference_engine_1_1_remote_context_1a9b0aa51076f3293c14c8967fa390098f>`();
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		const T \* :ref:`as<doxid-class_inference_engine_1_1_remote_context_1ad46a1b2173cc5806c907976c79f76e71>`() const;
	
		virtual std::string :ref:`getDeviceName<doxid-class_inference_engine_1_1_remote_context_1a5d3cd0e80b7b5442082e8bc51e42e1c3>`() const = 0;
	
		virtual :ref:`RemoteBlob::Ptr<doxid-class_inference_engine_1_1_remote_blob_1a495fd7cc9fbb55b2e0b6bc8b8790197b>` :ref:`CreateBlob<doxid-class_inference_engine_1_1_remote_context_1afe1313eb1a0d6f06fbb4a99889956145>`(
			const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc,
			const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params = {}
			) = 0;
	
		virtual :ref:`MemoryBlob::Ptr<doxid-class_inference_engine_1_1_memory_blob_1a294bf7449b6181f29ac05636a5968e1d>` :ref:`CreateHostBlob<doxid-class_inference_engine_1_1_remote_context_1a1c4a610a7e4ec6c9e66a338e858635da>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc);
		virtual :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>` :ref:`getParams<doxid-class_inference_engine_1_1_remote_context_1a2c6be24d0fbf02fcd3028b81945e8c90>`() const = 0;
		cl_context :ref:`get<doxid-class_inference_engine_1_1gpu_1_1_cl_context_1a90d4b3b912ac3be27cee9f268ed4226b>`();
		:ref:`operator cl_context<doxid-class_inference_engine_1_1gpu_1_1_cl_context_1a728bc5955540b7a8b10e6b586c80dd4d>` ();
		:ref:`operator cl::Context<doxid-class_inference_engine_1_1gpu_1_1_cl_context_1a81c0abc24cca2156cea79b262de82342>` ();

.. _details-class_inference_engine_1_1gpu_1_1_d3_d_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an abstraction for GPU plugin remote context which is shared with Direct3D 11 device. The plugin object derived from this class can be obtained either with GetContext() method of Executable network or using CreateContext() :ref:`Core <doxid-class_inference_engine_1_1_core>` call.

User can also obtain OpenCL context handle from this class.

Typedefs
--------

.. _doxid-class_inference_engine_1_1gpu_1_1_d3_d_context_1a1ece9eae5ddc8fa89bfe29f8e693b83e:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<D3DContext> Ptr

A smart pointer to the :ref:`D3DContext <doxid-class_inference_engine_1_1gpu_1_1_d3_d_context>` object.

Methods
-------

.. _doxid-class_inference_engine_1_1gpu_1_1_d3_d_context_1abe837ad0a05b08d331a38a7925cf497c:
.. index:: pair: function; operator ID3D11Device \*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator ID3D11Device \* ()

ID3D11Device conversion operator for the :ref:`D3DContext <doxid-class_inference_engine_1_1gpu_1_1_d3_d_context>` object.



.. rubric:: Returns:

Pointer to underlying ID3D11Device interface


