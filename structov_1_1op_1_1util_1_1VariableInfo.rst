.. index:: pair: struct; ov::op::util::VariableInfo
.. _doxid-structov_1_1op_1_1util_1_1_variable_info:

struct ov::op::util::VariableInfo
=================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable.hpp>
	
	struct VariableInfo
	{
		// fields
	
		:ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`data_shape<doxid-structov_1_1op_1_1util_1_1_variable_info_1a2c9549df9e852b646c4ec31ff1b5c83e>`;
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :target:`data_type<doxid-structov_1_1op_1_1util_1_1_variable_info_1a9ba5537d412bd93814e6cce6b185e25e>`;
		std::string :target:`variable_id<doxid-structov_1_1op_1_1util_1_1_variable_info_1ab7ed425b417d197d53ef1e2d75a09517>`;

		// methods
	
		bool :target:`operator ==<doxid-structov_1_1op_1_1util_1_1_variable_info_1a5017199c1f72d7fcccfa35483fff0bea>` (const VariableInfo& other) const;
	};

