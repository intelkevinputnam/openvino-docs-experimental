.. index:: pair: enum; ContextType
.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b:

enum ov::intel_gpu::ContextType
===============================

Overview
~~~~~~~~

Enum to define the type of the shared context. :ref:`More...<details-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <remote_properties.hpp>

	enum ContextType
	{
	    :ref:`OCL<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga3d30ef6bfc7628812b855ca2031ce01bae403d567d72bb88201223ceb860f58ae>`       = 0,
	    :ref:`VA_SHARED<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga3d30ef6bfc7628812b855ca2031ce01baf18a61f262883539ec5118f9ed3c8963>` = 1,
	};

.. _details-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define the type of the shared context.

Enum Values
-----------

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga3d30ef6bfc7628812b855ca2031ce01bae403d567d72bb88201223ceb860f58ae:
.. index:: pair: enumvalue; OCL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OCL

Pure OpenCL context.

.. _doxid-group__ov__runtime__ocl__gpu__cpp__api_1gga3d30ef6bfc7628812b855ca2031ce01baf18a61f262883539ec5118f9ed3c8963:
.. index:: pair: enumvalue; VA_SHARED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VA_SHARED

Context shared with a video decoding device.

