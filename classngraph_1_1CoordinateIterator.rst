.. index:: pair: class; ngraph::CoordinateIterator
.. _doxid-classngraph_1_1_coordinate_iterator:

class ngraph::CoordinateIterator
================================



Overview
~~~~~~~~

A useful class that allows to iterate over the tensor coordinates. For example, for tensor with dimensions {2, 3} this iterator produces the following coordinates: {0,0}, {0,1}, {0,2}, {1,0}, {1,1}, {2,2}. :ref:`More...<details-classngraph_1_1_coordinate_iterator>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <coordinate_transform.hpp>
	
	class CoordinateIterator
	{
	public:
		// construction
	
		:ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator_1a2f466ef802d93bb058d7a5375ac865c0>`(const Shape& target_shape);

		// methods
	
		void :ref:`operator ++<doxid-classngraph_1_1_coordinate_iterator_1a710b037dc5c3358741ca7189ea116a78>` ();
		CoordinateIterator :ref:`operator ++<doxid-classngraph_1_1_coordinate_iterator_1a417a1f9a967045e93a729167d9ff35c9>` (int);
		void :ref:`operator +=<doxid-classngraph_1_1_coordinate_iterator_1ac227c1f9c2228dfdf030e6c9e53d1919>` (size_t n);
		const Coordinate& :ref:`operator\*<doxid-classngraph_1_1_coordinate_iterator_1a9edd00d49f24300a3b9cdbd40e158f40>` () const;
		bool :ref:`operator !=<doxid-classngraph_1_1_coordinate_iterator_1ac7738246ed64be0eb4ca7f79adbb5fc4>` (const CoordinateIterator& it) const;
		bool :ref:`operator ==<doxid-classngraph_1_1_coordinate_iterator_1add48fd55ab08309bf853b3b8a7dbdae4>` (const CoordinateIterator& it) const;
		size_t :ref:`advance<doxid-classngraph_1_1_coordinate_iterator_1aeff161f826ebae50cecb6e495a0ea02d>`(size_t axis);
		static const CoordinateIterator& :ref:`end<doxid-classngraph_1_1_coordinate_iterator_1a1e9d00a78bcaf533174bbc04f09ed64f>`();
	};
.. _details-classngraph_1_1_coordinate_iterator:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A useful class that allows to iterate over the tensor coordinates. For example, for tensor with dimensions {2, 3} this iterator produces the following coordinates: {0,0}, {0,1}, {0,2}, {1,0}, {1,1}, {2,2}.

Deprecated

Construction
------------

.. _doxid-classngraph_1_1_coordinate_iterator_1a2f466ef802d93bb058d7a5375ac865c0:
.. index:: pair: function; CoordinateIterator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CoordinateIterator(const Shape& target_shape)

Coordinates iterator constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- target_shape

		- The target shape for coordinates iteration

Methods
-------

.. _doxid-classngraph_1_1_coordinate_iterator_1a710b037dc5c3358741ca7189ea116a78:
.. index:: pair: function; operator++

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void operator ++ ()

The postfix operation increment the iterator by one.

.. _doxid-classngraph_1_1_coordinate_iterator_1a417a1f9a967045e93a729167d9ff35c9:
.. index:: pair: function; operator++

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CoordinateIterator operator ++ (int)

The prefix operation increment the iterator by one.

.. _doxid-classngraph_1_1_coordinate_iterator_1ac227c1f9c2228dfdf030e6c9e53d1919:
.. index:: pair: function; operator+=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void operator += (size_t n)

Increments iterator n times.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- n

		- number of elements it should be advanced

.. _doxid-classngraph_1_1_coordinate_iterator_1a9edd00d49f24300a3b9cdbd40e158f40:
.. index:: pair: function; operator\*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const Coordinate& operator\* () const

Iterator dereferencing operator returns reference to current pointed coordinate.

.. _doxid-classngraph_1_1_coordinate_iterator_1ac7738246ed64be0eb4ca7f79adbb5fc4:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const CoordinateIterator& it) const

Checks for iterator inequality.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- it

		- second iterator to compare

.. _doxid-classngraph_1_1_coordinate_iterator_1add48fd55ab08309bf853b3b8a7dbdae4:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const CoordinateIterator& it) const

Checks for iterator equality.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- it

		- second iterator to compare

.. _doxid-classngraph_1_1_coordinate_iterator_1aeff161f826ebae50cecb6e495a0ea02d:
.. index:: pair: function; advance

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t advance(size_t axis)

Increments iterator using specified axis of the shape n times.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- axis

		- index used for iteration

.. _doxid-classngraph_1_1_coordinate_iterator_1a1e9d00a78bcaf533174bbc04f09ed64f:
.. index:: pair: function; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const CoordinateIterator& end()

Useful function to build the last iterator. Returns a singleton that points to the last iterator.


