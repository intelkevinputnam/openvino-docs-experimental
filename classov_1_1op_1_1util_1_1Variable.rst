.. index:: pair: class; ov::op::util::Variable
.. _doxid-classov_1_1op_1_1util_1_1_variable:

class ov::op::util::Variable
============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable.hpp>
	
	class Variable
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Variable> :target:`Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`;

		// construction
	
		:target:`Variable<doxid-classov_1_1op_1_1util_1_1_variable_1ac9fbe83d84da2ed4f6bacc31563cfb45>`();
		:target:`Variable<doxid-classov_1_1op_1_1util_1_1_variable_1a37d95a129a5970c8e68ad3da208fecd9>`(:ref:`VariableInfo<doxid-structov_1_1op_1_1util_1_1_variable_info>` variable_info);

		// methods
	
		:ref:`VariableInfo<doxid-structov_1_1op_1_1util_1_1_variable_info>` :target:`get_info<doxid-classov_1_1op_1_1util_1_1_variable_1aeeb750697f088ca2885a326525c7e4a0>`() const;
		void :target:`update<doxid-classov_1_1op_1_1util_1_1_variable_1ad4d8ccfd75dc2caebd89cabaeeac8d31>`(const :ref:`VariableInfo<doxid-structov_1_1op_1_1util_1_1_variable_info>`& variable_info);
	};

