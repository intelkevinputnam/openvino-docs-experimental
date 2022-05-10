.. index:: pair: class; ov::op::Op
.. _doxid-classov_1_1op_1_1_op:

class ov::op::Op
================



Overview
~~~~~~~~

Root of all actual ops. :ref:`More...<details-classov_1_1op_1_1_op>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <op.hpp>
	
	class Op: public :ref:`ov::Node<doxid-classov_1_1_node>`
	{
	public:
		// methods
	
		static _OPENVINO_HIDDEN_METHODconst :::ref:`ov::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& :target:`get_type_info_static<doxid-classov_1_1op_1_1_op_1a236ae4310a12e8b9ee7115af2154c489>`();
		virtual const :::ref:`ov::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& :ref:`get_type_info<doxid-classov_1_1op_1_1_op_1ae930efe3e70276acfd9d349aa58dabb7>`() const;
	};

	// direct descendants

	class :ref:`ConvolutionIE<doxid-classngraph_1_1op_1_1_convolution_i_e>`;
	class :ref:`CropIE<doxid-classngraph_1_1op_1_1_crop_i_e>`;
	class :ref:`DeconvolutionIE<doxid-classngraph_1_1op_1_1_deconvolution_i_e>`;
	class :ref:`Eltwise<doxid-classngraph_1_1op_1_1_eltwise>`;
	class :ref:`FullyConnected<doxid-classngraph_1_1op_1_1_fully_connected>`;
	class :ref:`GatherIE<doxid-classngraph_1_1op_1_1_gather_i_e>`;
	class :ref:`GatherTreeIE<doxid-classngraph_1_1op_1_1_gather_tree_i_e>`;
	class :ref:`GRUCellIE<doxid-classngraph_1_1op_1_1_g_r_u_cell_i_e>`;
	class :ref:`HardSigmoid_IE<doxid-classngraph_1_1op_1_1_hard_sigmoid___i_e>`;
	class :ref:`NonMaxSuppressionIEInternal<doxid-classngraph_1_1op_1_1internal_1_1_non_max_suppression_i_e_internal>`;
	class :ref:`Interp<doxid-classngraph_1_1op_1_1_interp>`;
	class :ref:`LRN_IE<doxid-classngraph_1_1op_1_1_l_r_n___i_e>`;
	class :ref:`LSTMCellIE<doxid-classngraph_1_1op_1_1_l_s_t_m_cell_i_e>`;
	class :ref:`NonMaxSuppressionIE<doxid-classngraph_1_1op_1_1_non_max_suppression_i_e>`;
	class :ref:`NonMaxSuppressionIE3<doxid-classngraph_1_1op_1_1_non_max_suppression_i_e3>`;
	class :ref:`NormalizeIE<doxid-classngraph_1_1op_1_1_normalize_i_e>`;
	class :ref:`OneHotIE<doxid-classngraph_1_1op_1_1_one_hot_i_e>`;
	class :ref:`PadIE<doxid-classngraph_1_1op_1_1_pad_i_e>`;
	class :ref:`PowerIE<doxid-classngraph_1_1op_1_1_power_i_e>`;
	class :ref:`ProposalIE<doxid-classngraph_1_1op_1_1_proposal_i_e>`;
	class :ref:`ReLUIE<doxid-classngraph_1_1op_1_1_re_l_u_i_e>`;
	class :ref:`ResampleV2<doxid-classngraph_1_1op_1_1_resample_v2>`;
	class :ref:`RNNCellIE<doxid-classngraph_1_1op_1_1_r_n_n_cell_i_e>`;
	class :ref:`ScaleShiftIE<doxid-classngraph_1_1op_1_1_scale_shift_i_e>`;
	class :ref:`SeluIE<doxid-classngraph_1_1op_1_1_selu_i_e>`;
	class :ref:`SwishIE<doxid-classngraph_1_1op_1_1_swish_i_e>`;
	class :ref:`TileIE<doxid-classngraph_1_1op_1_1_tile_i_e>`;
	class :ref:`TopKIE<doxid-classngraph_1_1op_1_1_top_k_i_e>`;
	template :ref:`BroadcastMove<doxid-classngraph_1_1snippets_1_1op_1_1_broadcast_move>`;
	template :ref:`Kernel<doxid-classngraph_1_1snippets_1_1op_1_1_kernel>`;
	template :ref:`Load<doxid-classngraph_1_1snippets_1_1op_1_1_load>`;
	template :ref:`Nop<doxid-classngraph_1_1snippets_1_1op_1_1_nop>`;
	class :ref:`Store<doxid-classngraph_1_1snippets_1_1op_1_1_store>`;
	template :ref:`Subgraph<doxid-classngraph_1_1snippets_1_1op_1_1_subgraph>`;
	template :ref:`Tile<doxid-classngraph_1_1snippets_1_1op_1_1_tile>`;
	class :ref:`Sink<doxid-classov_1_1op_1_1_sink>`;
	class :ref:`BinaryElementwiseArithmetic<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_arithmetic>`;
	class :ref:`BinaryElementwiseComparison<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_comparison>`;
	class :ref:`BinaryElementwiseLogical<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical>`;
	class :ref:`BroadcastBase<doxid-classov_1_1op_1_1util_1_1_broadcast_base>`;
	class :ref:`ConvertColorI420Base<doxid-classov_1_1op_1_1util_1_1_convert_color_i420_base>`;
	class :ref:`ConvertColorNV12Base<doxid-classov_1_1op_1_1util_1_1_convert_color_n_v12_base>`;
	class :ref:`DeformableConvolutionBase<doxid-classov_1_1op_1_1util_1_1_deformable_convolution_base>`;
	class :ref:`DetectionOutputBase<doxid-classov_1_1op_1_1util_1_1_detection_output_base>`;
	class :ref:`EmbeddingBagOffsetsBase<doxid-classov_1_1op_1_1util_1_1_embedding_bag_offsets_base>`;
	class :ref:`EmbeddingBagPackedBase<doxid-classov_1_1op_1_1util_1_1_embedding_bag_packed_base>`;
	class :ref:`FFTBase<doxid-classov_1_1op_1_1util_1_1_f_f_t_base>`;
	class :ref:`FrameworkNode<doxid-classov_1_1op_1_1util_1_1_framework_node>`;
	class :ref:`GatherBase<doxid-classov_1_1op_1_1util_1_1_gather_base>`;
	class :ref:`GatherNDBase<doxid-classov_1_1op_1_1util_1_1_gather_n_d_base>`;
	class :ref:`IndexReduction<doxid-classov_1_1op_1_1util_1_1_index_reduction>`;
	class :ref:`MaxPoolBase<doxid-classov_1_1op_1_1util_1_1_max_pool_base>`;
	class :ref:`MultiSubGraphOp<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`;
	class :ref:`NmsBase<doxid-classov_1_1op_1_1util_1_1_nms_base>`;
	class :ref:`ReadValueBase<doxid-classov_1_1op_1_1util_1_1_read_value_base>`;
	class :ref:`ReductionBase<doxid-classov_1_1op_1_1util_1_1_reduction_base>`;
	class :ref:`RNNCellBase<doxid-classov_1_1op_1_1util_1_1_r_n_n_cell_base>`;
	class :ref:`ScatterBase<doxid-classov_1_1op_1_1util_1_1_scatter_base>`;
	class :ref:`ScatterNDBase<doxid-classov_1_1op_1_1util_1_1_scatter_n_d_base>`;
	class :ref:`UnaryElementwiseArithmetic<doxid-classov_1_1op_1_1util_1_1_unary_elementwise_arithmetic>`;
	class :ref:`BatchNormInference<doxid-classov_1_1op_1_1v0_1_1_batch_norm_inference>`;
	class :ref:`Clamp<doxid-classov_1_1op_1_1v0_1_1_clamp>`;
	class :ref:`Concat<doxid-classov_1_1op_1_1v0_1_1_concat>`;
	class :ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`;
	class :ref:`Convert<doxid-classov_1_1op_1_1v0_1_1_convert>`;
	class :ref:`CTCGreedyDecoder<doxid-classov_1_1op_1_1v0_1_1_c_t_c_greedy_decoder>`;
	class :ref:`CumSum<doxid-classov_1_1op_1_1v0_1_1_cum_sum>`;
	class :ref:`DepthToSpace<doxid-classov_1_1op_1_1v0_1_1_depth_to_space>`;
	class :ref:`Elu<doxid-classov_1_1op_1_1v0_1_1_elu>`;
	class :ref:`FakeQuantize<doxid-classov_1_1op_1_1v0_1_1_fake_quantize>`;
	class :ref:`Gelu<doxid-classov_1_1op_1_1v0_1_1_gelu>`;
	class :ref:`GRN<doxid-classov_1_1op_1_1v0_1_1_g_r_n>`;
	class :ref:`HardSigmoid<doxid-classov_1_1op_1_1v0_1_1_hard_sigmoid>`;
	class :ref:`Interpolate<doxid-classov_1_1op_1_1v0_1_1_interpolate>`;
	class :ref:`LRN<doxid-classov_1_1op_1_1v0_1_1_l_r_n>`;
	class :ref:`LSTMSequence<doxid-classov_1_1op_1_1v0_1_1_l_s_t_m_sequence>`;
	class :ref:`MatMul<doxid-classov_1_1op_1_1v0_1_1_mat_mul>`;
	class :ref:`MVN<doxid-classov_1_1op_1_1v0_1_1_m_v_n>`;
	class :ref:`NormalizeL2<doxid-classov_1_1op_1_1v0_1_1_normalize_l2>`;
	class :ref:`Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`;
	class :ref:`PRelu<doxid-classov_1_1op_1_1v0_1_1_p_relu>`;
	class :ref:`PriorBox<doxid-classov_1_1op_1_1v0_1_1_prior_box>`;
	class :ref:`PriorBoxClustered<doxid-classov_1_1op_1_1v0_1_1_prior_box_clustered>`;
	class :ref:`Proposal<doxid-classov_1_1op_1_1v0_1_1_proposal>`;
	class :ref:`PSROIPooling<doxid-classov_1_1op_1_1v0_1_1_p_s_r_o_i_pooling>`;
	class :ref:`Range<doxid-classov_1_1op_1_1v0_1_1_range>`;
	class :ref:`RegionYolo<doxid-classov_1_1op_1_1v0_1_1_region_yolo>`;
	class :ref:`ReorgYolo<doxid-classov_1_1op_1_1v0_1_1_reorg_yolo>`;
	class :ref:`Result<doxid-classov_1_1op_1_1v0_1_1_result>`;
	class :ref:`ReverseSequence<doxid-classov_1_1op_1_1v0_1_1_reverse_sequence>`;
	class :ref:`ROIPooling<doxid-classov_1_1op_1_1v0_1_1_r_o_i_pooling>`;
	class :ref:`Selu<doxid-classov_1_1op_1_1v0_1_1_selu>`;
	class :ref:`ShapeOf<doxid-classov_1_1op_1_1v0_1_1_shape_of>`;
	class :ref:`ShuffleChannels<doxid-classov_1_1op_1_1v0_1_1_shuffle_channels>`;
	class :ref:`SpaceToDepth<doxid-classov_1_1op_1_1v0_1_1_space_to_depth>`;
	class :ref:`Squeeze<doxid-classov_1_1op_1_1v0_1_1_squeeze>`;
	class :ref:`Tile<doxid-classov_1_1op_1_1v0_1_1_tile>`;
	class :ref:`Unsqueeze<doxid-classov_1_1op_1_1v0_1_1_unsqueeze>`;
	class :ref:`AvgPool<doxid-classov_1_1op_1_1v1_1_1_avg_pool>`;
	class :ref:`BatchToSpace<doxid-classov_1_1op_1_1v1_1_1_batch_to_space>`;
	class :ref:`BinaryConvolution<doxid-classov_1_1op_1_1v1_1_1_binary_convolution>`;
	class :ref:`ConvertLike<doxid-classov_1_1op_1_1v1_1_1_convert_like>`;
	class :ref:`Convolution<doxid-classov_1_1op_1_1v1_1_1_convolution>`;
	class :ref:`ConvolutionBackpropData<doxid-classov_1_1op_1_1v1_1_1_convolution_backprop_data>`;
	class :ref:`DeformablePSROIPooling<doxid-classov_1_1op_1_1v1_1_1_deformable_p_s_r_o_i_pooling>`;
	class :ref:`GatherTree<doxid-classov_1_1op_1_1v1_1_1_gather_tree>`;
	class :ref:`GroupConvolution<doxid-classov_1_1op_1_1v1_1_1_group_convolution>`;
	class :ref:`GroupConvolutionBackpropData<doxid-classov_1_1op_1_1v1_1_1_group_convolution_backprop_data>`;
	class :ref:`LogicalNot<doxid-classov_1_1op_1_1v1_1_1_logical_not>`;
	class :ref:`NonMaxSuppression<doxid-classov_1_1op_1_1v1_1_1_non_max_suppression>`;
	class :ref:`OneHot<doxid-classov_1_1op_1_1v1_1_1_one_hot>`;
	class :ref:`Pad<doxid-classov_1_1op_1_1v1_1_1_pad>`;
	class :ref:`Reshape<doxid-classov_1_1op_1_1v1_1_1_reshape>`;
	class :ref:`Reverse<doxid-classov_1_1op_1_1v1_1_1_reverse>`;
	class :ref:`Select<doxid-classov_1_1op_1_1v1_1_1_select>`;
	class :ref:`Softmax<doxid-classov_1_1op_1_1v1_1_1_softmax>`;
	class :ref:`SpaceToBatch<doxid-classov_1_1op_1_1v1_1_1_space_to_batch>`;
	class :ref:`Split<doxid-classov_1_1op_1_1v1_1_1_split>`;
	class :ref:`StridedSlice<doxid-classov_1_1op_1_1v1_1_1_strided_slice>`;
	class :ref:`TopK<doxid-classov_1_1op_1_1v1_1_1_top_k>`;
	class :ref:`Transpose<doxid-classov_1_1op_1_1v1_1_1_transpose>`;
	class :ref:`VariadicSplit<doxid-classov_1_1op_1_1v1_1_1_variadic_split>`;
	class :ref:`Bucketize<doxid-classov_1_1op_1_1v3_1_1_bucketize>`;
	class :ref:`EmbeddingSegmentsSum<doxid-classov_1_1op_1_1v3_1_1_embedding_segments_sum>`;
	class :ref:`ExtractImagePatches<doxid-classov_1_1op_1_1v3_1_1_extract_image_patches>`;
	class :ref:`NonMaxSuppression<doxid-classov_1_1op_1_1v3_1_1_non_max_suppression>`;
	class :ref:`NonZero<doxid-classov_1_1op_1_1v3_1_1_non_zero>`;
	class :ref:`ROIAlign<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align>`;
	class :ref:`ScatterElementsUpdate<doxid-classov_1_1op_1_1v3_1_1_scatter_elements_update>`;
	class :ref:`ShapeOf<doxid-classov_1_1op_1_1v3_1_1_shape_of>`;
	class :ref:`CTCLoss<doxid-classov_1_1op_1_1v4_1_1_c_t_c_loss>`;
	class :ref:`Interpolate<doxid-classov_1_1op_1_1v4_1_1_interpolate>`;
	class :ref:`Mish<doxid-classov_1_1op_1_1v4_1_1_mish>`;
	class :ref:`Range<doxid-classov_1_1op_1_1v4_1_1_range>`;
	class :ref:`SoftPlus<doxid-classov_1_1op_1_1v4_1_1_soft_plus>`;
	class :ref:`Swish<doxid-classov_1_1op_1_1v4_1_1_swish>`;
	class :ref:`BatchNormInference<doxid-classov_1_1op_1_1v5_1_1_batch_norm_inference>`;
	class :ref:`LogSoftmax<doxid-classov_1_1op_1_1v5_1_1_log_softmax>`;
	class :ref:`NonMaxSuppression<doxid-classov_1_1op_1_1v5_1_1_non_max_suppression>`;
	class :ref:`Round<doxid-classov_1_1op_1_1v5_1_1_round>`;
	class :ref:`CTCGreedyDecoderSeqLen<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len>`;
	class :ref:`ExperimentalDetectronDetectionOutput<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_detection_output>`;
	class :ref:`ExperimentalDetectronGenerateProposalsSingleImage<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_generate_proposals_single_image>`;
	class :ref:`ExperimentalDetectronPriorGridGenerator<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_prior_grid_generator>`;
	class :ref:`ExperimentalDetectronROIFeatureExtractor<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_r_o_i_feature_extractor>`;
	class :ref:`ExperimentalDetectronTopKROIs<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_top_k_r_o_is>`;
	class :ref:`GatherElements<doxid-classov_1_1op_1_1v6_1_1_gather_elements>`;
	class :ref:`MVN<doxid-classov_1_1op_1_1v6_1_1_m_v_n>`;
	class :ref:`Einsum<doxid-classov_1_1op_1_1v7_1_1_einsum>`;
	class :ref:`Roll<doxid-classov_1_1op_1_1v7_1_1_roll>`;
	class :ref:`AdaptiveAvgPool<doxid-classov_1_1op_1_1v8_1_1_adaptive_avg_pool>`;
	class :ref:`AdaptiveMaxPool<doxid-classov_1_1op_1_1v8_1_1_adaptive_max_pool>`;
	class :ref:`PriorBox<doxid-classov_1_1op_1_1v8_1_1_prior_box>`;
	class :ref:`RandomUniform<doxid-classov_1_1op_1_1v8_1_1_random_uniform>`;
	class :ref:`Slice<doxid-classov_1_1op_1_1v8_1_1_slice>`;
	class :ref:`Softmax<doxid-classov_1_1op_1_1v8_1_1_softmax>`;
	class :ref:`Eye<doxid-classov_1_1op_1_1v9_1_1_eye>`;
	class :ref:`ROIAlign<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`;
		typedef std::map<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`;

		// methods
	
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1_node_1ac5224b5be848ec670d2078d9816d12e7>`();
		void :ref:`constructor_validate_and_infer_types<doxid-classov_1_1_node_1aab98e14f28ac255819dfa4118174ece3>`();
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_node_1a9743b56d352970486d17dae2416d958e>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		virtual const :ref:`ov::op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& :ref:`get_autob<doxid-classov_1_1_node_1a2b4875877f138f9cc7ee51a207268b73>`() const;
		virtual bool :ref:`has_evaluate<doxid-classov_1_1_node_1a606a47a0c2d39dcc4032b985c04c209e>`() const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1acfb82acc8349d7138aeaa05217c7014e>`(
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values
			) const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1afe8b36f599d5f2f1f8b4ef0f1a56a65c>`(
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values,
			const :ref:`EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`& evaluationContext
			) const;
	
		virtual bool :ref:`evaluate_lower<doxid-classov_1_1_node_1a214ae74aa0de1eeaadeafb719e6ff260>`(const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values) const;
		virtual bool :ref:`evaluate_upper<doxid-classov_1_1_node_1ab509aeccf31f20473fa742df915f67e5>`(const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values) const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1a6096b644f59b1a7d1a1bf6bafe140472>`(
			:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values,
			const :ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& input_values
			) const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1af17129ce66b7273dfe9328ef21e61494>`(
			:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values,
			const :ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& input_values,
			const :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`& evaluationContext
			) const;
	
		virtual bool :ref:`evaluate_lower<doxid-classov_1_1_node_1aed425e8df8114daefbfe2b90b6ccde59>`(:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values) const;
		virtual bool :ref:`evaluate_upper<doxid-classov_1_1_node_1a191a82c8acc6016e2991a2dff3c626f8>`(:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values) const;
		virtual bool :ref:`evaluate_label<doxid-classov_1_1_node_1a5ac5781812584d5bec31381fa513cb75>`(:ref:`TensorLabelVector<doxid-namespaceov_1aa5b856e58283417ceeace7343237b623>`& output_labels) const;
	
		virtual bool :ref:`constant_fold<doxid-classov_1_1_node_1a54e3bc84a49870563abf07e0fdd92de9>`(
			:ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& output_values,
			const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs_values
			);
	
		virtual :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :ref:`decompose_op<doxid-classov_1_1_node_1add7ebde1542aef560a5d5135e8fe7b67>`() const;
		virtual const :ref:`type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& :ref:`get_type_info<doxid-classov_1_1_node_1a09d7370d5fa57c28880598760fd9c893>`() const = 0;
		const char \* :ref:`get_type_name<doxid-classov_1_1_node_1a312ad4b62537167e5e5c784df8b03ff3>`() const;
		void :ref:`set_arguments<doxid-classov_1_1_node_1a939c896986f4c0cfc9e47895d698b051>`(const :ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& arguments);
		void :ref:`set_arguments<doxid-classov_1_1_node_1a9476f10de4bf8eaffbc3bc54abbd67bc>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& arguments);
		void :ref:`set_argument<doxid-classov_1_1_node_1ab90cfad02a35d49500c1773dca71d09a>`(size_t position, const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& argument);
	
		void :ref:`set_output_type<doxid-classov_1_1_node_1affde9025d41a4b200d726bee750b20e4>`(
			size_t i,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& pshape
			);
	
		void :ref:`set_output_size<doxid-classov_1_1_node_1a27a4363bf01e836006ef0ff0ad1fb7e0>`(size_t output_size);
		void :ref:`invalidate_values<doxid-classov_1_1_node_1af4f961268c306511c2c28ee66bc81639>`();
		virtual void :ref:`revalidate_and_infer_types<doxid-classov_1_1_node_1a474ccc02e97cb12224a339b843e30615>`();
		virtual std::string :ref:`description<doxid-classov_1_1_node_1abb0f7c0a63ff520f7955378ec52b98d3>`() const;
		const std::string& :ref:`get_name<doxid-classov_1_1_node_1a82d9842d00beff82932b5baac3e723a3>`() const;
		void :ref:`set_friendly_name<doxid-classov_1_1_node_1a7980b10e7fa641adb972bbfc27e94dc4>`(const std::string& name);
		const std::string& :ref:`get_friendly_name<doxid-classov_1_1_node_1a613bbf08ebce8c05c63dacabbc341080>`() const;
		virtual bool :ref:`is_dynamic<doxid-classov_1_1_node_1a55033c8479e6c6e51a6d2cf47cc0575b>`() const;
		size_t :ref:`get_instance_id<doxid-classov_1_1_node_1a97150e2017a476ce1b75580e084244d8>`() const;
		virtual std::ostream& :ref:`write_description<doxid-classov_1_1_node_1a7fcbf2c087273dfb0b7fc153c677dbbb>`(std::ostream& os, uint32_t depth = 0) const;
		const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& :ref:`get_control_dependencies<doxid-classov_1_1_node_1af66774ea3f8ec0699612ee69980de776>`() const;
		const std::vector<:ref:`Node<doxid-classov_1_1_node>` \*>& :ref:`get_control_dependents<doxid-classov_1_1_node_1a464cd8dfcf5f771974ce06bb7e6ec62f>`() const;
		void :ref:`add_control_dependency<doxid-classov_1_1_node_1a47d1a4fb855f1156614846a477f69adb>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		void :ref:`remove_control_dependency<doxid-classov_1_1_node_1a1037a77a8f0220d586b790906b6af488>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		void :ref:`clear_control_dependencies<doxid-classov_1_1_node_1a97cf3538584ac88d8121c38c45fd3820>`();
		void :ref:`clear_control_dependents<doxid-classov_1_1_node_1a08a2dd9069a63d69b6d1ebc7ac3d4921>`();
		void :ref:`add_node_control_dependencies<doxid-classov_1_1_node_1a5aeb2ec8bde867868c391a01dafc1870>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> source_node);
		void :ref:`add_node_control_dependents<doxid-classov_1_1_node_1a54474d9cdeb16624f1fd488c88ecf2ca>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> source_node);
		void :ref:`transfer_control_dependents<doxid-classov_1_1_node_1af0593c95b56ff9723fa748325868db22>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> replacement);
		size_t :ref:`get_output_size<doxid-classov_1_1_node_1ac8706eab0c33f0effa522a6bbed8437e>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_output_element_type<doxid-classov_1_1_node_1af54b4c4728f6fe535e00979c04181926>`(size_t i) const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1_node_1a5f04dfdfeafb4f47afa279f1fab8041f>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_output_shape<doxid-classov_1_1_node_1a9be808628e89171b222165ae2f4b71d5>`(size_t i) const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_output_partial_shape<doxid-classov_1_1_node_1a5002b656c4e79d19e3914f3d28195833>`(size_t i) const;
		:ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`get_default_output<doxid-classov_1_1_node_1aee8da8b622e352e9e21270b7f381e2b1>`() const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_default_output<doxid-classov_1_1_node_1a0a49fd568aea74a68baa2161e4f7df85>`();
		virtual size_t :ref:`get_default_output_index<doxid-classov_1_1_node_1a0d31de32156b3afd0c6db698d888575a>`() const;
		size_t :ref:`no_default_index<doxid-classov_1_1_node_1ad0035c4860b08e05b3e100966a570118>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1_node_1a0e635bd6c9dab32258beb74813a86fa2>`() const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_output_tensor<doxid-classov_1_1_node_1acdba65c4711078f39814267e953f9b26>`(size_t i) const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_input_tensor<doxid-classov_1_1_node_1a1f11abc6a67540cf165cff35c569474e>`(size_t i) const;
		const std::string& :ref:`get_output_tensor_name<doxid-classov_1_1_node_1a4917773db5557c76721e61dd086e2fed>`(size_t i) const;
		std::set<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`get_output_target_inputs<doxid-classov_1_1_node_1af4458f6b74c68754dd5e38b0562aed4c>`(size_t i) const;
		size_t :ref:`get_input_size<doxid-classov_1_1_node_1a19356bfdc8759abdb34f4269bbc6f821>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_input_element_type<doxid-classov_1_1_node_1a376e413971f30898cc2f9552cb80b525>`(size_t i) const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_input_shape<doxid-classov_1_1_node_1a34bd30fb200ea5432351e7495eca3aba>`(size_t i) const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_input_partial_shape<doxid-classov_1_1_node_1a1e506b8cb3d40b6cb096d26627a3227b>`(size_t i) const;
		const std::string& :ref:`get_input_tensor_name<doxid-classov_1_1_node_1a45607918c100cd66492aeb897927fd4c>`(size_t i) const;
		:ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_input_node_ptr<doxid-classov_1_1_node_1a8358ec5a06b653eb8f5a4c7895cb0bec>`(size_t index) const;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input_node_shared_ptr<doxid-classov_1_1_node_1a794272a6a64575a43b55f3854cf5da52>`(size_t index) const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input_source_output<doxid-classov_1_1_node_1aae6163287ddf09da421da058e2375ee2>`(size_t i) const;
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`clone_with_new_inputs<doxid-classov_1_1_node_1a177d1a61e81d506d190ee18818ff851f>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs) const = 0;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`copy_with_new_inputs<doxid-classov_1_1_node_1a71b79a703b6cb65796b3eab14d7f669b>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& new_args) const;
	
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`copy_with_new_inputs<doxid-classov_1_1_node_1aea49595d14777748fe215ce1b0b4f976>`(
			const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs,
			const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& control_dependencies
			) const;
	
		bool :ref:`has_same_type<doxid-classov_1_1_node_1aa0d6ac1b94265535fd6604f504f24bc0>`(std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`> node) const;
		:ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`& :ref:`get_rt_info<doxid-classov_1_1_node_1a5c73794fbc47e510198261d61682fe79>`();
		const :ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`& :ref:`get_rt_info<doxid-classov_1_1_node_1a6b70cf8118b8eb0f499e75e8c59e3dda>`() const;
		:ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` :ref:`get_users<doxid-classov_1_1_node_1ac91febe368510da62e45d591255a4c6e>`(bool check_is_used = false) const;
		virtual size_t :ref:`get_version<doxid-classov_1_1_node_1a09b3d13897b7cadcc7a9967f7a5a41f9>`() const;
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_default_value<doxid-classov_1_1_node_1a829ba04609ff698e5297f86a79eef103>`() const;
		bool :ref:`operator <<doxid-classov_1_1_node_1a041846b4bc1cf064f6bc3f6770a947cf>` (const :ref:`Node<doxid-classov_1_1_node>`& other) const;
		std::vector<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`inputs<doxid-classov_1_1_node_1aae7545fcb3386ab6dbdebdbda409d747>`();
		std::vector<:ref:`Input<doxid-classov_1_1_input>`<const :ref:`Node<doxid-classov_1_1_node>`>> :ref:`inputs<doxid-classov_1_1_node_1a02b7bc6696e0b8aa0bcb2d04d99bc2f1>`() const;
		std::vector<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`input_values<doxid-classov_1_1_node_1a5861ceeb81e573a7eaaf3d036fe5c23a>`() const;
		std::vector<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`outputs<doxid-classov_1_1_node_1aa6d74a054cf5302244978c9c6f9e338d>`();
		std::vector<:ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`>> :ref:`outputs<doxid-classov_1_1_node_1a0d79f0cbc914a3b411869e56a6cb1f94>`() const;
		:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_node_1a2e956e69b0de757004efe88f31f83720>`(size_t input_index);
		:ref:`Input<doxid-classov_1_1_input>`<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_node_1a414bd1a9899c4f1f96286fb2b0ac585b>`(size_t input_index) const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`input_value<doxid-classov_1_1_node_1a0309b251e1dc8722d0cf144199cb1de9>`(size_t input_index) const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_node_1a24dc2a2bac789d34d8e1959249b6347d>`(size_t output_index);
		:ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_node_1afbd386f7c799f4f05393336232b43144>`(size_t output_index) const;
		:ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` void :ref:`set_op_annotations<doxid-classov_1_1_node_1a9d8680c016917426085ce1e18977428f>`(std::shared_ptr<ngraph::op::util::OpAnnotations> op_annotations);
		std::shared_ptr<ngraph::op::util::OpAnnotations> :ref:`get_op_annotations<doxid-classov_1_1_node_1ab396069426f5eabed56e2c8fc3c840d0>`() const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool :ref:`match_value<doxid-classov_1_1_node_1a91d357857f994496c0bfb62f840fa273>`(
			:ref:`ov::pass::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>` \* matcher,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_value,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value
			);
	
		virtual bool :ref:`match_node<doxid-classov_1_1_node_1abdd7772bf5673526b64ddd6d310bb2f9>`(
			:ref:`ov::pass::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>` \* matcher,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value
			);

.. _details-classov_1_1op_1_1_op:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Root of all actual ops.

Methods
-------

.. _doxid-classov_1_1op_1_1_op_1ae930efe3e70276acfd9d349aa58dabb7:
.. index:: pair: function; get_type_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :::ref:`ov::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& get_type_info() const

Returns the NodeTypeInfo for the node's class. During transition to type_info, returns a dummy type_info for :ref:`Node <doxid-classov_1_1_node>` if the class has not been updated yet.


