.. index:: pair: struct; InferenceEngine::ROI
.. _doxid-struct_inference_engine_1_1_r_o_i:

struct InferenceEngine::ROI
===========================



Overview
~~~~~~~~

This structure describes :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` data for image-like tensors. :ref:`More...<details-struct_inference_engine_1_1_r_o_i>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layouts.h>
	
	struct ROI
	{
		// fields
	
		size_t :ref:`id<doxid-struct_inference_engine_1_1_r_o_i_1ab1deb8250a75e03506600d13045d0af1>` = 0;
		size_t :ref:`posX<doxid-struct_inference_engine_1_1_r_o_i_1afcf702ce814f3e24bf2a4e0edf2d2ce3>` = 0;
		size_t :ref:`posY<doxid-struct_inference_engine_1_1_r_o_i_1a11285002c451b43581c262d1ef556dee>` = 0;
		size_t :ref:`sizeX<doxid-struct_inference_engine_1_1_r_o_i_1a06ab26eda0f2fde468cd24a3505799ac>` = 0;
		size_t :ref:`sizeY<doxid-struct_inference_engine_1_1_r_o_i_1af2744a5cc139ac37ecdb954cb114da7c>` = 0;

		// construction
	
		:target:`ROI<doxid-struct_inference_engine_1_1_r_o_i_1a5e13799cda466e8a00245c31c937e2c2>`();
		:ref:`ROI<doxid-struct_inference_engine_1_1_r_o_i_1a0610da832bc7735748d3212b9236c335>`(size_t id, size_t posX, size_t posY, size_t sizeX, size_t sizeY);
	};
.. _details-struct_inference_engine_1_1_r_o_i:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This structure describes :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` data for image-like tensors.

Fields
------

.. _doxid-struct_inference_engine_1_1_r_o_i_1ab1deb8250a75e03506600d13045d0af1:
.. index:: pair: variable; id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t id = 0

ID of a :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` (offset over batch dimension)

.. _doxid-struct_inference_engine_1_1_r_o_i_1afcf702ce814f3e24bf2a4e0edf2d2ce3:
.. index:: pair: variable; posX

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t posX = 0

W upper left coordinate of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`.

.. _doxid-struct_inference_engine_1_1_r_o_i_1a11285002c451b43581c262d1ef556dee:
.. index:: pair: variable; posY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t posY = 0

H upper left coordinate of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`.

.. _doxid-struct_inference_engine_1_1_r_o_i_1a06ab26eda0f2fde468cd24a3505799ac:
.. index:: pair: variable; sizeX

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t sizeX = 0

W size of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`.

.. _doxid-struct_inference_engine_1_1_r_o_i_1af2744a5cc139ac37ecdb954cb114da7c:
.. index:: pair: variable; sizeY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t sizeY = 0

H size of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`.

Construction
------------

.. _doxid-struct_inference_engine_1_1_r_o_i_1a0610da832bc7735748d3212b9236c335:
.. index:: pair: function; ROI

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ROI(size_t id, size_t posX, size_t posY, size_t sizeX, size_t sizeY)

Creates a :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` objects with given parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- id

		- ID of a :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` (offset over batch dimension)

	*
		- posX

		- W upper left coordinate of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`

	*
		- posY

		- H upper left coordinate of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`

	*
		- sizeX

		- W size of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`

	*
		- sizeY

		- H size of :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>`


