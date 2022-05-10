.. index:: pair: class; ov::Dimension
.. _doxid-classov_1_1_dimension:

class ov::Dimension
===================



Overview
~~~~~~~~

Class representing a dimension, which may be dynamic (undetermined until runtime), in a shape or shape-like object. :ref:`More...<details-classov_1_1_dimension>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <dimension.hpp>
	
	class Dimension
	{
	public:
		// typedefs
	
		typedef int64_t :target:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>`;

		// construction
	
		:ref:`Dimension<doxid-classov_1_1_dimension_1a1c5b1183bde832d46aa4568d1e82ac75>`(:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` dimension);
		:ref:`Dimension<doxid-classov_1_1_dimension_1a982ddaa31c09c4a259e8a9e430b2f412>`(:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` min_dimension, :ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` max_dimension);
		:ref:`Dimension<doxid-classov_1_1_dimension_1ac302bc8b5a833366709b842a1d992c88>`();

		// methods
	
		bool :target:`operator ==<doxid-classov_1_1_dimension_1a48692b9dc9dbe14877cb0959d3f6bf0b>` (const Dimension& dimension) const;
		bool :target:`operator !=<doxid-classov_1_1_dimension_1aa145757db6b25e71ac4f2c62ba9f4c54>` (const Dimension& dimension) const;
		bool :ref:`is_static<doxid-classov_1_1_dimension_1a3dba0a54e648684e5d3290a9c9e2731c>`() const;
		bool :ref:`is_dynamic<doxid-classov_1_1_dimension_1ad3c9f93fdf64331c2d6bc8eb9eb884ed>`() const;
		:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` :ref:`get_length<doxid-classov_1_1_dimension_1a2107188aa66d1427a4bfb85a3ce89150>`() const;
		:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` :target:`get_min_length<doxid-classov_1_1_dimension_1a17d4e0073c6c4a971562728bb70f16a8>`() const;
		:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` :target:`get_max_length<doxid-classov_1_1_dimension_1a3c6b676598266de7a8c1769214e8effb>`() const;
		const :ref:`Interval<doxid-classov_1_1_interval>`& :ref:`get_interval<doxid-classov_1_1_dimension_1a0a95d35e9b42ec9eeb354d3f04c4dbe7>`() const;
		:ref:`Interval<doxid-classov_1_1_interval>`& :target:`get_interval<doxid-classov_1_1_dimension_1adfd4fb9969520e2b83c5dc5cec925540>`();
		bool :ref:`same_scheme<doxid-classov_1_1_dimension_1a8a463f7fdc62f36e22317d11b43d9f4c>`(const Dimension& dim) const;
		bool :ref:`compatible<doxid-classov_1_1_dimension_1a930fe268cb5c954ac8696c97a974ca5b>`(const Dimension& d) const;
		bool :ref:`relaxes<doxid-classov_1_1_dimension_1af86a6c838bde77d6b112f01b85b60d1e>`(const Dimension& d) const;
		bool :ref:`refines<doxid-classov_1_1_dimension_1a3c2e84dd061bbd2d6684093518a56b06>`(const Dimension& d) const;
		Dimension :ref:`operator +<doxid-classov_1_1_dimension_1a078b47506669183c8a363dd8207a934a>` (const Dimension& dim) const;
		Dimension :ref:`operator -<doxid-classov_1_1_dimension_1ab36cea5590691ab60110dfdc690e1c0c>` (const Dimension& dim) const;
		Dimension :ref:`operator/<doxid-classov_1_1_dimension_1af4eae9f53a49fcf263af5193517f8317>` (const :ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` divisor) const;
		Dimension& :ref:`operator/=<doxid-classov_1_1_dimension_1af19499a25249173cd62123b2797b46cb>` (const :ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` divisor);
		Dimension :ref:`operator\*<doxid-classov_1_1_dimension_1ac0ce753a03d8e2008a36c094d6476985>` (const Dimension& dim) const;
		Dimension& :ref:`operator +=<doxid-classov_1_1_dimension_1af354b2dcdefc57133ad10c8f2c77c592>` (const Dimension& dim);
		Dimension& :ref:`operator\*=<doxid-classov_1_1_dimension_1a8e0dd16a49df2ab309c27d3c84e005f3>` (const Dimension& dim);
		Dimension :ref:`operator &<doxid-classov_1_1_dimension_1ae7e99ad7f9bc9c37996f659c78a19c78>` (const Dimension& dim) const;
		Dimension& :ref:`operator &=<doxid-classov_1_1_dimension_1a0625ee3c0c1842f1d663422951dd6470>` (const Dimension& dim);
		static bool :ref:`merge<doxid-classov_1_1_dimension_1aef570cc1ebefa3e2b63fe91e4a600e5d>`(Dimension& dst, const Dimension& d1, const Dimension& d2);
	
		static bool :ref:`broadcast_merge<doxid-classov_1_1_dimension_1a9553bb0c9d092bce607de6be25a76bb4>`(
			Dimension& dst,
			const Dimension& d1,
			const Dimension& d2
			);
	
		static Dimension :ref:`dynamic<doxid-classov_1_1_dimension_1ae20d6e04468016921fc572308c712a20>`();
	};
