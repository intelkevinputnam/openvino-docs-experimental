.. index:: pair: class; ov::intel_gpu::ocl::D3DContext
.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context:

class ov::intel_gpu::ocl::D3DContext
====================================



Overview
~~~~~~~~

This class represents an abstraction for GPU plugin remote context which is shared with Direct3D 11 device. The plugin object derived from this class can be obtained either with :ref:`CompiledModel::get_context() <doxid-classov_1_1_compiled_model_1a22c5537d4c7182072d327077c386b01a>` or :ref:`Core::create_context() <doxid-classov_1_1_core_1ab9a3eef07c3471037070242f8da2fb01>` calls. :ref:`More...<details-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <dx.hpp>
	
	class D3DContext: public :ref:`ov::intel_gpu::ocl::ClContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>`
	{
	public:
		// construction
	
		:ref:`D3DContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1af24250fbac9c328b96595174a7c6112c>`(:ref:`Core<doxid-classov_1_1_core>`& core, ID3D11Device \* device, int target_tile_id = -1);

		// methods
	
		static void :ref:`type_check<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1abfd59006febdfd8127be1fd0f9db3432>`(const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& remote_context);
		:ref:`operator ID3D11Device \*<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a3e3fa85f275eefad24819630c98e3445>` ();
	
		std::pair<:ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>`, :ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>`> :ref:`create_tensor_nv12<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1ab50f4af62627b17602fdf0e66ae86b73>`(
			const size_t height,
			const size_t width,
			ID3D11Texture2D \* nv12_surf
			);
	
		:ref:`D3DBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_buffer_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a20f1fdfe8e231908be276cec21253acc>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			ID3D11Buffer \* buffer
			);
	
		:ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a09d75802c95989ac5c5032297bbc8242>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			ID3D11Texture2D \* surface,
			uint32_t plane = 0
			);
	
		:ref:`ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1ad9eb11f702e791114f2dc591a3abcb16>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const cl_mem buffer
			);
	
		:ref:`ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a064ce2f07cccd8845e13d473d45e9466>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const cl::Buffer& buffer
			);
	
		:ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a99ddc6f9d614821708458e0dbfb2d808>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const cl::Image2D& image
			);
	
		:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a997927db9d05e8841dc9deca012446bf>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			void \* usm_ptr
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		:ref:`RemoteContext<doxid-classov_1_1_remote_context>`& :ref:`operator =<doxid-classov_1_1_remote_context_1a21458de48b8c09459af904e52211a821>` (const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& other);
		:ref:`RemoteContext<doxid-classov_1_1_remote_context>`& :ref:`operator =<doxid-classov_1_1_remote_context_1a7c57cd1cee1195ce0d0bd316db992d08>` (:ref:`RemoteContext<doxid-classov_1_1_remote_context>`&& other);
	
		template <typename T>
		bool :ref:`is<doxid-classov_1_1_remote_context_1ad266845dbe86f7a187b659a9a1980198>`() const;
	
		template <typename T>
		const T :ref:`as<doxid-classov_1_1_remote_context_1a54021126344109640e35a18842d22654>`() const;
	
		:ref:`RemoteTensor<doxid-classov_1_1_remote_tensor>` :ref:`create_tensor<doxid-classov_1_1_remote_context_1ac1735cf031cfde65e2ced782b21cc256>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& params = {}
			);
	
		:ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>` :ref:`get_params<doxid-classov_1_1_remote_context_1a45f1cad216e6d44b811b89b78fe4e638>`() const;
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`create_host_tensor<doxid-classov_1_1_remote_context_1a5cfbba2a531a15c4f778a7a72092f848>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
	
		static void :ref:`type_check<doxid-classov_1_1_remote_context_1a1ce9cb6cb79a4fcfc21f03a8ed7cd257>`(
			const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& remote_context,
			const std::map<std::string, std::vector<std::string>>& type_info = {}
			);
	
		static void :ref:`type_check<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1af5ef5dacdd4bee54ac98129b4f7332ad>`(const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& remote_context);
		cl_context :ref:`get<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a9a8d57332c8bb376487fe5b4a0bfb6fe>`();
		:ref:`operator cl_context<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1afb0985203306fa40fe0f99742cbb4b79>` ();
		:ref:`operator cl::Context<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a2a48a2c2502b707517b27d96f5639ccf>` ();
	
		std::pair<:ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>`, :ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>`> :ref:`create_tensor_nv12<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a5a65b26a953f2ca6da00ad1ae784fcca>`(
			const cl::Image2D& nv12_image_plane_y,
			const cl::Image2D& nv12_image_plane_uv
			);
	
		:ref:`ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1ad9eb11f702e791114f2dc591a3abcb16>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const cl_mem buffer
			);
	
		:ref:`ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a064ce2f07cccd8845e13d473d45e9466>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const cl::Buffer& buffer
			);
	
		:ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a99ddc6f9d614821708458e0dbfb2d808>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const cl::Image2D& image
			);
	
		:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a997927db9d05e8841dc9deca012446bf>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			void \* usm_ptr
			);
	
		:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` :ref:`create_usm_host_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a999a034cec4c5f002a72216e9fd51627>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
		:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` :ref:`create_usm_device_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a0024d67f70734abe2c9930c0a11d903e>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
	
		:ref:`RemoteTensor<doxid-classov_1_1_remote_tensor>` :ref:`create_tensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1ac1735cf031cfde65e2ced782b21cc256>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& params = {}
			);

