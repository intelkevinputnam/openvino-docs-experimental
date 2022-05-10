.. index:: pair: group; FP16 to FP32 precision utilities
.. _doxid-group__ie__dev__api__precision:

FP16 to FP32 precision utilities
================================

.. toctree::
	:hidden:

	PrecisionUtils <namespaceInferenceEngine_1_1PrecisionUtils.rst>

Overview
~~~~~~~~

Set of functions to convert from FP32 to FP16 and vice versa. :ref:`More...<details-group__ie__dev__api__precision>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`InferenceEngine::PrecisionUtils<doxid-namespace_inference_engine_1_1_precision_utils>`;
		namespace :ref:`InferenceEngine::PrecisionUtils::details<doxid-namespace_inference_engine_1_1_precision_utils_1_1details>`;

	// typedefs

	typedef short :ref:`InferenceEngine::ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>`;

	// global functions

	:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` :ref:`InferenceEngine::PrecisionUtils::f32tof16<doxid-group__ie__dev__api__precision_1ga4669263097f51520c2f2f62c44d7bb65>`(float x);
	float :ref:`InferenceEngine::PrecisionUtils::f16tof32<doxid-group__ie__dev__api__precision_1ga13155ccd32a9c8ecca615eef89af3f5d>`(:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` x);

	void :ref:`InferenceEngine::PrecisionUtils::f16tof32Arrays<doxid-group__ie__dev__api__precision_1ga9b3a5d90bb1d3439dddf758af1035ffe>`(
		float \* dst,
		const :ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` \* src,
		size_t nelem,
		float scale = 1.f,
		float bias = 0.f
		);

	void :ref:`InferenceEngine::PrecisionUtils::f32tof16Arrays<doxid-group__ie__dev__api__precision_1gaa08cea0abc12560240b4f8c5c168ac75>`(
		:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` \* dst,
		const float \* src,
		size_t nelem,
		float scale = 1.f,
		float bias = 0.f
		);

	template <
		class OutT,
		class InT,
		typename std::enable_if<std::is_integral<OutT>::value&&std::is_integral<InT>::value&&std::is_signed<InT>::value&&!std::is_same<OutT, InT>::value>::type \* = nullptr
		>
	OutT :ref:`InferenceEngine::PrecisionUtils::saturate_cast<doxid-group__ie__dev__api__precision_1ga38df1785fcf8b10b4c6c8eb1e7568e6e>`(const InT& value);

	template <class InT>
	InT :ref:`InferenceEngine::PrecisionUtils::saturate_cast<doxid-group__ie__dev__api__precision_1ga5aebe960c48ca8518a3526dbb54969c8>`(const InT& value);

.. _details-group__ie__dev__api__precision:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of functions to convert from FP32 to FP16 and vice versa.

Typedefs
--------

.. _doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c:
.. index:: pair: typedef; ie_fp16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef short InferenceEngine::ie_fp16

A type difinition for FP16 data type. Defined as a singed short.

Global Functions
----------------

.. _doxid-group__ie__dev__api__precision_1ga4669263097f51520c2f2f62c44d7bb65:
.. index:: pair: function; f32tof16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` InferenceEngine::PrecisionUtils::f32tof16(float x)

Converts a single-precision floating point value to a half-precision floating poit value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- x

		- A single-precision floating point value



.. rubric:: Returns:

A half-precision floating point value

.. _doxid-group__ie__dev__api__precision_1ga13155ccd32a9c8ecca615eef89af3f5d:
.. index:: pair: function; f16tof32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float InferenceEngine::PrecisionUtils::f16tof32(:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` x)

Convers a half-precision floating point value to a single-precision floating point value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- x

		- A half-precision floating point value



.. rubric:: Returns:

A single-precision floating point value

.. _doxid-group__ie__dev__api__precision_1ga9b3a5d90bb1d3439dddf758af1035ffe:
.. index:: pair: function; f16tof32Arrays

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void InferenceEngine::PrecisionUtils::f16tof32Arrays(
		float \* dst,
		const :ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` \* src,
		size_t nelem,
		float scale = 1.f,
		float bias = 0.f
		)

Converts a half-precision floating point array to single-precision floating point array and applies ``scale`` and ``bias`` is needed.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst

		- A destination array of single-precision floating point values

	*
		- src

		- A source array of half-precision floating point values

	*
		- nelem

		- A number of elements in arrays

	*
		- scale

		- An optional scale parameter

	*
		- bias

		- An optional bias parameter

.. _doxid-group__ie__dev__api__precision_1gaa08cea0abc12560240b4f8c5c168ac75:
.. index:: pair: function; f32tof16Arrays

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void InferenceEngine::PrecisionUtils::f32tof16Arrays(
		:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` \* dst,
		const float \* src,
		size_t nelem,
		float scale = 1.f,
		float bias = 0.f
		)

Converts a single-precision floating point array to a half-precision floating point array and applies ``scale`` and ``bias`` if needed.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst

		- A destination array of half-precision floating point values

	*
		- src

		- A sources array of single-precision floating point values

	*
		- nelem

		- A number of elements in arrays

	*
		- scale

		- An optional scale parameter

	*
		- bias

		- An optional bias parameter

.. _doxid-group__ie__dev__api__precision_1ga38df1785fcf8b10b4c6c8eb1e7568e6e:
.. index:: pair: function; saturate_cast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class OutT,
		class InT,
		typename std::enable_if<std::is_integral<OutT>::value&&std::is_integral<InT>::value&&std::is_signed<InT>::value&&!std::is_same<OutT, InT>::value>::type \* = nullptr
		>
	OutT InferenceEngine::PrecisionUtils::saturate_cast(const InT& value)

Converts one integral type to another saturating the result if the source value doesn't fit into destination type range.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- Value to be converted



.. rubric:: Returns:

A saturated value

.. _doxid-group__ie__dev__api__precision_1ga5aebe960c48ca8518a3526dbb54969c8:
.. index:: pair: function; saturate_cast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class InT>
	InT InferenceEngine::PrecisionUtils::saturate_cast(const InT& value)

Converts one integral type to another saturating the result if the source value doesn't fit into destination type range.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- Value to be converted



.. rubric:: Returns:

A saturated value

