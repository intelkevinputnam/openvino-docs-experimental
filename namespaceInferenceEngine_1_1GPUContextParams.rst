.. index:: pair: namespace; InferenceEngine::GPUContextParams
.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params:

namespace InferenceEngine::GPUContextParams
===========================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace GPUContextParams {

	// global variables

	static constexpr auto :ref:`PARAM_CONTEXT_TYPE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a04badc3a957c8aa6cceec70d55c6189a>` = "CONTEXT_TYPE";
	static constexpr auto :ref:`OCL<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a24e50dd3a975ccec46371cb8baa9e979>` = "OCL";
	static constexpr auto :ref:`VA_SHARED<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1accc2d22983891e59d43a4fc4eba66fe6>` = "VA_SHARED";
	static constexpr auto :ref:`PARAM_OCL_CONTEXT<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ae00420829497329cadbddc347e69f0e5>` = "OCL_CONTEXT";
	static constexpr auto :ref:`PARAM_OCL_CONTEXT_DEVICE_ID<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a02284c17e9907a367c6ea25c47cc994f>` = "OCL_CONTEXT_DEVICE_ID";
	static constexpr auto :ref:`PARAM_TILE_ID<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a03ae4cc0a4b76fa945b60d1012435fdd>` = "TILE_ID";
	static constexpr auto :ref:`PARAM_OCL_QUEUE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a6dac6977e1f28ad5928647b65df9b41d>` = "OCL_QUEUE";
	static constexpr auto :ref:`PARAM_VA_DEVICE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a320a7343be59b501f2fa17f4a2e2cce0>` = "VA_DEVICE";
	static constexpr auto :ref:`PARAM_SHARED_MEM_TYPE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ade7fa015841f88de851ed790004cfee0>` = "SHARED_MEM_TYPE";
	static constexpr auto :ref:`OCL_BUFFER<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ac78e60ec9864242f650a48598f7cbc55>` = "OCL_BUFFER";
	static constexpr auto :ref:`OCL_IMAGE2D<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ad3ec68bf906e71efe29b13d848d27eb0>` = "OCL_IMAGE2D";
	static constexpr auto :ref:`USM_USER_BUFFER<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a19476c8e3d61ce5cab785183ac528625>` = "USM_USER_BUFFER";
	static constexpr auto :ref:`USM_HOST_BUFFER<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a627bee54deddf187f43762530b31e34d>` = "USM_HOST_BUFFER";
	static constexpr auto :ref:`USM_DEVICE_BUFFER<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ae8f928a2bdb23154600a7c13c22ab781>` = "USM_DEVICE_BUFFER";
	static constexpr auto :ref:`VA_SURFACE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a51a1ec87eacefe713d218d35c6d82a5c>` = "VA_SURFACE";
	static constexpr auto :ref:`DX_BUFFER<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ac5d7caf31eb1b3f7b43c9ea460cf00cc>` = "DX_BUFFER";
	static constexpr auto :ref:`PARAM_MEM_HANDLE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1acb936d562fe6a05c4549f065a284ab5f>` = "MEM_HANDLE";
	static constexpr auto :ref:`PARAM_DEV_OBJECT_HANDLE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a9ed6e0256e8987e2dca7aac86e67e60a>` = "DEV_OBJECT_HANDLE";
	static constexpr auto :ref:`PARAM_VA_PLANE<doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ace0815c3ccc7a198e1b57375f0158236>` = "VA_PLANE";

	} // namespace GPUContextParams
.. _details-namespace_inference_engine_1_1_g_p_u_context_params:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Variables
----------------

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a04badc3a957c8aa6cceec70d55c6189a:
.. index:: pair: variable; PARAM_CONTEXT_TYPE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_CONTEXT_TYPE = "CONTEXT_TYPE"

Shared device context type: can be either pure OpenCL (OCL) or shared video decoder (VA_SHARED) context.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a24e50dd3a975ccec46371cb8baa9e979:
.. index:: pair: variable; OCL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto OCL = "OCL"

Pure OpenCL device context.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1accc2d22983891e59d43a4fc4eba66fe6:
.. index:: pair: variable; VA_SHARED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto VA_SHARED = "VA_SHARED"

