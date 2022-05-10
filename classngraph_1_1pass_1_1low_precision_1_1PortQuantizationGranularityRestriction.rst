.. index:: pair: class; ngraph::pass::low_precision::PortQuantizationGranularityRestriction
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction:

class ngraph::pass::low_precision::PortQuantizationGranularityRestriction
=========================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <port_quantization_granularity_restriction.hpp>
	
	class PortQuantizationGranularityRestriction
	{
	public:
		// fields
	
		size_t :target:`port<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction_1a90cc865903f9a83d017f779074d69bfe>`;
		:ref:`QuantizationGranularityAttribute::Granularity<doxid-classngraph_1_1_quantization_granularity_attribute_1af0340f573997b98910c1f3c33742f530>` :target:`granularity<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction_1a13d5693f4166771ab685a0232b7b1ab5>`;

		// construction
	
		:target:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction_1ae3bfd22321c7b370076e4c51c7582b8a>`(
			const size_t port,
			:ref:`QuantizationGranularityAttribute::Granularity<doxid-classngraph_1_1_quantization_granularity_attribute_1af0340f573997b98910c1f3c33742f530>` granularity
			);
	};

