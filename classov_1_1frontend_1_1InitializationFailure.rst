.. index:: pair: class; ov::frontend::InitializationFailure
.. _doxid-classov_1_1frontend_1_1_initialization_failure:

class ov::frontend::InitializationFailure
=========================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <exception.hpp>
	
	class InitializationFailure: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`InitializationFailure<doxid-classov_1_1frontend_1_1_initialization_failure_1af06aaf87aee198c8e24cb14869e0a78a>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context,
			const std::string& explanation
			);
	};

