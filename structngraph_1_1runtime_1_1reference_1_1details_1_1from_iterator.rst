.. index:: pair: struct; ngraph::runtime::reference::details::from_iterator
.. _doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1from__iterator:

struct ngraph::runtime::reference::details::from_iterator
=========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <span.hpp>
	
	template <typename It>
	struct from_iterator
	{
		// typedefs
	
		typedef typename std::remove_pointer<typename std::iterator_traits<It>::pointer>::type :target:`stored_value<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1from__iterator_1a5d9c8b6d3cf3bbac0fe4ded737808b16>`;
	};

