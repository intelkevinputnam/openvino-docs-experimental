.. index:: pair: class; ov::EnumMask
.. _doxid-classov_1_1_enum_mask:

class ov::EnumMask
==================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <enum_mask.hpp>
	
	template <typename T>
	class EnumMask
	{
	public:
		// typedefs
	
		typedef typename std::underlying_type<T>::type :ref:`value_type<doxid-classov_1_1_enum_mask_1ac30215c708e2eb875bc4d7550a4583c0>`;

		// construction
	
		:ref:`EnumMask<doxid-classov_1_1_enum_mask_1a41ece4c328aadfae404e84a53f365dd3>`();
		:target:`EnumMask<doxid-classov_1_1_enum_mask_1a25aefe4b0b9b1fdf07be598ce972c09b>`(const T& enum_value);
		:target:`EnumMask<doxid-classov_1_1_enum_mask_1aaaa3584402a5ffaa468574a4b0a0cab2>`(const EnumMask& other);
		:target:`EnumMask<doxid-classov_1_1_enum_mask_1a7f61ea286e2d73891e51a005ba6de6b9>`(std::initializer_list<T> enum_values);

		// methods
	
		:ref:`value_type<doxid-classov_1_1_enum_mask_1ac30215c708e2eb875bc4d7550a4583c0>` :target:`value<doxid-classov_1_1_enum_mask_1ae8c3b5372ac8142c504679067e0bcaf0>`() const;
		bool :ref:`is_any_set<doxid-classov_1_1_enum_mask_1a5b63fa12047e85420a8bd774b9bf1e28>`(const EnumMask& p) const;
		bool :ref:`is_set<doxid-classov_1_1_enum_mask_1add2a84d8977b175417ff1462d3b8a018>`(const EnumMask& p) const;
		bool :ref:`is_any_clear<doxid-classov_1_1_enum_mask_1a34b8b5e870ca987a7262c00d32e453b2>`(const EnumMask& p) const;
		bool :ref:`is_clear<doxid-classov_1_1_enum_mask_1a8795c9a1308f47c3d2cb8adefba46493>`(const EnumMask& p) const;
		void :target:`set<doxid-classov_1_1_enum_mask_1ae67a0ff45809b174850bf15927c9be24>`(const EnumMask& p);
		void :target:`clear<doxid-classov_1_1_enum_mask_1ad4899b85f2fa7a60ade969a20fad5612>`(const EnumMask& p);
		void :target:`clear_all<doxid-classov_1_1_enum_mask_1a95d03366501381ae76380f2bff11c19a>`();
		bool :target:`operator []<doxid-classov_1_1_enum_mask_1a2f04557851b0d3fed81a61d853ea5ecc>` (const EnumMask& p) const;
		bool :target:`operator ==<doxid-classov_1_1_enum_mask_1ad8917db63bcae79d1c9dc791f7b68e24>` (const EnumMask& other) const;
		bool :target:`operator !=<doxid-classov_1_1_enum_mask_1a0313f21e0f03f3ebeb9d1dbe369f772b>` (const EnumMask& other) const;
		EnumMask& :target:`operator =<doxid-classov_1_1_enum_mask_1aa75fda057a47dbcbd60cc862bba8347f>` (const EnumMask& other);
		EnumMask& :target:`operator &=<doxid-classov_1_1_enum_mask_1a70c96acb1df4c79571a03fc0c28ba242>` (const EnumMask& other);
		EnumMask& :target:`operator|=<doxid-classov_1_1_enum_mask_1a0b9bad1487b1dac0d287aa02b4cd6f1d>` (const EnumMask& other);
		EnumMask :target:`operator &<doxid-classov_1_1_enum_mask_1a657ed9dca550396b1afba5d8473f07e1>` (const EnumMask& other) const;
		EnumMask :target:`operator|<doxid-classov_1_1_enum_mask_1ae23c2ee4ea5509a2f61d5537fa9497f2>` (const EnumMask& other) const;
	};
.. _details-classov_1_1_enum_mask:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Typedefs
--------

.. _doxid-classov_1_1_enum_mask_1ac30215c708e2eb875bc4d7550a4583c0:
.. index:: pair: typedef; value_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef typename std::underlying_type<T>::type value_type

Make sure the template type is an enum.

Extract the underlying type of the enum.

Construction
------------

.. _doxid-classov_1_1_enum_mask_1a41ece4c328aadfae404e84a53f365dd3:
.. index:: pair: function; EnumMask

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	EnumMask()

Some bit operations are not safe for signed values, we require enum type to use unsigned underlying type.

Methods
-------

.. _doxid-classov_1_1_enum_mask_1a5b63fa12047e85420a8bd774b9bf1e28:
.. index:: pair: function; is_any_set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_any_set(const EnumMask& p) const

Check if any of the input parameter enum bit mask match.

.. _doxid-classov_1_1_enum_mask_1add2a84d8977b175417ff1462d3b8a018:
.. index:: pair: function; is_set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_set(const EnumMask& p) const

Check if all of the input parameter enum bit mask match.

.. _doxid-classov_1_1_enum_mask_1a34b8b5e870ca987a7262c00d32e453b2:
.. index:: pair: function; is_any_clear

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_any_clear(const EnumMask& p) const

Check if any of the input parameter enum bit mask does not match.

.. _doxid-classov_1_1_enum_mask_1a8795c9a1308f47c3d2cb8adefba46493:
.. index:: pair: function; is_clear

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_clear(const EnumMask& p) const

Check if all of the input parameter enum bit mask do not match.


