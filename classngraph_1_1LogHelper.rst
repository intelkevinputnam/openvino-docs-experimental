.. index:: pair: class; ngraph::LogHelper
.. _doxid-classngraph_1_1_log_helper:

class ngraph::LogHelper
=======================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <log.hpp>
	
	class LogHelper
	{
	public:
		// construction
	
		:target:`LogHelper<doxid-classngraph_1_1_log_helper_1a17c3ca992714ae0ad93f611fe6b1bb4c>`(
			:ref:`LOG_TYPE<doxid-classngraph_1a0cab963f56b737df2702865a13c17db7>`,
			const char \* file,
			int line,
			std::function<void(const std::string&)> m_handler_func
			);

		// methods
	
		std::ostream& :target:`stream<doxid-classngraph_1_1_log_helper_1ae340f269318ea816862948cd58a8732d>`();
	};

