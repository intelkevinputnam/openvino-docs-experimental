.. index:: pair: namespace; ngraph::runtime::reference::fft_common
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common:

namespace ngraph::runtime::reference::fft_common
================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace fft_common {

	// global functions

	std::vector<int64_t> :target:`reverse_shape_of_emulated_complex_tensor<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common_1a6ed4498ac1fa7b8ad8a4c39ca9808dd3>`(const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& shape);
	std::vector<int64_t> :target:`compute_strides<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common_1acbc1b292131109c7e003c794a01a8a14>`(const std::vector<int64_t>& v);

	std::vector<int64_t> :target:`coords_from_index<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common_1a68d54f8eeb38efc5ada4c7e7770f20f4>`(
		int64_t index,
		const std::vector<int64_t>& strides
		);

	int64_t :target:`offset_from_coords_and_strides<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common_1a8690a564ccaedb34daac1c527ac2ff25>`(
		const std::vector<int64_t>& coords,
		const std::vector<int64_t>& strides
		);

	} // namespace fft_common
