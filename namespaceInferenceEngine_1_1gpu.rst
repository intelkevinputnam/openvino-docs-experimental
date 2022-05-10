.. index:: pair: namespace; InferenceEngine::gpu
.. _doxid-namespace_inference_engine_1_1gpu:

namespace InferenceEngine::gpu
==============================

.. toctree::
	:hidden:

	ClBlob <classInferenceEngine_1_1gpu_1_1ClBlob.rst>
	ClBufferBlob <classInferenceEngine_1_1gpu_1_1ClBufferBlob.rst>
	ClContext <classInferenceEngine_1_1gpu_1_1ClContext.rst>
	ClImage2DBlob <classInferenceEngine_1_1gpu_1_1ClImage2DBlob.rst>
	D3DBufferBlob <classInferenceEngine_1_1gpu_1_1D3DBufferBlob.rst>
	D3DContext <classInferenceEngine_1_1gpu_1_1D3DContext.rst>
	D3DSurface2DBlob <classInferenceEngine_1_1gpu_1_1D3DSurface2DBlob.rst>
	USMBlob <classInferenceEngine_1_1gpu_1_1USMBlob.rst>
	VAContext <classInferenceEngine_1_1gpu_1_1VAContext.rst>
	VASurfaceBlob <classInferenceEngine_1_1gpu_1_1VASurfaceBlob.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace gpu {

	// classes

	class :ref:`ClBlob<doxid-class_inference_engine_1_1gpu_1_1_cl_blob>`;
	class :ref:`ClBufferBlob<doxid-class_inference_engine_1_1gpu_1_1_cl_buffer_blob>`;
	class :ref:`ClContext<doxid-class_inference_engine_1_1gpu_1_1_cl_context>`;
	class :ref:`ClImage2DBlob<doxid-class_inference_engine_1_1gpu_1_1_cl_image2_d_blob>`;
	class :ref:`D3DBufferBlob<doxid-class_inference_engine_1_1gpu_1_1_d3_d_buffer_blob>`;
	class :ref:`D3DContext<doxid-class_inference_engine_1_1gpu_1_1_d3_d_context>`;
	class :ref:`D3DSurface2DBlob<doxid-class_inference_engine_1_1gpu_1_1_d3_d_surface2_d_blob>`;
	class :ref:`USMBlob<doxid-class_inference_engine_1_1gpu_1_1_u_s_m_blob>`;
	class :ref:`VAContext<doxid-class_inference_engine_1_1gpu_1_1_v_a_context>`;
	class :ref:`VASurfaceBlob<doxid-class_inference_engine_1_1gpu_1_1_v_a_surface_blob>`;

	// global functions

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob_nv12<doxid-namespace_inference_engine_1_1gpu_1ac72ef58817d0933f40f735ba3e19dda0>`(
		size_t height,
		size_t width,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		ID3D11Texture2D \* nv12_surf
		);

	static :ref:`D3DContext::Ptr<doxid-class_inference_engine_1_1gpu_1_1_d3_d_context_1a1ece9eae5ddc8fa89bfe29f8e693b83e>` :ref:`make_shared_context<doxid-namespace_inference_engine_1_1gpu_1a5a979f098ea0dc89cd46c71b805302a0>`(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		ID3D11Device \* device,
		int target_tile_id = -1
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1acbf3f7789d4a3c2daa4c63891d8e8577>`(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		ID3D11Buffer \* buffer
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1a53c4517258c8b6e439f561bfedca845f>`(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		ID3D11Texture2D \* surface,
		uint32_t plane = 0
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob_nv12<doxid-namespace_inference_engine_1_1gpu_1a9b13e6964400f1d6724baad7c4c86876>`(
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl::Image2D& nv12_image_plane_y,
		cl::Image2D& nv12_image_plane_uv
		);

	static :ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`make_shared_context<doxid-namespace_inference_engine_1_1gpu_1ad6313247a73161759773e2b3fd054fb0>`(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		cl_context ctx,
		int target_tile_id = -1
		);

	static :ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`make_shared_context<doxid-namespace_inference_engine_1_1gpu_1abe7febe6387e312731fafe76efa3fa2c>`(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		cl_command_queue queue
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1a60b59713ecdd4d400b17ff47cefe0da0>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc, :ref:`ClContext::Ptr<doxid-class_inference_engine_1_1gpu_1_1_cl_context_1a7c6b73b0d487f9a35644e696d89eca3a>` ctx);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1aff39e19df2cf6916a5599dd195bcd0c3>`(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl::Buffer& buffer
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1a33d130489a10ed2d10c2a9dbc842b62a>`(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl_mem buffer
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1ae96aec1659ebd3283c478c09f6e8cfae>`(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl::Image2D& image
		);

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_shared_blob_nv12<doxid-namespace_inference_engine_1_1gpu_1acaa3dc7389d6fdfaa5452e08ba925489>`(
		size_t height,
		size_t width,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		VASurfaceID nv12_surf
		);

	static :ref:`VAContext::Ptr<doxid-class_inference_engine_1_1gpu_1_1_v_a_context_1a618acae0ec67eddf09180c6af6ca343e>` :ref:`make_shared_context<doxid-namespace_inference_engine_1_1gpu_1a251bc7130aab41116ebdccc9955a2bae>`(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		VADisplay device,
		int target_tile_id = -1
		);

	static :ref:`VASurfaceBlob::Ptr<doxid-class_inference_engine_1_1gpu_1_1_v_a_surface_blob_1a79c56780d0dd02794c837ccabbad4b3b>` :ref:`make_shared_blob<doxid-namespace_inference_engine_1_1gpu_1a34c6c5f89430f39651644f76b52a0901>`(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		VASurfaceID surface,
		uint32_t plane = 0
		);

	} // namespace gpu
.. _details-namespace_inference_engine_1_1gpu:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespace_inference_engine_1_1gpu_1ac72ef58817d0933f40f735ba3e19dda0:
.. index:: pair: function; make_shared_blob_nv12

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob_nv12(
		size_t height,
		size_t width,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		ID3D11Texture2D \* nv12_surf
		)

This function is used to obtain a NV12 compound blob object from NV12 DXGI video decoder output. The resulting compound contains two remote blobs for Y and UV planes of the surface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- height

		- Height of Y plane

	*
		- width

		- Widht of Y plane

	*
		- ctx

		- A pointer to remote context

	*
		- nv12_surf

		- A ID3D11Texture2D instance to create NV12 blob from



.. rubric:: Returns:

NV12 remote blob

.. _doxid-namespace_inference_engine_1_1gpu_1a5a979f098ea0dc89cd46c71b805302a0:
.. index:: pair: function; make_shared_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`D3DContext::Ptr<doxid-class_inference_engine_1_1gpu_1_1_d3_d_context_1a1ece9eae5ddc8fa89bfe29f8e693b83e>` make_shared_context(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		ID3D11Device \* device,
		int target_tile_id = -1
		)

This function is used to obtain remote context object from ID3D11Device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` object instance

	*
		- deviceName

		- A name of to create a remote context for

	*
		- device

		- A pointer to ID3D11Device to be used to create a remote context

	*
		- target_tile_id

		- Desired tile id within given context for multi-tile system. Default value (-1) means that root device should be used



.. rubric:: Returns:

A shared remote context instance

.. _doxid-namespace_inference_engine_1_1gpu_1acbf3f7789d4a3c2daa4c63891d8e8577:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		ID3D11Buffer \* buffer
		)

This function is used to obtain remote blob object from ID3D11Buffer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- A tensor description which describes blob configuration

	*
		- ctx

		- A shared pointer to a remote context

	*
		- buffer

		- A pointer to ID3D11Buffer instance to create remote blob based on



.. rubric:: Returns:

A remote blob instance

.. _doxid-namespace_inference_engine_1_1gpu_1a53c4517258c8b6e439f561bfedca845f:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		ID3D11Texture2D \* surface,
		uint32_t plane = 0
		)

This function is used to obtain remote blob object from ID3D11Texture2D.

The underlying ID3D11Texture2D can also be a plane of output surface of DXGI video decoder



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- Tensor description

	*
		- ctx

		- the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object whuch owns context for the blob to be created

	*
		- surface

		- Pointer to ID3D11Texture2D interface of the objects that owns NV12 texture

	*
		- plane

		- ID of the plane to be shared (0 or 1)



.. rubric:: Returns:

Smart pointer to created :ref:`RemoteBlob <doxid-class_inference_engine_1_1_remote_blob>` object cast to base class

.. _doxid-namespace_inference_engine_1_1gpu_1a9b13e6964400f1d6724baad7c4c86876:
.. index:: pair: function; make_shared_blob_nv12

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob_nv12(
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl::Image2D& nv12_image_plane_y,
		cl::Image2D& nv12_image_plane_uv
		)

This function is used to construct a NV12 compound blob object from two cl::Image2D wrapper objects. The resulting compound contains two remote blobs for Y and UV planes of the surface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ctx

		- :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` plugin object derived from :ref:`ClContext <doxid-class_inference_engine_1_1gpu_1_1_cl_context>` class.

	*
		- nv12_image_plane_y

		- cl::Image2D object containing Y plane data.

	*
		- nv12_image_plane_uv

		- cl::Image2D object containing UV plane data.



.. rubric:: Returns:

A shared remote blob instance

.. _doxid-namespace_inference_engine_1_1gpu_1ad6313247a73161759773e2b3fd054fb0:
.. index:: pair: function; make_shared_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` make_shared_context(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		cl_context ctx,
		int target_tile_id = -1
		)

This function is used to obtain remote context object from user-supplied OpenCL context handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- A reference to Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` object

	*
		- deviceName

		- A name of device to create a remote context for

	*
		- ctx

		- A OpenCL context to be used to create shared remote context

	*
		- target_tile_id

		- Desired tile id within given context for multi-tile system. Default value (-1) means that root device should be used



.. rubric:: Returns:

A shared remote context instance

.. _doxid-namespace_inference_engine_1_1gpu_1abe7febe6387e312731fafe76efa3fa2c:
.. index:: pair: function; make_shared_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` make_shared_context(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		cl_command_queue queue
		)

This function is used to obtain remote context object from user-supplied OpenCL context handle.

Only latency mode is supported for such context sharing case.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- A reference to Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` object

	*
		- deviceName

		- A name of device to create a remote context for

	*
		- queue

		- An OpenCL queue to be used to create shared remote context. Queue will be reused inside the plugin.



.. rubric:: Returns:

A shared remote context instance

.. _doxid-namespace_inference_engine_1_1gpu_1a60b59713ecdd4d400b17ff47cefe0da0:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc, :ref:`ClContext::Ptr<doxid-class_inference_engine_1_1gpu_1_1_cl_context_1a7c6b73b0d487f9a35644e696d89eca3a>` ctx)

This function is used to create remote blob object within default GPU plugin OpenCL context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- A tensor descriptor object representing remote blob configuration

	*
		- ctx

		- A remote context used to create remote blob



.. rubric:: Returns:

A remote blob instance

.. _doxid-namespace_inference_engine_1_1gpu_1aff39e19df2cf6916a5599dd195bcd0c3:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl::Buffer& buffer
		)

