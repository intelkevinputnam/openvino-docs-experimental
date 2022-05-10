.. index:: pair: namespace; ngraph::runtime::reference::adaptive_pool
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool:

namespace ngraph::runtime::reference::adaptive_pool
===================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace adaptive_pool {

	// global functions

	size_t :target:`window_start<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool_1ac2e571a1484021a7d122af074abe2f2f>`(size_t idx, size_t arg_shape, size_t out_shape);
	size_t :target:`window_end<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool_1a1ef21ee41e8db1e103e6695ce5643dfb>`(size_t idx, size_t arg_shape, size_t out_shape);

	template <typename T>
	T :target:`avg_div<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool_1aefd41fd47332e1db95ef0ad45bdf1da6>`(const T sum, size_t n);

	template <typename T>
	void :target:`adaptive_avg_pool_1d<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool_1a197a8e9b88d2821c1ce0088829bd5e75>`(
		const T \* arg,
		T \* out,
		size_t h_in,
		size_t h_out
		);

	template <typename T>
	void :target:`adaptive_avg_pool_2d<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool_1ad4c302db91e8d55a4860ccf785c23ecf>`(
		const T \* arg,
		T \* out,
		size_t h_in,
		size_t h_out,
		size_t w_in,
		size_t w_out
		);

	template <typename T>
	void :target:`adaptive_avg_pool_3d<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool_1a5d29004ed2890d954a5938d664a6ce6d>`(
		const T \* arg,
		T \* out,
		size_t d_in,
		size_t d_out,
		size_t h_in,
		size_t h_out,
		size_t w_in,
		size_t w_out
		);

	} // namespace adaptive_pool
