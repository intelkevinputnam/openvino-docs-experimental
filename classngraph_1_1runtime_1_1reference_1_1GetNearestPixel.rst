.. index:: pair: class; ngraph::runtime::reference::GetNearestPixel
.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel:

class ngraph::runtime::reference::GetNearestPixel
=================================================



Overview
~~~~~~~~

Calculation of nearest pixel. :ref:`More...<details-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	class GetNearestPixel
	{
	public:
		// construction
	
		:ref:`GetNearestPixel<doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel_1a71bb09528a5bdff9eb4a8c47ae9ce153>`();
		:ref:`GetNearestPixel<doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel_1aa1a35b895ca35e2399998fb77d262fc8>`(:ref:`Nearest_mode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>` mode);

		// methods
	
		int64_t :ref:`operator ()<doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel_1aa824565407a5497221e6d9cb6d6ed2e0>` (float original, bool is_downsample) const;
	};
.. _details-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Calculation of nearest pixel.

Construction
------------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel_1a71bb09528a5bdff9eb4a8c47ae9ce153:
.. index:: pair: function; GetNearestPixel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GetNearestPixel()

Constructs calculation of a nearest pixel in the default mode.

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel_1aa1a35b895ca35e2399998fb77d262fc8:
.. index:: pair: function; GetNearestPixel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GetNearestPixel(:ref:`Nearest_mode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>` mode)

Constructs calculation of nearest pixel for the specified mode.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- mode

		- the mode of the calculation of the nearest pixel

Methods
-------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel_1aa824565407a5497221e6d9cb6d6ed2e0:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t operator () (float original, bool is_downsample) const

Performing the nearest pixel calculation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- original

		- original coordinate

	*
		- is_downsample

		- true if it has downsample and false otherwise



.. rubric:: Returns:

the nearest pixel


