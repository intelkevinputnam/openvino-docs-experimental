.. index:: pair: namespace; ov::op::v8
.. _doxid-namespaceov_1_1op_1_1v8:

namespace ov::op::v8
====================

.. toctree::
	:hidden:

	DetectionOutput <classov_1_1op_1_1v8_1_1DetectionOutput.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v8 {

	// classes

	class :ref:`AdaptiveAvgPool<doxid-classov_1_1op_1_1v8_1_1_adaptive_avg_pool>`;
	class :ref:`AdaptiveMaxPool<doxid-classov_1_1op_1_1v8_1_1_adaptive_max_pool>`;
	class :ref:`DeformableConvolution<doxid-classov_1_1op_1_1v8_1_1_deformable_convolution>`;
	class :ref:`DetectionOutput<doxid-classov_1_1op_1_1v8_1_1_detection_output>`;
	class :ref:`Gather<doxid-classov_1_1op_1_1v8_1_1_gather>`;
	class :ref:`GatherND<doxid-classov_1_1op_1_1v8_1_1_gather_n_d>`;
	class :ref:`I420toBGR<doxid-classov_1_1op_1_1v8_1_1_i420to_b_g_r>`;
	class :ref:`I420toRGB<doxid-classov_1_1op_1_1v8_1_1_i420to_r_g_b>`;
	class :ref:`If<doxid-classov_1_1op_1_1v8_1_1_if>`;
	class :ref:`MatrixNms<doxid-classov_1_1op_1_1v8_1_1_matrix_nms>`;
	class :ref:`MaxPool<doxid-classov_1_1op_1_1v8_1_1_max_pool>`;
	class :ref:`MulticlassNms<doxid-classov_1_1op_1_1v8_1_1_multiclass_nms>`;
	class :ref:`NV12toBGR<doxid-classov_1_1op_1_1v8_1_1_n_v12to_b_g_r>`;
	class :ref:`NV12toRGB<doxid-classov_1_1op_1_1v8_1_1_n_v12to_r_g_b>`;
	class :ref:`PriorBox<doxid-classov_1_1op_1_1v8_1_1_prior_box>`;
	class :ref:`RandomUniform<doxid-classov_1_1op_1_1v8_1_1_random_uniform>`;
	class :ref:`Slice<doxid-classov_1_1op_1_1v8_1_1_slice>`;
	class :ref:`Softmax<doxid-classov_1_1op_1_1v8_1_1_softmax>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v8_1a89b011116dac96fa6cc56f4911d0d2ce>`(
		const :ref:`DetectionOutput<doxid-classov_1_1op_1_1v8_1_1_detection_output>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	} // namespace v8
