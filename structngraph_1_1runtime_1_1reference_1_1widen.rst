.. index:: pair: struct; ngraph::runtime::reference::widen<double>
.. _doxid-structngraph_1_1runtime_1_1reference_1_1widen_3_01double_01_4:

struct ngraph::runtime::reference::widen<double>
================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <helpers.hpp>
	
	template <>
	struct widen<double>
	{
		// typedefs
	
		typedef long double :target:`type<doxid-structngraph_1_1runtime_1_1reference_1_1widen_3_01double_01_4_1ad3831e5cc67d042825b0a6b1c4b0c231>`;
	};

.. index:: pair: struct; ngraph::runtime::reference::widen
.. _doxid-structngraph_1_1runtime_1_1reference_1_1widen:

struct ngraph::runtime::reference::widen
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <helpers.hpp>
	
	template <typename T>
	struct widen
	{
		// typedefs
	
		typedef T :target:`type<doxid-structngraph_1_1runtime_1_1reference_1_1widen_1a833bbfd1d937d0d8bb6dfe0baca1cf0c>`;
	};

.. index:: pair: struct; ngraph::runtime::reference::widen<float>
.. _doxid-structngraph_1_1runtime_1_1reference_1_1widen_3_01float_01_4:

struct ngraph::runtime::reference::widen<float>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <helpers.hpp>
	
	template <>
	struct widen<float>
	{
		// typedefs
	
		typedef double :target:`type<doxid-structngraph_1_1runtime_1_1reference_1_1widen_3_01float_01_4_1a5e18fa92ab062256f01253103db23a1e>`;
	};

