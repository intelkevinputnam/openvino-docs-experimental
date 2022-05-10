.. index:: pair: class; ov::element::Type
.. _doxid-classov_1_1element_1_1_type:

class ov::element::Type
=======================



Overview
~~~~~~~~

Base class to define element type. :ref:`More...<details-classov_1_1element_1_1_type>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <element_type.hpp>
	
	class Type
	{
	public:
		// construction
	
		:target:`Type<doxid-classov_1_1element_1_1_type_1afbadc9f94aeb4815a224726bde713fbb>`();
		:target:`Type<doxid-classov_1_1element_1_1_type_1a9c4db5a666c55a5bd3fccb94a9dc1fcf>`(const Type&);
		:target:`Type<doxid-classov_1_1element_1_1_type_1a377cbe539867a9f19a22d4ed38f4ad48>`(const :ref:`Type_t<doxid-group__ov__element__cpp__api_1gac13a83fdcf171bd2c98577bfcd37f2f1>` t);
	
		:target:`Type<doxid-classov_1_1element_1_1_type_1ab9b725c80270fad9ff47c0c0c7120c5e>`(
			size_t bitwidth,
			bool is_real,
			bool is_signed,
			bool is_quantized,
			const std::string& cname
			);

		// methods
	
		Type& :target:`operator =<doxid-classov_1_1element_1_1_type_1a0c1fc85b77fb452a031e64618c25aaa5>` (const Type&);
		std::string :target:`c_type_string<doxid-classov_1_1element_1_1_type_1a4c1eb9bf656bc797e4e619ee2aae94dd>`() const;
		size_t :target:`size<doxid-classov_1_1element_1_1_type_1a5e14ed0ad8e1347848975132be59d040>`() const;
		size_t :target:`hash<doxid-classov_1_1element_1_1_type_1a53b813bbdf285468414c2f1144ecf448>`() const;
		bool :target:`is_static<doxid-classov_1_1element_1_1_type_1a9e28313b12ecdf73e95580ef0f451ddc>`() const;
		bool :target:`is_dynamic<doxid-classov_1_1element_1_1_type_1a7fa0f5cb645bc6f7b32a37b918cbd5aa>`() const;
		bool :target:`is_real<doxid-classov_1_1element_1_1_type_1a956bdc19dae45442fb49ec2782531aa1>`() const;
		bool :target:`is_integral<doxid-classov_1_1element_1_1_type_1ab0972ab6ac27e06ad4deada0787d7eeb>`() const;
		bool :target:`is_integral_number<doxid-classov_1_1element_1_1_type_1aa15ff6feeee4796f2db153f16a704e12>`() const;
		bool :target:`is_signed<doxid-classov_1_1element_1_1_type_1a33098a503b94b7376a16451f4ed9a225>`() const;
		bool :target:`is_quantized<doxid-classov_1_1element_1_1_type_1ac075323ee1a967217fb037151ffbb8e6>`() const;
		size_t :target:`bitwidth<doxid-classov_1_1element_1_1_type_1a72b91e538b6d342dc17e9cfd5fc2e7d3>`() const;
		std::string :target:`get_type_name<doxid-classov_1_1element_1_1_type_1a66c557c56eeb46cf87c83fbb17319bbc>`() const;
		bool :ref:`compatible<doxid-classov_1_1element_1_1_type_1a3ae20156e347f316ce5df71967d63b25>`(const element::Type& t) const;
		constexpr :target:`operator Type_t<doxid-classov_1_1element_1_1_type_1aed758be053968b3f16c5afb6f38aedf1>` () const;
		static std::vector<const Type \*> :target:`get_known_types<doxid-classov_1_1element_1_1_type_1a2fee0bd8bfef2de8dbff0231eac2d3e7>`();
	
		static bool :ref:`merge<doxid-classov_1_1element_1_1_type_1a0b4953ef3da0ba04ada0fcfb77660657>`(
			element::Type& dst,
			const element::Type& t1,
			const element::Type& t2
			);
	};
.. _details-classov_1_1element_1_1_type:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Base class to define element type.

Methods
-------

.. _doxid-classov_1_1element_1_1_type_1a3ae20156e347f316ce5df71967d63b25:
.. index:: pair: function; compatible

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool compatible(const element::Type& t) const

Checks whether this element type is merge-compatible with ``t``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- t

		- The element type to compare this element type to.



.. rubric:: Returns:

``true`` if this element type is compatible with ``t``, else ``false``.

.. _doxid-classov_1_1element_1_1_type_1a0b4953ef3da0ba04ada0fcfb77660657:
.. index:: pair: function; merge

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool merge(
		element::Type& dst,
		const element::Type& t1,
		const element::Type& t2
		)

Merges two element types t1 and t2, writing the result into dst and returning true if successful, else returning false.

To "merge" two element types t1 and t2 is to find the least restrictive element type t that is no more restrictive than t1 and t2, if t exists. More simply:

merge(dst,element::Type::dynamic,t) writes t to dst and returns true

merge(dst,t,element::Type::dynamic) writes t to dst and returns true

merge(dst,t1,t2) where t1, t2 both static and equal writes t1 to dst and returns true

merge(dst,t1,t2) where t1, t2 both static and unequal does nothing to dst, and returns false


