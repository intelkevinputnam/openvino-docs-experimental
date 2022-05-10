.. index:: pair: class; ov::frontend::GeneralFailure
.. _doxid-classov_1_1frontend_1_1_general_failure:

class ov::frontend::GeneralFailure
==================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <exception.hpp>
	
	class GeneralFailure: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`GeneralFailure<doxid-classov_1_1frontend_1_1_general_failure_1a8ddb1004b34d43aef2f0bcd92a2120bb>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context,
			const std::string& explanation
			);
	};

