.. index:: pair: namespace; ov::op::ShapeInferRange
.. _doxid-namespaceov_1_1op_1_1_shape_infer_range:

namespace ov::op::ShapeInferRange
=================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace ShapeInferRange {

	// global functions

	template <class T>
	bool :target:`get_data_as_double<doxid-namespaceov_1_1op_1_1_shape_infer_range_1adabb53b5eb1f874d2830b45fac26dc28>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		std::vector<double>& axes_value,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	bool :target:`get_data_as_double< ov::PartialShape ><doxid-namespaceov_1_1op_1_1_shape_infer_range_1aca3923807e9c3b27d2687a832f772980>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		std::vector<double>& axes_value,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	void :target:`range_shape_infer<doxid-namespaceov_1_1op_1_1_shape_infer_range_1abf23f372b40758055cb561ecac930abf>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		bool output_is_integral,
		bool step_allows_zero,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	} // namespace ShapeInferRange