.. _details-classov_1_1_dimension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class representing a dimension, which may be dynamic (undetermined until runtime), in a shape or shape-like object.

Static dimensions may be implicitly converted from value_type. A dynamic dimension is constructed with :ref:`Dimension() <doxid-classov_1_1_dimension_1ac302bc8b5a833366709b842a1d992c88>` or :ref:`Dimension::dynamic() <doxid-classov_1_1_dimension_1ae20d6e04468016921fc572308c712a20>`.

Construction
------------

.. _doxid-classov_1_1_dimension_1a1c5b1183bde832d46aa4568d1e82ac75:
.. index:: pair: function; Dimension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension(:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` dimension)

Construct a static dimension.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dimension

		- Value of the dimension.

.. _doxid-classov_1_1_dimension_1a982ddaa31c09c4a259e8a9e430b2f412:
.. index:: pair: function; Dimension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension(:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` min_dimension, :ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` max_dimension)

Construct a dynamic dimension with bounded range.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- min_dimension

		- The lower inclusive limit for the dimension

	*
		- max_dimension

		- The upper inclusive limit for the dimension

.. _doxid-classov_1_1_dimension_1ac302bc8b5a833366709b842a1d992c88:
.. index:: pair: function; Dimension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension()

Construct a dynamic dimension with range [0, ...].

Methods
-------

.. _doxid-classov_1_1_dimension_1a3dba0a54e648684e5d3290a9c9e2731c:
.. index:: pair: function; is_static

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_static() const

Check whether this dimension is static.



.. rubric:: Returns:

``true`` if the dimension is static, else ``false``.

.. _doxid-classov_1_1_dimension_1ad3c9f93fdf64331c2d6bc8eb9eb884ed:
.. index:: pair: function; is_dynamic

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_dynamic() const

Check whether this dimension is dynamic.



.. rubric:: Returns:

``false`` if the dimension is static, else ``true``.

.. _doxid-classov_1_1_dimension_1a2107188aa66d1427a4bfb85a3ce89150:
.. index:: pair: function; get_length

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` get_length() const

Convert this dimension to ``value_type``. This dimension must be static and non-negative.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::invalid_argument

		- If this dimension is dynamic or negative.

.. _doxid-classov_1_1_dimension_1a0a95d35e9b42ec9eeb354d3f04c4dbe7:
.. index:: pair: function; get_interval

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Interval<doxid-classov_1_1_interval>`& get_interval() const

Return the interval of valid lengths.

.. _doxid-classov_1_1_dimension_1a8a463f7fdc62f36e22317d11b43d9f4c:
.. index:: pair: function; same_scheme

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool same_scheme(const Dimension& dim) const

Check whether this dimension represents the same scheme as the argument (both dynamic, or equal).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dim

		- The other dimension to compare this dimension to.



.. rubric:: Returns:

``true`` if this dimension and ``dim`` are both dynamic, or if they are both static and equal; otherwise, ``false``.

.. _doxid-classov_1_1_dimension_1a930fe268cb5c954ac8696c97a974ca5b:
.. index:: pair: function; compatible

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool compatible(const Dimension& d) const

Check whether this dimension is capable of being merged with the argument dimension.

Two dimensions are considered compatible if it is possible to merge them. (See :ref:`Dimension::merge <doxid-classov_1_1_dimension_1aef570cc1ebefa3e2b63fe91e4a600e5d>`.)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- d

		- The dimension to compare this dimension with.



.. rubric:: Returns:

``true`` if this dimension is compatible with ``d``, else ``false``.

.. _doxid-classov_1_1_dimension_1af86a6c838bde77d6b112f01b85b60d1e:
.. index:: pair: function; relaxes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool relaxes(const Dimension& d) const

Check whether this dimension is a relaxation of the argument.

A dimension ``d1`` *relaxes* (or *is a relaxation of*) ``d2`` if ``d1`` and ``d2`` are static and equal, or ``d1`` is dynamic.

``d1.relaxes(d2)`` is equivalent to ``d2.refines(d1)``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- d

		- The dimension to compare this dimension with.



.. rubric:: Returns:

``true`` if this dimension relaxes ``d``, else ``false``.

.. _doxid-classov_1_1_dimension_1a3c2e84dd061bbd2d6684093518a56b06:
.. index:: pair: function; refines

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool refines(const Dimension& d) const

Check whether this dimension is a refinement of the argument.

A dimension ``d2`` *refines* (or *is a refinement of*) ``d1`` if ``d1`` and ``d2`` are static and equal, or ``d2`` is dynamic.

``d1.refines(d2)`` is equivalent to ``d2.relaxes(d1)``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- d

		- The dimension to compare this dimension with.



.. rubric:: Returns:

``true`` if this dimension relaxes ``d``, else ``false``.

.. _doxid-classov_1_1_dimension_1a078b47506669183c8a363dd8207a934a:
.. index:: pair: function; operator+

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension operator + (const Dimension& dim) const

Addition operator for :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dim

		- Right operand for addition.



.. rubric:: Returns:

Smallest interval dimension enclosing inputs

.. _doxid-classov_1_1_dimension_1ab36cea5590691ab60110dfdc690e1c0c:
.. index:: pair: function; operator-

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension operator - (const Dimension& dim) const

Subtraction operator for :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dim

		- Right operand for subtraction.



.. rubric:: Returns:

Smallest interval dimension enclosing inputs

.. _doxid-classov_1_1_dimension_1af4eae9f53a49fcf263af5193517f8317:
.. index:: pair: function; operator/

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension operator/ (const :ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` divisor) const

