.. index:: pair: namespace; InferenceEngine::PrecisionUtils
.. _doxid-namespace_inference_engine_1_1_precision_utils:

namespace InferenceEngine::PrecisionUtils
=========================================

.. toctree::
	:hidden:

	details <namespaceInferenceEngine_1_1PrecisionUtils_1_1details.rst>

Namespace for precision utilities.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace PrecisionUtils {

	// namespaces

	namespace :ref:`InferenceEngine::PrecisionUtils::details<doxid-namespace_inference_engine_1_1_precision_utils_1_1details>`;

	// global functions

	:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` :ref:`f32tof16<doxid-group__ie__dev__api__precision_1ga4669263097f51520c2f2f62c44d7bb65>`(float x);
	float :ref:`f16tof32<doxid-group__ie__dev__api__precision_1ga13155ccd32a9c8ecca615eef89af3f5d>`(:ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` x);

	void :ref:`f16tof32Arrays<doxid-group__ie__dev__api__precision_1ga9b3a5d90bb1d3439dddf758af1035ffe>`(
		float \* dst,
		const :ref:`ie_fp16<doxid-group__ie__dev__api__precision_1ga262fb3c75a243a474ab6d46e056e537c>` \* src,
		size_t nelem,
		float scale = 1.f,
		float bias = 0.f
		);

	void :ref:`f32tof16Arrays<doxid-group__ie__dev__api__precision_1gaa08cea0abc12560240b4f8c5c168ac75>`(
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
	OutT :ref:`saturate_cast<doxid-group__ie__dev__api__precision_1ga38df1785fcf8b10b4c6c8eb1e7568e6e>`(const InT& value);

	template <class InT>
	InT :ref:`saturate_cast<doxid-group__ie__dev__api__precision_1ga5aebe960c48ca8518a3526dbb54969c8>`(const InT& value);

	} // namespace PrecisionUtils
