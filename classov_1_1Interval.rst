.. index:: pair: class; ov::Interval
.. _doxid-classov_1_1_interval:

class ov::Interval
==================



Overview
~~~~~~~~

:ref:`Interval <doxid-classov_1_1_interval>` arithmetic. :ref:`More...<details-classov_1_1_interval>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interval.hpp>
	
	class Interval
	{
	public:
		// typedefs
	
		typedef std::int64_t :target:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>`;
		typedef std::uint64_t :target:`size_type<doxid-classov_1_1_interval_1a4abb7913aa5f4353f12b57d41593f66f>`;

		// fields
	
		static constexpr :ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` :ref:`s_max<doxid-classov_1_1_interval_1a461591c80824cb147d31b81a6dca1727>` {std::numeric_limits<:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>`>::max()};

		// construction
	
		:ref:`Interval<doxid-classov_1_1_interval_1add1f107dede5bab2312ec74add2749bd>`();
		:ref:`Interval<doxid-classov_1_1_interval_1a94890d1a0c910509516d6e25df0dce52>`(const Interval& interval);
		:ref:`Interval<doxid-classov_1_1_interval_1afc10cf08dc138c2cbef5006355e79ca8>`(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` min_val, :ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` max_val);
		:ref:`Interval<doxid-classov_1_1_interval_1a7140e1f241f00a5c359d5ed5b2284b03>`(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` val);

		// methods
	
		Interval& :target:`operator =<doxid-classov_1_1_interval_1a293fb0a56e5f14f1f67a29c7cd59cff5>` (const Interval& interval);
		:ref:`size_type<doxid-classov_1_1_interval_1a4abb7913aa5f4353f12b57d41593f66f>` :ref:`size<doxid-classov_1_1_interval_1a23fdd239c4ef2b9d21c423fe3b665444>`() const;
		bool :ref:`empty<doxid-classov_1_1_interval_1a4e76e94f7617f9311f486b5c0d1263f2>`() const;
		:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` :ref:`get_min_val<doxid-classov_1_1_interval_1aa543a73c42779ed2085bd2131a8cb546>`() const;
		void :ref:`set_min_val<doxid-classov_1_1_interval_1aa5d56c74a3a2e1f4716a991b02a08b61>`(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` val);
		:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` :ref:`get_max_val<doxid-classov_1_1_interval_1acb777f7c6cf2323c3f2a04d1821be3cd>`() const;
		void :ref:`set_max_val<doxid-classov_1_1_interval_1a385fb349b66c60e3a80b1c916bec71db>`(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` val);
		bool :ref:`has_upper_bound<doxid-classov_1_1_interval_1a12ad3c8d1e627074b5997011a986bfe1>`() const;
		bool :ref:`operator ==<doxid-classov_1_1_interval_1ad0e5e866e926a53ace85b4e418c7680c>` (const Interval& interval) const;
		bool :target:`operator !=<doxid-classov_1_1_interval_1ac8836949e14c32e4de60dc41e48f50e2>` (const Interval& interval) const;
		Interval :ref:`operator +<doxid-classov_1_1_interval_1a25f256094456935fe2e37c2c772e0b82>` (const Interval& interval) const;
		Interval& :ref:`operator +=<doxid-classov_1_1_interval_1a4c9be1f7d36d5e62b13d575d509867e5>` (const Interval& interval);
		Interval :ref:`operator -<doxid-classov_1_1_interval_1a1fe3725da6b68a6de85e042ce7a11c05>` (const Interval& interval) const;
		Interval& :ref:`operator -=<doxid-classov_1_1_interval_1a01caa514192f67225d35ffe6cfbfd15b>` (const Interval& interval);
		Interval :ref:`operator\*<doxid-classov_1_1_interval_1ad69d7631987e4a9ffdb2189cbb2cd9cb>` (const Interval& interval) const;
		Interval& :ref:`operator\*=<doxid-classov_1_1_interval_1a05d7e86c0ccfd835705294442f73d4be>` (const Interval& interval);
		Interval :ref:`operator &<doxid-classov_1_1_interval_1af4161bcb62ec3ff9edc929528e94d8a5>` (const Interval& interval) const;
		Interval& :ref:`operator &=<doxid-classov_1_1_interval_1a4571c0a86e4a6b06d4454fa1a90e6436>` (const Interval& interval);
		bool :ref:`contains<doxid-classov_1_1_interval_1a74d5caff242fd9f155d484c40b21ec61>`(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` value) const;
		bool :ref:`contains<doxid-classov_1_1_interval_1ad5bde211f5e91a7b22b5915bf73e15e8>`(const Interval& interval) const;
	};
.. _details-classov_1_1_interval:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Interval <doxid-classov_1_1_interval>` arithmetic.

An interval is the set of integers from m_min_val through m_max_val. The value s_max acts like infinity. The addition, subtraction, or multiplication of intervals is the smallest interval containing the sums, differences, or products of elements of the two intervals. An empty interval is canonicalized to [s_max, s_max].

Fields
------

.. _doxid-classov_1_1_interval_1a461591c80824cb147d31b81a6dca1727:
.. index:: pair: variable; s_max

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` s_max {std::numeric_limits<:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>`>::max()}

The value used for no upper bound.

Construction
------------

.. _doxid-classov_1_1_interval_1add1f107dede5bab2312ec74add2749bd:
.. index:: pair: function; Interval

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval()

:ref:`Interval <doxid-classov_1_1_interval>` of everything.

.. _doxid-classov_1_1_interval_1a94890d1a0c910509516d6e25df0dce52:
.. index:: pair: function; Interval

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval(const Interval& interval)

Copy constructor.

.. _doxid-classov_1_1_interval_1afc10cf08dc138c2cbef5006355e79ca8:
.. index:: pair: function; Interval

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` min_val, :ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` max_val)

Closed interval {x|min_val <= x <= max_val}.

.. _doxid-classov_1_1_interval_1a7140e1f241f00a5c359d5ed5b2284b03:
.. index:: pair: function; Interval

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` val)

Single-valued interval; just contains val.

Methods
-------

.. _doxid-classov_1_1_interval_1a23fdd239c4ef2b9d21c423fe3b665444:
.. index:: pair: function; size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`size_type<doxid-classov_1_1_interval_1a4abb7913aa5f4353f12b57d41593f66f>` size() const

The number of elements in the interval. Zero if max < min.

.. _doxid-classov_1_1_interval_1a4e76e94f7617f9311f486b5c0d1263f2:
.. index:: pair: function; empty

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool empty() const

Returns true if the interval has no elements.

.. _doxid-classov_1_1_interval_1aa543a73c42779ed2085bd2131a8cb546:
.. index:: pair: function; get_min_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` get_min_val() const

the inclusive lower bound of the interval

.. _doxid-classov_1_1_interval_1aa5d56c74a3a2e1f4716a991b02a08b61:
.. index:: pair: function; set_min_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_min_val(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` val)

