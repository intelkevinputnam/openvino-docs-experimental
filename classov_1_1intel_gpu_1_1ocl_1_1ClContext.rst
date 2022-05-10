.. index:: pair: class; ov::intel_gpu::ocl::ClContext
.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context:

class ov::intel_gpu::ocl::ClContext
===================================



Overview
~~~~~~~~

This class represents an abstraction for GPU plugin remote context which is shared with OpenCL context object. The plugin object derived from this class can be obtained either with :ref:`CompiledModel::get_context() <doxid-classov_1_1_compiled_model_1a22c5537d4c7182072d327077c386b01a>` or :ref:`Core::create_context() <doxid-classov_1_1_core_1ab9a3eef07c3471037070242f8da2fb01>` calls. :ref:`More...<details-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ocl.hpp>
	
	class ClContext: public :ref:`ov::RemoteContext<doxid-classov_1_1_remote_context>`
	{
	public:
		// construction
	
		:ref:`ClContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1af57ac93a0bfc7a350447492f9eb81489>`(:ref:`Core<doxid-classov_1_1_core>`& core, cl_context ctx, int ctx_device_id = 0);
		:ref:`ClContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a9973f84c05650b4fcbf00d91c6394642>`(:ref:`Core<doxid-classov_1_1_core>`& core, cl_command_queue queue);

		// methods
	
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
	};

	// direct descendants

	class :ref:`D3DContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context>`;
	class :ref:`VAContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_v_a_context>`;

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

.. _details-classov_1_1intel__gpu_1_1ocl_1_1_cl_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an abstraction for GPU plugin remote context which is shared with OpenCL context object. The plugin object derived from this class can be obtained either with :ref:`CompiledModel::get_context() <doxid-classov_1_1_compiled_model_1a22c5537d4c7182072d327077c386b01a>` or :ref:`Core::create_context() <doxid-classov_1_1_core_1ab9a3eef07c3471037070242f8da2fb01>` calls.

Construction
------------

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1af57ac93a0bfc7a350447492f9eb81489:
.. index:: pair: function; ClContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClContext(:ref:`Core<doxid-classov_1_1_core>`& core, cl_context ctx, int ctx_device_id = 0)

Constructs context object from user-supplied OpenCL context handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- A reference to OpenVINO Runtime :ref:`Core <doxid-classov_1_1_core>` object

	*
		- ctx

		- A OpenCL context to be used to create shared remote context

	*
		- ctx_device_id

		- An ID of device to be used from ctx

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a9973f84c05650b4fcbf00d91c6394642:
.. index:: pair: function; ClContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClContext(:ref:`Core<doxid-classov_1_1_core>`& core, cl_command_queue queue)

Constructs context object from user-supplied OpenCL context handle.

Only latency mode is supported for such context sharing case.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- A reference to OpenVINO Runtime :ref:`Core <doxid-classov_1_1_core>` object

	*
		- queue

		- An OpenCL queue to be used to create shared remote context. Queue will be reused inside the plugin.

Methods
-------

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1af5ef5dacdd4bee54ac98129b4f7332ad:
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

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a9a8d57332c8bb376487fe5b4a0bfb6fe:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	cl_context get()

Returns the underlying OpenCL context handle.



.. rubric:: Returns:

``cl_context``

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1afb0985203306fa40fe0f99742cbb4b79:
.. index:: pair: function; operator cl_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator cl_context ()

OpenCL context handle conversion operator for the :ref:`ClContext <doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>` object.



.. rubric:: Returns:

``cl_context``

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a2a48a2c2502b707517b27d96f5639ccf:
.. index:: pair: function; operator cl::Context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator cl::Context ()

Standard Khronos cl::Context wrapper conversion operator for the :ref:`ClContext <doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>` object.



.. rubric:: Returns:

``cl::Context`` object

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a5a65b26a953f2ca6da00ad1ae784fcca:
.. index:: pair: function; create_tensor_nv12

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<:ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>`, :ref:`ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>`> create_tensor_nv12(
		const cl::Image2D& nv12_image_plane_y,
		const cl::Image2D& nv12_image_plane_uv
		)

This function is used to construct a NV12 compound tensor object from two cl::Image2D wrapper objects. The resulting compound contains two remote tensors for Y and UV planes of the surface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- nv12_image_plane_y

		- cl::Image2D object containing Y plane data.

	*
		- nv12_image_plane_uv

		- cl::Image2D object containing UV plane data.



.. rubric:: Returns:

A pair of remote tensors for each plane

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1ad9eb11f702e791114f2dc591a3abcb16:
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

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a064ce2f07cccd8845e13d473d45e9466:
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

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a99ddc6f9d614821708458e0dbfb2d808:
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

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a997927db9d05e8841dc9deca012446bf:
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

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a999a034cec4c5f002a72216e9fd51627:
.. index:: pair: function; create_usm_host_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` create_usm_host_tensor(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

This function is used to allocate USM tensor with host allocation type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape



.. rubric:: Returns:

A remote tensor instance

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1a0024d67f70734abe2c9930c0a11d903e:
.. index:: pair: function; create_usm_device_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>` create_usm_device_tensor(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

This function is used to allocate USM tensor with device allocation type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape



.. rubric:: Returns:

A remote tensor instance

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1ac1735cf031cfde65e2ced782b21cc256:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteTensor<doxid-classov_1_1_remote_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& params = {}
		)

Allocates memory tensor in device memory or wraps user-supplied memory handle using the specified tensor description and low-level device-specific parameters. Returns a pointer to the object that implements the :ref:`RemoteTensor <doxid-classov_1_1_remote_tensor>` interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Defines the element type of the tensor.

	*
		- shape

		- Defines the shape of the tensor.

	*
		- params

		- Map of the low-level tensor object parameters.



.. rubric:: Returns:

Pointer to a plugin object that implements the :ref:`RemoteTensor <doxid-classov_1_1_remote_tensor>` interface.


