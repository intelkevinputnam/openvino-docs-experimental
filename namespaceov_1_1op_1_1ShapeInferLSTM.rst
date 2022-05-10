.. index:: pair: namespace; ov::op::ShapeInferLSTM
.. _doxid-namespaceov_1_1op_1_1_shape_infer_l_s_t_m:

namespace ov::op::ShapeInferLSTM
================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace ShapeInferLSTM {

	// global functions

	template <class OpsType, class ShapeType>
	void :target:`lstm_shape_infer<doxid-namespaceov_1_1op_1_1_shape_infer_l_s_t_m_1a36f808a3d3ab022537c60b71b2941641>`(
		const OpsType \* op,
		const std::vector<ShapeType>& input_shapes,
		std::vector<ShapeType>& output_shapes,
		std::size_t gates_count
		);

	} // namespace ShapeInferLSTM
