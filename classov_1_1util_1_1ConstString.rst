.. index:: pair: class; ov::util::ConstString
.. _doxid-classov_1_1util_1_1_const_string:

class ov::util::ConstString
===========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <log.hpp>
	
	class ConstString
	{
	public:
		// construction
	
		template <size_t SIZE>
		:target:`ConstString<doxid-classov_1_1util_1_1_const_string_1a3b239ddbcb753cd73a0261b17f4742e3>`(const char(&) p[SIZE]);

		// methods
	
		constexpr char :target:`operator []<doxid-classov_1_1util_1_1_const_string_1a60e28f232d0532eacf68c51bfac8a82a>` (size_t i) const;
		constexpr const char \* :target:`get_ptr<doxid-classov_1_1util_1_1_const_string_1a2092e9112c1e486513637e5f9b446564>`(size_t offset) const;
		constexpr size_t :target:`size<doxid-classov_1_1util_1_1_const_string_1ac67ca7e8407f2eef156aaff825241a6e>`() const;
	};

