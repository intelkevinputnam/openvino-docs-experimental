.. index:: pair: class; ngraph::pass::low_precision::NetworkHelper::InsertDequantizationResult
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result:

class ngraph::pass::low_precision::NetworkHelper::InsertDequantizationResult
============================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <network_helper.hpp>
	
	class InsertDequantizationResult
	{
	public:
		// fields
	
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`newOperation<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result_1aa5346139c9c82a3c0c3fd3e5149c4937>`;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`lastDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result_1ad0ba9bd35b87cbb5382359a0654ae067>`;

		// construction
	
		:target:`InsertDequantizationResult<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result_1aff66ca8c1aa7230c284061099ae33ab5>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& newOperation,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& lastDequantization
			);
	};