.. _details-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an abstraction for GPU plugin remote context which is shared with Direct3D 11 device. The plugin object derived from this class can be obtained either with :ref:`CompiledModel::get_context() <doxid-classov_1_1_compiled_model_1a22c5537d4c7182072d327077c386b01a>` or :ref:`Core::create_context() <doxid-classov_1_1_core_1ab9a3eef07c3471037070242f8da2fb01>` calls.

User can also obtain OpenCL context handle from this class.

Construction
------------

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1af24250fbac9c328b96595174a7c6112c:
.. index:: pair: function; D3DContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	D3DContext(:ref:`Core<doxid-classov_1_1_core>`& core, ID3D11Device \* device, int target_tile_id = -1)

Constructs :ref:`D3DContext <doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context>` remote context object from ID3D11Device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- OpenVINO Runtime :ref:`Core <doxid-classov_1_1_core>` object instance

	*
		- device

		- A pointer to ID3D11Device to be used to create a remote context

	*
		- target_tile_id

		- Desired tile id within given context for multi-tile system. Default value (-1) means that root device should be used

Methods
-------

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1abfd59006febdfd8127be1fd0f9db3432:
.. index:: pair: function; type_check

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void type_check(const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& remote_context)

Checks that type defined runtime parameters are presented in remote object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- remote_context

		- A remote context to check

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a3e3fa85f275eefad24819630c98e3445:
.. index:: pair: function; operator ID3D11Device \*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator ID3D11Device \* ()

ID3D11Device conversion operator for the :ref:`D3DContext <doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context>` object.



.. rubric:: Returns:

Pointer to underlying ID3D11Device interface

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1ab50f4af62627b17602fdf0e66ae86b73:
.. index:: pair: function; create_tensor_nv12

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<:ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>`, :ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>`> create_tensor_nv12(
		const size_t height,
		const size_t width,
		ID3D11Texture2D \* nv12_surf
		)

This function is used to obtain a NV12 tensor from NV12 DXGI video decoder output. The resulting tensor contains two remote tensors for Y and UV planes of the surface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- height

		- Height of Y plane

	*
		- width

		- Width of Y plane

	*
		- nv12_surf

		- A ID3D11Texture2D instance to create NV12 tensor from



.. rubric:: Returns:

A pair of remote tensors for each plane

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a20f1fdfe8e231908be276cec21253acc:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`D3DBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_buffer_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		ID3D11Buffer \* buffer
		)

This function is used to obtain remote tensor object from ID3D11Buffer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- buffer

		- A pointer to ID3D11Buffer instance to create remote tensor based on



.. rubric:: Returns:

A remote tensor instance

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a09d75802c95989ac5c5032297bbc8242:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		ID3D11Texture2D \* surface,
		uint32_t plane = 0
		)

This function is used to obtain remote tensor object from ID3D11Texture2D.

The underlying ID3D11Texture2D can also be a plane of output surface of DXGI video decoder



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- surface

		- Pointer to ID3D11Texture2D interface of the objects that owns NV12 texture

	*
		- plane

		- ID of the plane to be shared (0 or 1)



.. rubric:: Returns:

:ref:`D3DSurface2DTensor <doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>` tensor

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1ad9eb11f702e791114f2dc591a3abcb16:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const cl_mem buffer
		)

This function is used to obtain remote tensor object from user-supplied cl_mem object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- buffer

		- A cl_mem object that should be wrapped by a remote tensor



.. rubric:: Returns:

A remote tensor instance

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a064ce2f07cccd8845e13d473d45e9466:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const cl::Buffer& buffer
		)

This function is used to obtain remote tensor object from user-supplied cl::Buffer object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- buffer

		- A cl::Buffer object that should be wrapped by a remote tensor



.. rubric:: Returns:

A remote tensor instance

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a99ddc6f9d614821708458e0dbfb2d808:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const cl::Image2D& image
		)

This function is used to obtain remote tensor object from user-supplied cl::Image2D object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- image

		- A cl::Image2D object that should be wrapped by a remote tensor



.. rubric:: Returns:

A remote tensor instance

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context_1a997927db9d05e8841dc9deca012446bf:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		void \* usm_ptr
		)

This function is used to obtain remote tensor object from user-supplied USM pointer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- usm_ptr

		- A USM pointer that should be wrapped by a remote tensor



.. rubric:: Returns:

A remote tensor instance