Set the inclusive lower bound of the interval.

.. _doxid-classov_1_1_interval_1acb777f7c6cf2323c3f2a04d1821be3cd:
.. index:: pair: function; get_max_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` get_max_val() const

the inclusive upper bound of the interval

.. _doxid-classov_1_1_interval_1a385fb349b66c60e3a80b1c916bec71db:
.. index:: pair: function; set_max_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_max_val(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` val)

Set the inclusive upper bound of the interval.

.. _doxid-classov_1_1_interval_1a12ad3c8d1e627074b5997011a986bfe1:
.. index:: pair: function; has_upper_bound

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has_upper_bound() const

True if the upper bound is finite.

.. _doxid-classov_1_1_interval_1ad0e5e866e926a53ace85b4e418c7680c:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const Interval& interval) const

True if min and max bounds match.

.. _doxid-classov_1_1_interval_1a25f256094456935fe2e37c2c772e0b82:
.. index:: pair: function; operator+

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval operator + (const Interval& interval) const

The interval whose elements are a sum of an element from each interval.

.. _doxid-classov_1_1_interval_1a4c9be1f7d36d5e62b13d575d509867e5:
.. index:: pair: function; operator+=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval& operator += (const Interval& interval)

Extend this interval to sums of elements in this interval and interval.

.. _doxid-classov_1_1_interval_1a1fe3725da6b68a6de85e042ce7a11c05:
.. index:: pair: function; operator-

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval operator - (const Interval& interval) const

The interval whose elements are a difference of an element from each interval.

.. _doxid-classov_1_1_interval_1a01caa514192f67225d35ffe6cfbfd15b:
.. index:: pair: function; operator-=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval& operator -= (const Interval& interval)

Extend this interval to differences of elements in this interval and interval.

.. _doxid-classov_1_1_interval_1ad69d7631987e4a9ffdb2189cbb2cd9cb:
.. index:: pair: function; operator\*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval operator\* (const Interval& interval) const

The smallest interval whose elements are a product of an element from each interval.

.. _doxid-classov_1_1_interval_1a05d7e86c0ccfd835705294442f73d4be:
.. index:: pair: function; operator\*=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval& operator\*= (const Interval& interval)

Extend this interval to products of elements in this interval and interval.

.. _doxid-classov_1_1_interval_1af4161bcb62ec3ff9edc929528e94d8a5:
.. index:: pair: function; operator&

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval operator & (const Interval& interval) const

The interval that is the intersection of this interval and interval.

.. _doxid-classov_1_1_interval_1a4571c0a86e4a6b06d4454fa1a90e6436:
.. index:: pair: function; operator&=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Interval& operator &= (const Interval& interval)

Change this interval to only include elements also in interval.

.. _doxid-classov_1_1_interval_1a74d5caff242fd9f155d484c40b21ec61:
.. index:: pair: function; contains

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool contains(:ref:`value_type<doxid-classov_1_1_interval_1ad9bf71005f9c818a404a436ce60ce23e>` value) const

True if this interval includes value.

.. _doxid-classov_1_1_interval_1ad5bde211f5e91a7b22b5915bf73e15e8:
.. index:: pair: function; contains

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool contains(const Interval& interval) const

True if this interval includes all the values in interval.