Shared context (video decoder or D3D)

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ae00420829497329cadbddc347e69f0e5:
.. index:: pair: variable; PARAM_OCL_CONTEXT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_OCL_CONTEXT = "OCL_CONTEXT"

This key identifies OpenCL context handle in a shared context or shared memory blob parameter map.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a02284c17e9907a367c6ea25c47cc994f:
.. index:: pair: variable; PARAM_OCL_CONTEXT_DEVICE_ID

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_OCL_CONTEXT_DEVICE_ID = "OCL_CONTEXT_DEVICE_ID"

This key identifies ID of device in OpenCL context if multiple devices are present in the context.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a03ae4cc0a4b76fa945b60d1012435fdd:
.. index:: pair: variable; PARAM_TILE_ID

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_TILE_ID = "TILE_ID"

In case of multi-tile system, this key identifies tile within given context.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a6dac6977e1f28ad5928647b65df9b41d:
.. index:: pair: variable; PARAM_OCL_QUEUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_OCL_QUEUE = "OCL_QUEUE"

This key identifies OpenCL queue handle in a shared context.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a320a7343be59b501f2fa17f4a2e2cce0:
.. index:: pair: variable; PARAM_VA_DEVICE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_VA_DEVICE = "VA_DEVICE"

This key identifies video acceleration device/display handle in a shared context or shared memory blob parameter map.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ade7fa015841f88de851ed790004cfee0:
.. index:: pair: variable; PARAM_SHARED_MEM_TYPE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_SHARED_MEM_TYPE = "SHARED_MEM_TYPE"

This key identifies type of internal shared memory in a shared memory blob parameter map.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ac78e60ec9864242f650a48598f7cbc55:
.. index:: pair: variable; OCL_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto OCL_BUFFER = "OCL_BUFFER"

Shared OpenCL buffer blob.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ad3ec68bf906e71efe29b13d848d27eb0:
.. index:: pair: variable; OCL_IMAGE2D

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto OCL_IMAGE2D = "OCL_IMAGE2D"

Shared OpenCL 2D image blob.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a19476c8e3d61ce5cab785183ac528625:
.. index:: pair: variable; USM_USER_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto USM_USER_BUFFER = "USM_USER_BUFFER"

Shared USM pointer allocated by user.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a627bee54deddf187f43762530b31e34d:
.. index:: pair: variable; USM_HOST_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto USM_HOST_BUFFER = "USM_HOST_BUFFER"

Shared USM pointer type with host allocation type allocated by plugin.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ae8f928a2bdb23154600a7c13c22ab781:
.. index:: pair: variable; USM_DEVICE_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto USM_DEVICE_BUFFER = "USM_DEVICE_BUFFER"

Shared USM pointer type with device allocation type allocated by plugin.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a51a1ec87eacefe713d218d35c6d82a5c:
.. index:: pair: variable; VA_SURFACE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto VA_SURFACE = "VA_SURFACE"

Shared video decoder surface or D3D 2D texture blob.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ac5d7caf31eb1b3f7b43c9ea460cf00cc:
.. index:: pair: variable; DX_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto DX_BUFFER = "DX_BUFFER"

Shared D3D buffer blob.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1acb936d562fe6a05c4549f065a284ab5f:
.. index:: pair: variable; PARAM_MEM_HANDLE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_MEM_HANDLE = "MEM_HANDLE"

This key identifies OpenCL memory handle in a shared memory blob parameter map.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1a9ed6e0256e8987e2dca7aac86e67e60a:
.. index:: pair: variable; PARAM_DEV_OBJECT_HANDLE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_DEV_OBJECT_HANDLE = "DEV_OBJECT_HANDLE"

This key identifies video decoder surface handle in a shared memory blob parameter map.

.. _doxid-namespace_inference_engine_1_1_g_p_u_context_params_1ace0815c3ccc7a198e1b57375f0158236:
.. index:: pair: variable; PARAM_VA_PLANE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto PARAM_VA_PLANE = "VA_PLANE"

This key identifies video decoder surface plane in a shared memory blob parameter map.

