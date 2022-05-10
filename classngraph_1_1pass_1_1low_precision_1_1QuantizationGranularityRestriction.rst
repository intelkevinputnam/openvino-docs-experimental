.. index:: pair: class; ngraph::pass::low_precision::QuantizationGranularityRestriction
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction:

class ngraph::pass::low_precision::QuantizationGranularityRestriction
=====================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <quantization_granularity_restriction.hpp>
	
	class QuantizationGranularityRestriction
	{
	public:
		// fields
	
		:ref:`ngraph::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>` :target:`operationType<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1ac1d0448424f04d7cb1718de20b851546>`;
		bool :target:`specifyVersion<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1aa8bfdee0415a2ed4021c756af7727369>`;
		std::vector<:ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`> :target:`restrictions<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1a7ad38157eb330c47b653f38711e40b5f>`;

		// construction
	
		:target:`QuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1a08805cdf9544a6d72e66cae337bbdf23>`();
	
		:target:`QuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1a3fab53b3521b40863888fa469e540d06>`(
			const :ref:`ngraph::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>` operationType,
			const bool specifyVersion,
			const std::vector<:ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`>& restrictions
			);

		// methods
	
		template <typename T>
		static QuantizationGranularityRestriction :target:`create<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1a897bb0fe336fd08b58e269ba90e68d14>`(
			const std::vector<:ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`>& restrictions,
			const bool specifyVersion
			);
	
		template <typename T>
		static QuantizationGranularityRestriction :target:`create<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1a8f77e8879998cb7468930fb455d22fe7>`(
			const std::vector<size_t>& restrictedPorts = {},
			const bool specifyVersion = false
			);
	
		template <typename T>
		static std::vector<:ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`> :target:`getPrecisionsByOperationType<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction_1a5a9836fea6ef804e65f84118602a795d>`(std::vector<QuantizationGranularityRestriction>& restrictions);
	};

