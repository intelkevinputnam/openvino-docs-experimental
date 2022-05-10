.. index:: pair: class; ov::NodeValidationFailure
.. _doxid-classov_1_1_node_validation_failure:

class ov::NodeValidationFailure
===============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node.hpp>
	
	class NodeValidationFailure: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`NodeValidationFailure<doxid-classov_1_1_node_validation_failure_1afd87cc279f15f3c9bcaabe6f8e4ad652>`(
			const :ref:`ov::CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const :ref:`Node<doxid-classov_1_1_node>` \* node,
			const std::string& explanation
			);
	};

