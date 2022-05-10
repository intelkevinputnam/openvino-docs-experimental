.. index:: pair: class; ov::util::LogHelper
.. _doxid-classov_1_1util_1_1_log_helper:

class ov::util::LogHelper
=========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <log.hpp>
	
	class LogHelper
	{
	public:
		// construction
	
		:target:`LogHelper<doxid-classov_1_1util_1_1_log_helper_1aece5dcfd489a099ecaa3cd1786b47af3>`(
			:ref:`LOG_TYPE<doxid-namespaceov_1_1util_1a652c65f7fe5550a6d96d273d12fe0a13>`,
			const char \* file,
			int line,
			std::function<void(const std::string&)> m_handler_func
			);

		// methods
	
		std::ostream& :target:`stream<doxid-classov_1_1util_1_1_log_helper_1a51116b145f59f170d08ea53b5c304b81>`();
	};

