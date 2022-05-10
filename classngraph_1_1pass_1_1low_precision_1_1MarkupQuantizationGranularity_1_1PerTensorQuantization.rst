.. index:: pair: class; ngraph::pass::low_precision::MarkupQuantizationGranularity::PerTensorQuantization
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity_1_1_per_tensor_quantization:

class ngraph::pass::low_precision::MarkupQuantizationGranularity::PerTensorQuantization
=======================================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <markup_quantization_granularity.hpp>
	
	class PerTensorQuantization
	{
	public:
		// fields
	
		bool :target:`versionIsRequired<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity_1_1_per_tensor_quantization_1adb7c1617b98f736fa5d0933a3add95ec>`;
		std::unordered_map<uint64_t, std::vector<:ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`>> :target:`portsByVersion<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity_1_1_per_tensor_quantization_1a6c48fd6873b426abcb12fae82c5b0d1b>`;

		// construction
	
		:target:`PerTensorQuantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity_1_1_per_tensor_quantization_1a77e7b11c13398097bc486821d0518072>`(const bool versionIsRequired);

		// methods
	
		void :target:`add<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity_1_1_per_tensor_quantization_1ac834f45d1b3f26cada5fa8ac1fbda971>`(
			const uint64_t version,
			const std::vector<:ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`>& restrictions
			);
	};