This function is used to obtain remote blob object from user-supplied cl::Buffer wrapper object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- A tensor descriptor object representing remote blob configuration

	*
		- ctx

		- A remote context used to create remote blob

	*
		- buffer

		- A cl::Buffer object wrapped by a remote blob



.. rubric:: Returns:

A remote blob instance

.. _doxid-namespace_inference_engine_1_1gpu_1a33d130489a10ed2d10c2a9dbc842b62a:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl_mem buffer
		)

This function is used to obtain remote blob object from user-supplied OpenCL buffer handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- A tensor descriptor object representing remote blob configuration

	*
		- ctx

		- A remote context used to create remote blob

	*
		- buffer

		- A cl_mem object wrapped by a remote blob



.. rubric:: Returns:

A remote blob instance

.. _doxid-namespace_inference_engine_1_1gpu_1ae96aec1659ebd3283c478c09f6e8cfae:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		cl::Image2D& image
		)

This function is used to obtain remote blob object from user-supplied cl::Image2D wrapper object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- A tensor descriptor object representing remote blob configuration

	*
		- ctx

		- A remote context used to create remote blob

	*
		- image

		- A cl::Image2D object wrapped by a remote blob



.. rubric:: Returns:

A remote blob instance

.. _doxid-namespace_inference_engine_1_1gpu_1acaa3dc7389d6fdfaa5452e08ba925489:
.. index:: pair: function; make_shared_blob_nv12

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` make_shared_blob_nv12(
		size_t height,
		size_t width,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		VASurfaceID nv12_surf
		)

This function is used to obtain a NV12 compound blob object from NV12 VA decoder output. The resulting compound contains two remote blobs for Y and UV planes of the surface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- height

		- A height of Y plane

	*
		- width

		- A width of Y plane

	*
		- ctx

		- A remote context instance

	*
		- nv12_surf

		- NV12 ``VASurfaceID`` to create NV12 from



.. rubric:: Returns:

A remote NV12 blob wrapping ``VASurfaceID``

.. _doxid-namespace_inference_engine_1_1gpu_1a251bc7130aab41116ebdccc9955a2bae:
.. index:: pair: function; make_shared_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`VAContext::Ptr<doxid-class_inference_engine_1_1gpu_1_1_v_a_context_1a618acae0ec67eddf09180c6af6ca343e>` make_shared_context(
		:ref:`Core<doxid-class_inference_engine_1_1_core>`& core,
		std::string deviceName,
		VADisplay device,
		int target_tile_id = -1
		)

This function is used to obtain remote context object from VA display handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` object

	*
		- deviceName

		- A device name to create a remote context for

	*
		- device

		- A ``VADisplay`` to create remote context from

	*
		- target_tile_id

		- Desired tile id within given context for multi-tile system. Default value (-1) means that root device should be used



.. rubric:: Returns:

A remote context wrapping ``VADisplay``

.. _doxid-namespace_inference_engine_1_1gpu_1a34c6c5f89430f39651644f76b52a0901:
.. index:: pair: function; make_shared_blob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`VASurfaceBlob::Ptr<doxid-class_inference_engine_1_1gpu_1_1_v_a_surface_blob_1a79c56780d0dd02794c837ccabbad4b3b>` make_shared_blob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` ctx,
		VASurfaceID surface,
		uint32_t plane = 0
		)

This function is used to obtain remote blob object from VA surface handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- Tensor descriptor

	*
		- ctx

		- A remote context instance

	*
		- surface

		- A ``VASurfaceID`` to create remote blob from

	*
		- plane

		- An index of a plane inside ``VASurfaceID`` to create blob from



.. rubric:: Returns:

A remote blob wrapping ``VASurfaceID``

