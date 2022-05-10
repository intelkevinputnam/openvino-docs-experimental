.. index:: pair: group; Intel GPU OpenCL interoperability
.. _doxid-group__ov__runtime__ocl__gpu__cpp__api:

Intel GPU OpenCL interoperability
=================================

.. toctree::
	:hidden:

	ContextType <enumov_1_1intel_gpu_1_1ContextType.rst>
	SharedMemType <enumov_1_1intel_gpu_1_1SharedMemType.rst>
	ClBufferTensor <classov_1_1intel_gpu_1_1ocl_1_1ClBufferTensor.rst>
	ClContext <classov_1_1intel_gpu_1_1ocl_1_1ClContext.rst>
	ClImage2DTensor <classov_1_1intel_gpu_1_1ocl_1_1ClImage2DTensor.rst>
	D3DBufferTensor <classov_1_1intel_gpu_1_1ocl_1_1D3DBufferTensor.rst>
	D3DContext <classov_1_1intel_gpu_1_1ocl_1_1D3DContext.rst>
	D3DSurface2DTensor <classov_1_1intel_gpu_1_1ocl_1_1D3DSurface2DTensor.rst>
	USMTensor <classov_1_1intel_gpu_1_1ocl_1_1USMTensor.rst>
	VAContext <classov_1_1intel_gpu_1_1ocl_1_1VAContext.rst>
	VASurfaceTensor <classov_1_1intel_gpu_1_1ocl_1_1VASurfaceTensor.rst>

Overview
~~~~~~~~

Set of C++ classes and properties to work with Remote API for Intel GPU OpenCL plugin. :ref:`More...<details-group__ov__runtime__ocl__gpu__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// typedefs

	typedef void \* :ref:`ov::intel_gpu::ocl::gpu_handle_param<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga15a4712a2261ea1ceb5f68d582bcfaac>`;

	// enums

	enum :ref:`ov::intel_gpu::ContextType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b>`;
	enum :ref:`ov::intel_gpu::SharedMemType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491>`;

	// classes

	class :ref:`ov::intel_gpu::ocl::ClBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor>`;
	class :ref:`ov::intel_gpu::ocl::ClContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>`;
	class :ref:`ov::intel_gpu::ocl::ClImage2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>`;
	class :ref:`ov::intel_gpu::ocl::D3DBufferTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_buffer_tensor>`;
	class :ref:`ov::intel_gpu::ocl::D3DContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context>`;
	class :ref:`ov::intel_gpu::ocl::D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>`;
	class :ref:`ov::intel_gpu::ocl::USMTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor>`;
	class :ref:`ov::intel_gpu::ocl::VAContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_v_a_context>`;
	class :ref:`ov::intel_gpu::ocl::VASurfaceTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_v_a_surface_tensor>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ContextType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b>`> :ref:`ov::intel_gpu::context_type<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga79db7ddeadb921be11875f65aab4fa97>` {"CONTEXT_TYPE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ov::intel_gpu::ocl_context<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga603300e0890eacc6a72b653f922a9b17>` {"OCL_CONTEXT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int> :ref:`ov::intel_gpu::ocl_context_device_id<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gaaef948041b53eca18f873d90423028a4>` {"OCL_CONTEXT_DEVICE_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int> :ref:`ov::intel_gpu::tile_id<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga0809250f740b2d33b1c036a508b709dd>` {"TILE_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ov::intel_gpu::ocl_queue<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga293347d96f2828219be99e2796d5a58d>` {"OCL_QUEUE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ov::intel_gpu::va_device<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gaead16bba9c3e710a5bbc37a3d7ec131e>` {"VA_DEVICE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`SharedMemType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491>`> :ref:`ov::intel_gpu::shared_mem_type<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gad1d680fdc8440d41b4106d6e0fbbf66d>` {"SHARED_MEM_TYPE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ov::intel_gpu::mem_handle<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga802dc72abf97bd4fbad889b55ac659e8>` {"MEM_HANDLE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ov::intel_gpu::dev_object_handle<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga821530fcff2dba9aaaab557cffaf7955>` {"DEV_OBJECT_HANDLE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t> :ref:`ov::intel_gpu::va_plane<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gab033a8e885c875bef228ad92a79d32fc>` {"VA_PLANE"};

.. _details-group__ov__runtime__ocl__gpu__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of C++ classes and properties to work with Remote API for Intel GPU OpenCL plugin.

Typedefs
--------

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga15a4712a2261ea1ceb5f68d582bcfaac:
.. index:: pair: typedef; gpu_handle_param

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef void \* ov::intel_gpu::ocl::gpu_handle_param

Shortcut for defining a handle parameter.

Global Variables
----------------

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga79db7ddeadb921be11875f65aab4fa97:
.. index:: pair: variable; context_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ContextType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b>`> ov::intel_gpu::context_type {"CONTEXT_TYPE"}

Shared device context type: can be either pure OpenCL (OCL) or shared video decoder (VA_SHARED) context.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga603300e0890eacc6a72b653f922a9b17:
.. index:: pair: variable; ocl_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> ov::intel_gpu::ocl_context {"OCL_CONTEXT"}

This key identifies OpenCL context handle in a shared context or shared memory blob parameter map.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gaaef948041b53eca18f873d90423028a4:
.. index:: pair: variable; ocl_context_device_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int> ov::intel_gpu::ocl_context_device_id {"OCL_CONTEXT_DEVICE_ID"}

This key identifies ID of device in OpenCL context if multiple devices are present in the context.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga0809250f740b2d33b1c036a508b709dd:
.. index:: pair: variable; tile_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int> ov::intel_gpu::tile_id {"TILE_ID"}

In case of multi-tile system, this key identifies tile within given context.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga293347d96f2828219be99e2796d5a58d:
.. index:: pair: variable; ocl_queue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> ov::intel_gpu::ocl_queue {"OCL_QUEUE"}

This key identifies OpenCL queue handle in a shared context.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gaead16bba9c3e710a5bbc37a3d7ec131e:
.. index:: pair: variable; va_device

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> ov::intel_gpu::va_device {"VA_DEVICE"}

This key identifies video acceleration device/display handle in a shared context or shared memory blob parameter map.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gad1d680fdc8440d41b4106d6e0fbbf66d:
.. index:: pair: variable; shared_mem_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`SharedMemType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491>`> ov::intel_gpu::shared_mem_type {"SHARED_MEM_TYPE"}

This key identifies type of internal shared memory in a shared memory blob parameter map.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga802dc72abf97bd4fbad889b55ac659e8:
.. index:: pair: variable; mem_handle

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> ov::intel_gpu::mem_handle {"MEM_HANDLE"}

This key identifies OpenCL memory handle in a shared memory blob parameter map.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga821530fcff2dba9aaaab557cffaf7955:
.. index:: pair: variable; dev_object_handle

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> ov::intel_gpu::dev_object_handle {"DEV_OBJECT_HANDLE"}

This key identifies video decoder surface handle in a shared memory blob parameter map.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gab033a8e885c875bef228ad92a79d32fc:
.. index:: pair: variable; va_plane

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t> ov::intel_gpu::va_plane {"VA_PLANE"}

This key identifies video decoder surface plane in a shared memory blob parameter map.

