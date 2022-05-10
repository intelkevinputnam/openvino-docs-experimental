.. index:: pair: class; ngraph::CoordinateTransformBasic
.. _doxid-classngraph_1_1_coordinate_transform_basic:

class ngraph::CoordinateTransformBasic
======================================



Overview
~~~~~~~~

Class which allows to calculate item index with given coordinates in tensor and helps to iterate over all coordinates. Tensor items should be placed in memory in row-major order. :ref:`More...<details-classngraph_1_1_coordinate_transform_basic>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <coordinate_transform.hpp>
	
	class CoordinateTransformBasic
	{
	public:
		// typedefs
	
		typedef :ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator>` :target:`Iterator<doxid-classngraph_1_1_coordinate_transform_basic_1ac5d0ae4424842e41f4161f827fd15e30>`;

		// construction
	
		:target:`CoordinateTransformBasic<doxid-classngraph_1_1_coordinate_transform_basic_1aecb2a54364e9785dc8a823cb1a3a1644>`(const Shape& source_shape);

		// methods
	
		size_t :ref:`index<doxid-classngraph_1_1_coordinate_transform_basic_1a93ac5a4ead81a70fca6b93bf1cd28240>`(const Coordinate& c) const;
		:ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator>` :ref:`begin<doxid-classngraph_1_1_coordinate_transform_basic_1a4b138f74f23baa6d32e28af8a22efee0>`() const;
		const :ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator>`& :ref:`end<doxid-classngraph_1_1_coordinate_transform_basic_1a1537adeb55d85716ff0503045f1ce8e2>`() const;
	};
.. _details-classngraph_1_1_coordinate_transform_basic:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class which allows to calculate item index with given coordinates in tensor and helps to iterate over all coordinates. Tensor items should be placed in memory in row-major order.

Methods
-------

.. _doxid-classngraph_1_1_coordinate_transform_basic_1a93ac5a4ead81a70fca6b93bf1cd28240:
.. index:: pair: function; index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t index(const Coordinate& c) const

The tensor element index calculation by given coordinate.

Deprecated



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- c

		- tensor element coordinate

.. _doxid-classngraph_1_1_coordinate_transform_basic_1a4b138f74f23baa6d32e28af8a22efee0:
.. index:: pair: function; begin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator>` begin() const

Returns an iterator to the first coordinate of the tensor.

.. _doxid-classngraph_1_1_coordinate_transform_basic_1a1537adeb55d85716ff0503045f1ce8e2:
.. index:: pair: function; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator>`& end() const

Returns an iterator to the coordinate following the last element of the tensor.


