.. index:: pair: namespace; ngraph::runtime::reference::fake_quantize_details
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details:

namespace ngraph::runtime::reference::fake_quantize_details
===========================================================

.. toctree::
	:hidden:

	QuantizationBound <classngraph_1_1runtime_1_1reference_1_1fake_quantize_details_1_1QuantizationBound.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace fake_quantize_details {

	// classes

	template <typename T>
	class :ref:`QuantizationBound<doxid-classngraph_1_1runtime_1_1reference_1_1fake__quantize__details_1_1_quantization_bound>`;

	// global functions

	std::vector<size_t> :target:`calc_broadcast_index_offset<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details_1a46aedd37a42a2b6980f2ddd4184f953d>`(
		const std::vector<size_t>& memory_offsets,
		const std::vector<size_t>& broadcast_shape
		);

	size_t :target:`calc_full_broadcast_offset<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details_1aaf3d04e29aeda2f72bfa533a538a6bdd>`(
		const std::vector<size_t>& current_dims,
		const std::vector<size_t>& offsets
		);

	:ref:`Shape<doxid-classov_1_1_shape>` :target:`align_shape_sizes<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details_1a4adb226ed3fa4fb6f17679a121613c4d>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& target_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast
		);

	void :target:`increment_current_dim<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details_1aa7083f31fe412d95c0a4b24ec8480014>`(
		std::vector<size_t>& current_dims,
		const std::vector<size_t>& shape
		);

	template <typename T>
	T :target:`quantize<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details_1af99cbebad57b74e27af4c402cdcff0ef>`(
		const T& arg,
		const T& in_low,
		const T& in_high,
		const T& out_low,
		const T& out_high,
		const size_t& levels
		);

	} // namespace fake_quantize_details
