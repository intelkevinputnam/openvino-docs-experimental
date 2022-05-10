.. index:: pair: class; ngraph::runtime::reference::GetOriginalCoordinate
.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate:

class ngraph::runtime::reference::GetOriginalCoordinate
=======================================================



Overview
~~~~~~~~

Calculation of the source coordinate using the resized coordinate. :ref:`More...<details-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	class GetOriginalCoordinate
	{
	public:
		// construction
	
		:ref:`GetOriginalCoordinate<doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate_1a8356e66200a3168517cba801724ae1ff>`();
		:ref:`GetOriginalCoordinate<doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate_1a43cb7d25acf0acc8b6ad8dcb8ec286bc>`(:ref:`Transform_mode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>` mode);

		// methods
	
		float :ref:`operator ()<doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate_1a00a9ed0078bebeb677eb4f5e534ec160>` (
			float x_resized,
			float x_scale,
			float length_resized,
			float length_original
			) const;
	};
.. _details-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Calculation of the source coordinate using the resized coordinate.

Construction
------------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate_1a8356e66200a3168517cba801724ae1ff:
.. index:: pair: function; GetOriginalCoordinate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GetOriginalCoordinate()

Constructs calculation of a nearest pixel in the default mode.

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate_1a43cb7d25acf0acc8b6ad8dcb8ec286bc:
.. index:: pair: function; GetOriginalCoordinate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GetOriginalCoordinate(:ref:`Transform_mode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>` mode)

Constructs calculation of the source coordinate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- mode

		- the mode of the calculation of the source coordinate.

Methods
-------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate_1a00a9ed0078bebeb677eb4f5e534ec160:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float operator () (
		float x_resized,
		float x_scale,
		float length_resized,
		float length_original
		) const

Performing the source coordinate calculation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- x_resized

		- resized coordinate

	*
		- x_scale

		- scale for the considered axis

	*
		- length_resized

		- length of the resized axis

	*
		- length_original

		- original length of the axis



.. rubric:: Returns:

the source coordinate


