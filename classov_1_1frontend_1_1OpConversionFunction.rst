.. index:: pair: class; ov::frontend::OpConversionFunction
.. _doxid-classov_1_1frontend_1_1_op_conversion_function:

class ov::frontend::OpConversionFunction
========================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <op.hpp>
	
	class OpConversionFunction
	{
	public:
		// construction
	
		:target:`OpConversionFunction<doxid-classov_1_1frontend_1_1_op_conversion_function_1a615fd3a693a394d312231a4f7068b174>`(
			const std::function<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>()>& op_creator,
			const std::map<std::string, std::string>& attr_names_map = {},
			const std::map<std::string, :ref:`ov::Any<doxid-classov_1_1_any>`>& attr_values_map = {}
			);

		// methods
	
		:ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :target:`operator ()<doxid-classov_1_1frontend_1_1_op_conversion_function_1a723f098f13a95df0e69e14a55ea520f7>` (const :ref:`NodeContext<doxid-classov_1_1frontend_1_1_node_context>`& context);
	};

