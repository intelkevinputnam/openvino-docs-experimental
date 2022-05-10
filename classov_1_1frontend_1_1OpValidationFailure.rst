.. index:: pair: class; ov::frontend::OpValidationFailure
.. _doxid-classov_1_1frontend_1_1_op_validation_failure:

class ov::frontend::OpValidationFailure
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <exception.hpp>
	
	class OpValidationFailure: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`OpValidationFailure<doxid-classov_1_1frontend_1_1_op_validation_failure_1acbe3e55a52c01cd39aa5fa7a3ab1d39d>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context,
			const std::string& explanation
			);
	};

