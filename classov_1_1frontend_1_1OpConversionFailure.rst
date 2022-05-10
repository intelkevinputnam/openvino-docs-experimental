.. index:: pair: class; ov::frontend::OpConversionFailure
.. _doxid-classov_1_1frontend_1_1_op_conversion_failure:

class ov::frontend::OpConversionFailure
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <exception.hpp>
	
	class OpConversionFailure: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`OpConversionFailure<doxid-classov_1_1frontend_1_1_op_conversion_failure_1a37f972984e1e999ef656802a7abc5d8f>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context,
			const std::string& explanation
			);
	};

