.. index:: pair: class; ov::frontend::NotImplementedFailure
.. _doxid-classov_1_1frontend_1_1_not_implemented_failure:

class ov::frontend::NotImplementedFailure
=========================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <exception.hpp>
	
	class NotImplementedFailure: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`NotImplementedFailure<doxid-classov_1_1frontend_1_1_not_implemented_failure_1a6f02da6ab12599411138cf2b85dfb45d>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context,
			const std::string& explanation
			);
	};

