.. index:: pair: class; InferenceEngine::Precision
.. _doxid-class_inference_engine_1_1_precision:

class InferenceEngine::Precision
================================

.. toctree::
	:hidden:

	ePrecision <enumInferenceEngine_1_1Precision_1_1ePrecision.rst>
	PrecisionInfo <structInferenceEngine_1_1Precision_1_1PrecisionInfo.rst>

Overview
~~~~~~~~

This class holds precision value and provides precision related operations. :ref:`More...<details-class_inference_engine_1_1_precision>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_precision.hpp>
	
	class Precision
	{
	public:
		// enums
	
		enum :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>`;

		// structs
	
		struct :ref:`PrecisionInfo<doxid-struct_inference_engine_1_1_precision_1_1_precision_info>`;

		// construction
	
		:ref:`Precision<doxid-class_inference_engine_1_1_precision_1a67ba42294fa19849af86a50b9d04d15f>`();
		:ref:`Precision<doxid-class_inference_engine_1_1_precision_1ae450b495a6d2e7361f9e944d3028f9bb>`(const :ref:`Precision::ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` value);
		:ref:`Precision<doxid-class_inference_engine_1_1_precision_1ab52d14199e87437f49e74c64a17a9770>`(size_t bitsSize, const char \* name = nullptr);

		// methods
	
		template <class T>
		bool :ref:`hasStorageType<doxid-class_inference_engine_1_1_precision_1a1f91074f540e6d21da96408988401e44>`(const char \* typeName = nullptr) const;
	
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_precision_1af2478e83d94c6299a59a6ac1fd964ba9>` (const Precision& p) const;
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_precision_1a09fc6d150059c81e73f60ce2f1d3eb09>` (const :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` p) const;
		bool :ref:`operator !=<doxid-class_inference_engine_1_1_precision_1a9ea497024c90df58ffd666d5cb81e4f9>` (const :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` p) const;
		Precision& :ref:`operator =<doxid-class_inference_engine_1_1_precision_1ab63fd020d439beda25171822e0f77316>` (const :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` p);
		:ref:`operator bool<doxid-class_inference_engine_1_1_precision_1a2d5f6eb8d115e2ac2cc0ee9264c72fc8>` () const;
		bool :ref:`operator !<doxid-class_inference_engine_1_1_precision_1a77f9ecf379dcd2aa62fefa75c1d82d92>` () const;
		:ref:`operator Precision::ePrecision<doxid-class_inference_engine_1_1_precision_1ad6e35e2c6c85972356b43f2c708382f6>` () const;
		constexpr uint8_t :ref:`getPrecVal<doxid-class_inference_engine_1_1_precision_1a9e79c12e1de354f45505f1b5c9c2a1f8>`() const;
		const char \* :ref:`name<doxid-class_inference_engine_1_1_precision_1ad7a09f00a9b6ea37010862b4e9920dfd>`() const;
		size_t :ref:`size<doxid-class_inference_engine_1_1_precision_1a08914efdabf29e5dee6332b6a3015383>`() const;
		size_t :ref:`bitsSize<doxid-class_inference_engine_1_1_precision_1a2b041b5289424fe9819db98885fac7d2>`() const;
		bool :ref:`is_float<doxid-class_inference_engine_1_1_precision_1a75120c3755cd82bca4218d61bae40248>`() const;
		bool :ref:`isSigned<doxid-class_inference_engine_1_1_precision_1afbfc1677ee6219eead50423fe00a6a10>`() const;
	
		template <class T>
		static Precision :ref:`fromType<doxid-class_inference_engine_1_1_precision_1a8075496ecb8be9312a27de00b5438f8d>`(const char \* typeName = nullptr);
	
		static Precision :ref:`FromStr<doxid-class_inference_engine_1_1_precision_1a1d04c5b1aa711d6859b123debedb6d82>`(const std::string& str);
	};
.. _details-class_inference_engine_1_1_precision:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class holds precision value and provides precision related operations.

Construction
------------

.. _doxid-class_inference_engine_1_1_precision_1a67ba42294fa19849af86a50b9d04d15f:
.. index:: pair: function; Precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Precision()

Default constructor.

.. _doxid-class_inference_engine_1_1_precision_1ae450b495a6d2e7361f9e944d3028f9bb:
.. index:: pair: function; Precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Precision(const :ref:`Precision::ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` value)

Constructor with specified precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- A value of ePrecision to create an object from

.. _doxid-class_inference_engine_1_1_precision_1ab52d14199e87437f49e74c64a17a9770:
.. index:: pair: function; Precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Precision(size_t bitsSize, const char \* name = nullptr)

Custom precision constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bitsSize

		- size of elements

	*
		- name

		- optional: name string, used in serialisation

Methods
-------

.. _doxid-class_inference_engine_1_1_precision_1a1f91074f540e6d21da96408988401e44:
.. index:: pair: function; hasStorageType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	bool hasStorageType(const char \* typeName = nullptr) const

checks whether given storage class T can be used to store objects of current precision



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- typeName

		- A string name of precision



.. rubric:: Returns:

``true`` if ``typeName`` has underlaying storage type

.. _doxid-class_inference_engine_1_1_precision_1af2478e83d94c6299a59a6ac1fd964ba9:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const Precision& p) const

Equality operator with :ref:`Precision <doxid-class_inference_engine_1_1_precision>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- A value of :ref:`Precision <doxid-class_inference_engine_1_1_precision>` to compare with



.. rubric:: Returns:

``true`` if values represent the same precisions, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1a09fc6d150059c81e73f60ce2f1d3eb09:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` p) const

Equality operator with ePrecision enum value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- A value of ePrecision to compare with



.. rubric:: Returns:

``true`` if values represent the same precisions, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1a9ea497024c90df58ffd666d5cb81e4f9:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` p) const

