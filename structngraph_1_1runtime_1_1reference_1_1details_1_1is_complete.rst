.. index:: pair: struct; ngraph::runtime::reference::details::is_complete
.. _doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1is__complete:

struct ngraph::runtime::reference::details::is_complete
=======================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <span.hpp>
	
	template <typename, typename = size_t>
	struct is_complete: public false_type
	{
	};

.. index:: pair: struct; ngraph::runtime::reference::details::is_complete<T, decltype(sizeof(T))>
.. _doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1is__complete_3_01_t_00_01decltype_07sizeof_07_t_08_08_4:

struct ngraph::runtime::reference::details::is_complete<T, decltype(sizeof(T))>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <span.hpp>
	
	template <typename T>
	struct is_complete<T, decltype(sizeof(T))>: public true_type
	{
	};