Division operator for :ref:`Dimension <doxid-classov_1_1_dimension>` divided by a value_type parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- divisor

		- Right operand for division.



.. rubric:: Returns:

Smallest interval dimension enclosing inputs

.. _doxid-classov_1_1_dimension_1af19499a25249173cd62123b2797b46cb:
.. index:: pair: function; operator/=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension& operator/= (const :ref:`value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>` divisor)

Divided-into operator for :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- divisor

		- Right operand for multiplication.



.. rubric:: Returns:

A reference to ``\*this``, after updating ``\*this`` to the value ``\*this \* dim``.

.. _doxid-classov_1_1_dimension_1ac0ce753a03d8e2008a36c094d6476985:
.. index:: pair: function; operator\*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension operator\* (const Dimension& dim) const

Multiplication operator for :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dim

		- Right operand for multiplicaiton.



.. rubric:: Returns:

Smallest interval containing all "produces" which are 0 if either of ``this`` or ``dim`` has length ``0``, else unbounded if either is unbounded, else product of lengths.

.. _doxid-classov_1_1_dimension_1af354b2dcdefc57133ad10c8f2c77c592:
.. index:: pair: function; operator+=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension& operator += (const Dimension& dim)

Add-into operator for :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dim

		- Right operand for addition.



.. rubric:: Returns:

A reference to ``\*this``, after updating ``\*this`` to the value ``\*this + dim``.

.. _doxid-classov_1_1_dimension_1a8e0dd16a49df2ab309c27d3c84e005f3:
.. index:: pair: function; operator\*=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension& operator\*= (const Dimension& dim)

Multiply-into operator for :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dim

		- Right operand for multiplication.



.. rubric:: Returns:

A reference to ``\*this``, after updating ``\*this`` to the value ``\*this \* dim``.

.. _doxid-classov_1_1_dimension_1ae7e99ad7f9bc9c37996f659c78a19c78:
.. index:: pair: function; operator&

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension operator & (const Dimension& dim) const

Intersection of dimensions.

.. _doxid-classov_1_1_dimension_1a0625ee3c0c1842f1d663422951dd6470:
.. index:: pair: function; operator&=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Dimension& operator &= (const Dimension& dim)

Intersection of dimensions.

.. _doxid-classov_1_1_dimension_1aef570cc1ebefa3e2b63fe91e4a600e5d:
.. index:: pair: function; merge

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool merge(Dimension& dst, const Dimension& d1, const Dimension& d2)

Try to merge two :ref:`Dimension <doxid-classov_1_1_dimension>` objects together.

* If ``d1`` is dynamic, writes ``d2`` to ``dst`` and returns ``true``.

* If ``d2`` is dynamic, writes ``d1`` to ``dst`` and returns ``true``.

* If ``d1`` and ``d2`` are static and equal, writes ``d1`` to ``dst`` and returns ``true``.

* If ``d1`` and ``d2`` are both static and unequal, leaves ``dst`` unchanged and returns ``false``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst

		- Reference to write the merged :ref:`Dimension <doxid-classov_1_1_dimension>` into.

	*
		- d1

		- First dimension to merge.

	*
		- d2

		- Second dimension to merge.



.. rubric:: Returns:

``true`` if merging succeeds, else ``false``.

.. _doxid-classov_1_1_dimension_1a9553bb0c9d092bce607de6be25a76bb4:
.. index:: pair: function; broadcast_merge

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool broadcast_merge(
		Dimension& dst,
		const Dimension& d1,
		const Dimension& d2
		)

Try to merge two :ref:`Dimension <doxid-classov_1_1_dimension>` objects together with implicit broadcasting of unit-sized dimension to non unit-sized dimension.

.. _doxid-classov_1_1_dimension_1ae20d6e04468016921fc572308c712a20:
.. index:: pair: function; dynamic

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static Dimension dynamic()

Create a dynamic dimension.



.. rubric:: Returns:

A dynamic dimension.


