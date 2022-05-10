.. index:: pair: struct; ngraph::runtime::reference::details::IsRandomAccessIt
.. _doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_is_random_access_it:

struct ngraph::runtime::reference::details::IsRandomAccessIt
============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <span.hpp>
	
	template <typename It>
	struct IsRandomAccessIt
	{
		// fields
	
		static constexpr bool :target:`value<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_is_random_access_it_1a1cda34ea8df73d6ccf001fa97ffeeb98>` = std::is_same<typename It::iterator_category, std::random_access_iterator_tag>::value;
	};

