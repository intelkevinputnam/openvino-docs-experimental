.. index:: pair: class; ngraph::ConstString
.. _doxid-classngraph_1_1_const_string:

class ngraph::ConstString
=========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <log.hpp>
	
	class ConstString
	{
	public:
		// construction
	
		template <size_t SIZE>
		:target:`ConstString<doxid-classngraph_1_1_const_string_1a9e0dfaa308edbdc9969c016ad857ba3d>`(const char(&) p[SIZE]);

		// methods
	
		constexpr char :target:`operator []<doxid-classngraph_1_1_const_string_1a094cfccd1690ad05392170462693aaaf>` (size_t i) const;
		constexpr const char \* :target:`get_ptr<doxid-classngraph_1_1_const_string_1a72a264e10ad17bab7e1c31a16033adf7>`(size_t offset) const;
		constexpr size_t :target:`size<doxid-classngraph_1_1_const_string_1ae8a8a7a900ccb70ac88cbdb4497dbebc>`() const;
	};

