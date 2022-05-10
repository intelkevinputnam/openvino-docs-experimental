.. index:: pair: enum; SharedMemType
.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491:

enum ov::intel_gpu::SharedMemType
=================================

Overview
~~~~~~~~

Enum to define the type of the shared memory buffer. :ref:`More...<details-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <remote_properties.hpp>

	enum SharedMemType
	{
	    :ref:`OCL_BUFFER<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491af0d4cbbb2c5052481ccee69705098ef3>`        = 0,
	    :ref:`OCL_IMAGE2D<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491ab9695d2a64444daa22223ff3b0050005>`       = 1,
	    :ref:`USM_USER_BUFFER<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a78fc7d3e6b40730cddb406b66c11ec2c>`   = 2,
	    :ref:`USM_HOST_BUFFER<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491ac46e477c002123df1d4124ea739dccfc>`   = 3,
	    :ref:`USM_DEVICE_BUFFER<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a9241de34fae91bfb8f9dc05b1f2ed682>` = 4,
	    :ref:`VA_SURFACE<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a1dc1d7da09640f0f082a1957ce4aa1f7>`        = 5,
	    :ref:`DX_BUFFER<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a6d8338cb672f5a755880c0cdc5771798>`         = 6,
	};

.. _details-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define the type of the shared memory buffer.

Enum Values
-----------

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491af0d4cbbb2c5052481ccee69705098ef3:
.. index:: pair: enumvalue; OCL_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OCL_BUFFER

Shared OpenCL buffer blob.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491ab9695d2a64444daa22223ff3b0050005:
.. index:: pair: enumvalue; OCL_IMAGE2D

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OCL_IMAGE2D

Shared OpenCL 2D image blob.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a78fc7d3e6b40730cddb406b66c11ec2c:
.. index:: pair: enumvalue; USM_USER_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	USM_USER_BUFFER

Shared USM pointer allocated by user.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491ac46e477c002123df1d4124ea739dccfc:
.. index:: pair: enumvalue; USM_HOST_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	USM_HOST_BUFFER

Shared USM pointer type with host allocation type allocated by plugin.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a9241de34fae91bfb8f9dc05b1f2ed682:
.. index:: pair: enumvalue; USM_DEVICE_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	USM_DEVICE_BUFFER

Shared USM pointer type with device allocation type allocated by plugin.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a1dc1d7da09640f0f082a1957ce4aa1f7:
.. index:: pair: enumvalue; VA_SURFACE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VA_SURFACE

Shared video decoder surface or D3D 2D texture blob.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga887d079a3a8ffaa6d75aeb28c0fb3491a6d8338cb672f5a755880c0cdc5771798:
.. index:: pair: enumvalue; DX_BUFFER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DX_BUFFER

Shared D3D buffer blob.

