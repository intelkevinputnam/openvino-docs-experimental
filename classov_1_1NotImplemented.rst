.. index:: pair: class; ov::NotImplemented
.. _doxid-classov_1_1_not_implemented:

class ov::NotImplemented
========================



:ref:`Exception <doxid-classov_1_1_exception>` class to be thrown on not implemented code.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <except.hpp>
	
	class NotImplemented: public :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>`
	{
	public:
		// construction
	
		:target:`NotImplemented<doxid-classov_1_1_not_implemented_1ad359be4182300842f293ae91305f5f69>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context_info,
			const std::string& explanation
			);
	};