Inequality operator with ePrecision enum value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- A value of ePrecision to compare with



.. rubric:: Returns:

``true`` if values represent different precisions, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1ab63fd020d439beda25171822e0f77316:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Precision& operator = (const :ref:`ePrecision<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` p)

Assignment operator with ePrecision enum value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- A value of ePrecision enumeration



.. rubric:: Returns:

A :ref:`Precision <doxid-class_inference_engine_1_1_precision>` instance

.. _doxid-class_inference_engine_1_1_precision_1a2d5f6eb8d115e2ac2cc0ee9264c72fc8:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Cast operator to a bool.



.. rubric:: Returns:

``true`` if precision is specified, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1a77f9ecf379dcd2aa62fefa75c1d82d92:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Logical negation operator.



.. rubric:: Returns:

``true`` if precision is NOT specified, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1ad6e35e2c6c85972356b43f2c708382f6:
.. index:: pair: function; operator Precision::ePrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator Precision::ePrecision () const

Cast operator to a ePrecision.



.. rubric:: Returns:

A casted value of :ref:`Precision::ePrecision <doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>` enumeration

.. _doxid-class_inference_engine_1_1_precision_1a9e79c12e1de354f45505f1b5c9c2a1f8:
.. index:: pair: function; getPrecVal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr uint8_t getPrecVal() const

Gets the precision value of type ePrecision.



.. rubric:: Returns:

The preccision value.

.. _doxid-class_inference_engine_1_1_precision_1ad7a09f00a9b6ea37010862b4e9920dfd:
.. index:: pair: function; name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const char \* name() const

Getter of precision name.



.. rubric:: Returns:

A string representing precision name

.. _doxid-class_inference_engine_1_1_precision_1a08914efdabf29e5dee6332b6a3015383:
.. index:: pair: function; size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t size() const

Returns size of single element of that precision in bytes.



.. rubric:: Returns:

Number of bytes per element

.. _doxid-class_inference_engine_1_1_precision_1a2b041b5289424fe9819db98885fac7d2:
.. index:: pair: function; bitsSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t bitsSize() const

Returns size of single element of that precision in bits.



.. rubric:: Returns:

Number of bits per element

.. _doxid-class_inference_engine_1_1_precision_1a75120c3755cd82bca4218d61bae40248:
.. index:: pair: function; is_float

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_float() const

Checks if it is a floating point value.



.. rubric:: Returns:

True if precision is float point, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1afbfc1677ee6219eead50423fe00a6a10:
.. index:: pair: function; isSigned

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isSigned() const

Checks if it is a signed value.



.. rubric:: Returns:

True if precision is signed, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_precision_1a8075496ecb8be9312a27de00b5438f8d:
.. index:: pair: function; fromType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	static Precision fromType(const char \* typeName = nullptr)

Creates custom precision with specific underlined type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- typeName

		- A string name of precision



.. rubric:: Returns:

:ref:`Precision <doxid-class_inference_engine_1_1_precision>` converted from string name

.. _doxid-class_inference_engine_1_1_precision_1a1d04c5b1aa711d6859b123debedb6d82:
.. index:: pair: function; FromStr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static Precision FromStr(const std::string& str)

Creates :ref:`Precision <doxid-class_inference_engine_1_1_precision>` from string with precision name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- str

		- A string representing precision



.. rubric:: Returns:

:ref:`Precision <doxid-class_inference_engine_1_1_precision>` created from string representation


