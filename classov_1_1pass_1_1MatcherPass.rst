.. index:: pair: class; ov::pass::MatcherPass
.. _doxid-classov_1_1pass_1_1_matcher_pass:

class ov::pass::MatcherPass
===========================



Overview
~~~~~~~~

:ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` is a basic block for pattern based transformations. It describes pattern and action that is applied if pattern is matched. :ref:`More...<details-classov_1_1pass_1_1_matcher_pass>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <graph_rewrite.hpp>
	
	class MatcherPass: public :ref:`ov::pass::PassBase<doxid-classov_1_1pass_1_1_pass_base>`
	{
	public:
		// construction
	
		:target:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass_1a9e5c87177b308b2faf904e0fa967c74c>`();
		:target:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass_1a31224c9105cd687ff2c2f1a547727b89>`(const MatcherPass&);
	
		:target:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass_1a8aae05eafd6c7dfdd08794bda518acf0>`(
			const std::string& name,
			const std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`>& m,
			const :ref:`handler_callback<doxid-namespaceov_1ae9fb36437dbf96b3608f52b7ff565bf0>`& handler,
			const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& property = :ref:`PassProperty::CHANGE_DYNAMIC_STATE<doxid-namespaceov_1_1pass_1afb326b1cdca8f8b1602590c947cf997ea9ea3c2d2ce46d35ece28ff37002ca4b2>`
			);
	
		:target:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass_1a0164cf9b3ca81b683594a22d746d8f5c>`(
			const std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`>& m,
			const :ref:`matcher_pass_callback<doxid-namespaceov_1a0a124d479a37653bc99b1b118d47fc79>`& callback
			);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_matcher_pass_1a525c64de11717629f6599042761eb844>`("ov::pass::MatcherPass");
		MatcherPass& :target:`operator =<doxid-classov_1_1pass_1_1_matcher_pass_1ae003cfdc27f2418f603f12b4f031ba3c>` (const MatcherPass&);
		bool :target:`apply<doxid-classov_1_1pass_1_1_matcher_pass_1afe5e71b978b3dc8274ea93bb6e7dcc23>`(std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> node);
	
		template <typename T, class... Args>
		std::shared_ptr<T> :target:`register_new_node<doxid-classov_1_1pass_1_1_matcher_pass_1a6e14fcb5d87373bab47d5778ea39ba55>`(Args&&... args);
	
		template <typename T>
		std::shared_ptr<T> :target:`register_new_node<doxid-classov_1_1pass_1_1_matcher_pass_1acb4756e168d3130377473123783c16fa>`(const std::shared_ptr<T>& node);
	
		std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`register_new_node_<doxid-classov_1_1pass_1_1_matcher_pass_1ae343beb91a81a3a6b43670726c7e7abe>`(const std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>& node);
		const std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>>& :target:`get_new_nodes<doxid-classov_1_1pass_1_1_matcher_pass_1abf2e6b740f5e27a13589f19b47e934af>`();
		void :target:`clear_new_nodes<doxid-classov_1_1pass_1_1_matcher_pass_1a9a3abba77cc94f47e1cdc4e064544d6a>`();
		std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`> :target:`get_matcher<doxid-classov_1_1pass_1_1_matcher_pass_1a69329c064bb3cb7268ae397f374648e8>`();
	};

	// direct descendants

	class :ref:`ConvertReduceBase<doxid-class_convert_reduce_base>`;
	class :ref:`AddAddFusion<doxid-classngraph_1_1pass_1_1_add_add_fusion>`;
	class :ref:`AddFakeQuantizeFusion<doxid-classngraph_1_1pass_1_1_add_fake_quantize_fusion>`;
	class :ref:`AddMultiplyFusion<doxid-classngraph_1_1pass_1_1_add_multiply_fusion>`;
	class :ref:`AlignEltwiseInputRanks<doxid-classngraph_1_1pass_1_1_align_eltwise_input_ranks>`;
	class :ref:`BatchNormDecomposition<doxid-classngraph_1_1pass_1_1_batch_norm_decomposition>`;
	class :ref:`BatchToSpaceFusion<doxid-classngraph_1_1pass_1_1_batch_to_space_fusion>`;
	class :ref:`BidirectionalGRUSequenceDecomposition<doxid-classngraph_1_1pass_1_1_bidirectional_g_r_u_sequence_decomposition>`;
	class :ref:`BidirectionalLSTMSequenceDecomposition<doxid-classngraph_1_1pass_1_1_bidirectional_l_s_t_m_sequence_decomposition>`;
	class :ref:`BidirectionalRNNSequenceDecomposition<doxid-classngraph_1_1pass_1_1_bidirectional_r_n_n_sequence_decomposition>`;
	class :ref:`BinarizeWeights<doxid-classngraph_1_1pass_1_1_binarize_weights>`;
	class :ref:`BroadcastConstRangeReplacement<doxid-classngraph_1_1pass_1_1_broadcast_const_range_replacement>`;
	class :ref:`BroadcastElementwiseFusion<doxid-classngraph_1_1pass_1_1_broadcast_elementwise_fusion>`;
	class :ref:`ClampFusion<doxid-classngraph_1_1pass_1_1_clamp_fusion>`;
	class :ref:`CompressQuantizeWeights<doxid-classngraph_1_1pass_1_1_compress_quantize_weights>`;
	class :ref:`ConvAddFusion<doxid-classngraph_1_1pass_1_1_conv_add_fusion>`;
	class :ref:`ConvertBatchToSpace<doxid-classngraph_1_1pass_1_1_convert_batch_to_space>`;
	class :ref:`ConvertBroadcast3<doxid-classngraph_1_1pass_1_1_convert_broadcast3>`;
	class :ref:`ConvertBroadcastToTiles<doxid-classngraph_1_1pass_1_1_convert_broadcast_to_tiles>`;
	class :ref:`ConvertConvolution<doxid-classngraph_1_1pass_1_1_convert_convolution>`;
	class :ref:`ConvertDeconvolution<doxid-classngraph_1_1pass_1_1_convert_deconvolution>`;
	class :ref:`ConvertDeformableConv8To1<doxid-classngraph_1_1pass_1_1_convert_deformable_conv8_to1>`;
	class :ref:`ConvertDepthToSpace<doxid-classngraph_1_1pass_1_1_convert_depth_to_space>`;
	class :ref:`ConvertDetectionOutput1ToDetectionOutput8<doxid-classngraph_1_1pass_1_1_convert_detection_output1_to_detection_output8>`;
	class :ref:`ConvertDetectionOutput8ToDetectionOutput1<doxid-classngraph_1_1pass_1_1_convert_detection_output8_to_detection_output1>`;
	class :ref:`ConvertDivide<doxid-classngraph_1_1pass_1_1_convert_divide>`;
	class :ref:`ConvertDivideWithConstant<doxid-classngraph_1_1pass_1_1_convert_divide_with_constant>`;
	class :ref:`ConvertGather0D<doxid-classngraph_1_1pass_1_1_convert_gather0_d>`;
	class :ref:`ConvertGather1ToGather7<doxid-classngraph_1_1pass_1_1_convert_gather1_to_gather7>`;
	class :ref:`ConvertGather7ToGather1<doxid-classngraph_1_1pass_1_1_convert_gather7_to_gather1>`;
	class :ref:`ConvertGather7ToGather8<doxid-classngraph_1_1pass_1_1_convert_gather7_to_gather8>`;
	class :ref:`ConvertGather8ToGather7<doxid-classngraph_1_1pass_1_1_convert_gather8_to_gather7>`;
	class :ref:`ConvertGatherToGatherIEMatcher<doxid-classngraph_1_1pass_1_1_convert_gather_to_gather_i_e_matcher>`;
	class :ref:`ConvertGatherTreeToGatherTreeIEMatcher<doxid-classngraph_1_1pass_1_1_convert_gather_tree_to_gather_tree_i_e_matcher>`;
	class :ref:`ConvertGELU<doxid-classngraph_1_1pass_1_1_convert_g_e_l_u>`;
	class :ref:`ConvertGroupConvolution<doxid-classngraph_1_1pass_1_1_convert_group_convolution>`;
	class :ref:`ConvertGroupDeconvolution<doxid-classngraph_1_1pass_1_1_convert_group_deconvolution>`;
	class :ref:`ConvertGRUCellMatcher<doxid-classngraph_1_1pass_1_1_convert_g_r_u_cell_matcher>`;
	class :ref:`ConvertGRUSequenceMatcher<doxid-classngraph_1_1pass_1_1_convert_g_r_u_sequence_matcher>`;
	class :ref:`ConvertGRUSequenceToTensorIterator<doxid-classngraph_1_1pass_1_1_convert_g_r_u_sequence_to_tensor_iterator>`;
	class :ref:`ConvertHardSigmoidToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_hard_sigmoid_to_legacy_matcher>`;
	class :ref:`ConvertInterpolate1ToInterpolate4<doxid-classngraph_1_1pass_1_1_convert_interpolate1_to_interpolate4>`;
	class :ref:`ConvertInterpolateToInterpOrResampleMatcher<doxid-classngraph_1_1pass_1_1_convert_interpolate_to_interp_or_resample_matcher>`;
	class :ref:`ConvertLRNToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_l_r_n_to_legacy_matcher>`;
	class :ref:`ConvertLSTMCellMatcher<doxid-classngraph_1_1pass_1_1_convert_l_s_t_m_cell_matcher>`;
	class :ref:`ConvertLSTMSequenceMatcher<doxid-classngraph_1_1pass_1_1_convert_l_s_t_m_sequence_matcher>`;
	class :ref:`ConvertLSTMSequenceToTensorIterator<doxid-classngraph_1_1pass_1_1_convert_l_s_t_m_sequence_to_tensor_iterator>`;
	class :ref:`ConvertMatMulToFC<doxid-classngraph_1_1pass_1_1_convert_mat_mul_to_f_c>`;
	class :ref:`ConvertMatMulToGemm<doxid-classngraph_1_1pass_1_1_convert_mat_mul_to_gemm>`;
	class :ref:`ConvertMatrixNmsToMatrixNmsIE<doxid-classngraph_1_1pass_1_1_convert_matrix_nms_to_matrix_nms_i_e>`;
	class :ref:`ConvertMaxPool1ToMaxPool8<doxid-classngraph_1_1pass_1_1_convert_max_pool1_to_max_pool8>`;
	class :ref:`ConvertMaxPool8ToMaxPool1<doxid-classngraph_1_1pass_1_1_convert_max_pool8_to_max_pool1>`;
	class :ref:`ConvertMinimum<doxid-classngraph_1_1pass_1_1_convert_minimum>`;
	class :ref:`ConvertMod<doxid-classngraph_1_1pass_1_1_convert_mod>`;
	class :ref:`ConvertMulAddToScaleShiftOrPower<doxid-classngraph_1_1pass_1_1_convert_mul_add_to_scale_shift_or_power>`;
	class :ref:`ConvertMulticlassNmsToMulticlassNmsIE<doxid-classngraph_1_1pass_1_1_convert_multiclass_nms_to_multiclass_nms_i_e>`;
	class :ref:`ConvertMVN1ToMVN6<doxid-classngraph_1_1pass_1_1_convert_m_v_n1_to_m_v_n6>`;
	class :ref:`ConvertNegative<doxid-classngraph_1_1pass_1_1_convert_negative>`;
	class :ref:`ConvertNMS1ToNMS5<doxid-classngraph_1_1pass_1_1_convert_n_m_s1_to_n_m_s5>`;
	class :ref:`ConvertNMS3ToNMS5<doxid-classngraph_1_1pass_1_1_convert_n_m_s3_to_n_m_s5>`;
	class :ref:`ConvertNMS4ToNMS5<doxid-classngraph_1_1pass_1_1_convert_n_m_s4_to_n_m_s5>`;
	class :ref:`ConvertNMS5ToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_n_m_s5_to_legacy_matcher>`;
	class :ref:`ConvertNMSToNMSIEInternal<doxid-classngraph_1_1pass_1_1_convert_n_m_s_to_n_m_s_i_e_internal>`;
	class :ref:`ConvertNMSToNMSIEMatcher<doxid-classngraph_1_1pass_1_1_convert_n_m_s_to_n_m_s_i_e_matcher>`;
	class :ref:`ConvertNormalizeL2ToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_normalize_l2_to_legacy_matcher>`;
	class :ref:`ConvertNormalizeL2WithMulToNormalizeIE<doxid-classngraph_1_1pass_1_1_convert_normalize_l2_with_mul_to_normalize_i_e>`;
	class :ref:`ConvertOneHotToOneHotIEMatcher<doxid-classngraph_1_1pass_1_1_convert_one_hot_to_one_hot_i_e_matcher>`;
	class :ref:`ConvertPadToGroupConvolution<doxid-classngraph_1_1pass_1_1_convert_pad_to_group_convolution>`;
	class :ref:`ConvertPadToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_pad_to_legacy_matcher>`;
	class :ref:`ConvertPowerToPowerIEMatcher<doxid-classngraph_1_1pass_1_1_convert_power_to_power_i_e_matcher>`;
	class :ref:`ConvertPReLUToReLUIE<doxid-classngraph_1_1pass_1_1_convert_p_re_l_u_to_re_l_u_i_e>`;
	class :ref:`ConvertPriorBox8To0<doxid-classngraph_1_1pass_1_1_convert_prior_box8_to0>`;
	class :ref:`ConvertProposal4ToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_proposal4_to_legacy_matcher>`;
	class :ref:`ConvertProposalToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_proposal_to_legacy_matcher>`;
	class :ref:`ConvertQuantizeDequantize<doxid-classngraph_1_1pass_1_1_convert_quantize_dequantize>`;
	class :ref:`ConvertRNNCellMatcher<doxid-classngraph_1_1pass_1_1_convert_r_n_n_cell_matcher>`;
	class :ref:`ConvertRNNSequenceMatcher<doxid-classngraph_1_1pass_1_1_convert_r_n_n_sequence_matcher>`;
	class :ref:`ConvertRNNSequenceToTensorIterator<doxid-classngraph_1_1pass_1_1_convert_r_n_n_sequence_to_tensor_iterator>`;
	class :ref:`ConvertROIAlign3To9<doxid-classngraph_1_1pass_1_1_convert_r_o_i_align3_to9>`;
	class :ref:`ConvertROIAlign9To3<doxid-classngraph_1_1pass_1_1_convert_r_o_i_align9_to3>`;
	class :ref:`ConvertScatterElementsToScatter<doxid-classngraph_1_1pass_1_1_convert_scatter_elements_to_scatter>`;
	class :ref:`ConvertSeluToSeluIEMatcher<doxid-classngraph_1_1pass_1_1_convert_selu_to_selu_i_e_matcher>`;
	class :ref:`ConvertShapeOf3<doxid-classngraph_1_1pass_1_1_convert_shape_of3>`;
	class :ref:`ConvertShuffleChannels3<doxid-classngraph_1_1pass_1_1_convert_shuffle_channels3>`;
	class :ref:`ConvertSoftMax1ToSoftMax8<doxid-classngraph_1_1pass_1_1_convert_soft_max1_to_soft_max8>`;
	class :ref:`ConvertSoftMax8ToSoftMax1<doxid-classngraph_1_1pass_1_1_convert_soft_max8_to_soft_max1>`;
	class :ref:`ConvertSpaceToBatch<doxid-classngraph_1_1pass_1_1_convert_space_to_batch>`;
	class :ref:`ConvertSpaceToDepth<doxid-classngraph_1_1pass_1_1_convert_space_to_depth>`;
	class :ref:`ConvertSqrtToPowerIEMatcher<doxid-classngraph_1_1pass_1_1_convert_sqrt_to_power_i_e_matcher>`;
	class :ref:`ConvertStridedSliceToCropMatcher<doxid-classngraph_1_1pass_1_1_convert_strided_slice_to_crop_matcher>`;
	class :ref:`ConvertSubtract<doxid-classngraph_1_1pass_1_1_convert_subtract>`;
	class :ref:`ConvertSwishToSwishIEMatcher<doxid-classngraph_1_1pass_1_1_convert_swish_to_swish_i_e_matcher>`;
	class :ref:`ConvertTensorIteratorToGRUSequence<doxid-classngraph_1_1pass_1_1_convert_tensor_iterator_to_g_r_u_sequence>`;
	class :ref:`ConvertTensorIteratorToLSTMSequence<doxid-classngraph_1_1pass_1_1_convert_tensor_iterator_to_l_s_t_m_sequence>`;
	class :ref:`ConvertTensorIteratorToRNNSequence<doxid-classngraph_1_1pass_1_1_convert_tensor_iterator_to_r_n_n_sequence>`;
	class :ref:`ConvertTileToLegacyMatcher<doxid-classngraph_1_1pass_1_1_convert_tile_to_legacy_matcher>`;
	class :ref:`ConvertTopK3<doxid-classngraph_1_1pass_1_1_convert_top_k3>`;
	class :ref:`ConvertTopKToTopKIEMatcher<doxid-classngraph_1_1pass_1_1_convert_top_k_to_top_k_i_e_matcher>`;
	class :ref:`ConvMultiplyFusion<doxid-classngraph_1_1pass_1_1_conv_multiply_fusion>`;
	class :ref:`ConvolutionBackpropDataMultiplyFusion<doxid-classngraph_1_1pass_1_1_convolution_backprop_data_multiply_fusion>`;
	class :ref:`ConvolutionMultiplyFusion<doxid-classngraph_1_1pass_1_1_convolution_multiply_fusion>`;
	class :ref:`ConvStridesPropagation<doxid-classngraph_1_1pass_1_1_conv_strides_propagation>`;
	class :ref:`ConvToBinaryConv<doxid-classngraph_1_1pass_1_1_conv_to_binary_conv>`;
	class :ref:`DeconvAddFusion<doxid-classngraph_1_1pass_1_1_deconv_add_fusion>`;
	class :ref:`DepthToSpaceFusion<doxid-classngraph_1_1pass_1_1_depth_to_space_fusion>`;
	class :ref:`DilatedConvolutionConverter<doxid-classngraph_1_1pass_1_1_dilated_convolution_converter>`;
	class :ref:`DisableConvertConstantFoldingOnConstPath<doxid-classngraph_1_1pass_1_1_disable_convert_constant_folding_on_const_path>`;
	class :ref:`DisableRandomUniformConstantFolding<doxid-classngraph_1_1pass_1_1_disable_random_uniform_constant_folding>`;
	class :ref:`DisableShapeOfConstantFolding<doxid-classngraph_1_1pass_1_1_disable_shape_of_constant_folding>`;
	class :ref:`DivideFusion<doxid-classngraph_1_1pass_1_1_divide_fusion>`;
	class :ref:`DropoutWithRandomUniformReplacer<doxid-classngraph_1_1pass_1_1_dropout_with_random_uniform_replacer>`;
	class :ref:`EinsumDecomposition<doxid-classngraph_1_1pass_1_1_einsum_decomposition>`;
	class :ref:`EliminateConcat<doxid-classngraph_1_1pass_1_1_eliminate_concat>`;
	class :ref:`EliminateConvert<doxid-classngraph_1_1pass_1_1_eliminate_convert>`;
	class :ref:`EliminateConvertNonZero<doxid-classngraph_1_1pass_1_1_eliminate_convert_non_zero>`;
	class :ref:`EliminateEltwise<doxid-classngraph_1_1pass_1_1_eliminate_eltwise>`;
	class :ref:`EliminateGatherUnsqueeze<doxid-classngraph_1_1pass_1_1_eliminate_gather_unsqueeze>`;
	class :ref:`EliminatePad<doxid-classngraph_1_1pass_1_1_eliminate_pad>`;
	class :ref:`EliminateSplit<doxid-classngraph_1_1pass_1_1_eliminate_split>`;
	class :ref:`EliminateSqueeze<doxid-classngraph_1_1pass_1_1_eliminate_squeeze>`;
	class :ref:`EliminateTranspose<doxid-classngraph_1_1pass_1_1_eliminate_transpose>`;
	class :ref:`EliminateUnsqueezeGather<doxid-classngraph_1_1pass_1_1_eliminate_unsqueeze_gather>`;
	class :ref:`FakeQuantizeDecomposition<doxid-classngraph_1_1pass_1_1_fake_quantize_decomposition>`;
	class :ref:`FakeQuantizeMulFusion<doxid-classngraph_1_1pass_1_1_fake_quantize_mul_fusion>`;
	class :ref:`FakeQuantizeReshapeFusion<doxid-classngraph_1_1pass_1_1_fake_quantize_reshape_fusion>`;
	class :ref:`FullyConnectedBiasFusion<doxid-classngraph_1_1pass_1_1_fully_connected_bias_fusion>`;
	class :ref:`GatherNegativeConstIndicesNormalize<doxid-classngraph_1_1pass_1_1_gather_negative_const_indices_normalize>`;
	class :ref:`GatherNopElimination<doxid-classngraph_1_1pass_1_1_gather_nop_elimination>`;
	class :ref:`Gelu7Downgrade<doxid-classngraph_1_1pass_1_1_gelu7_downgrade>`;
	class :ref:`GeluFusionWithErfOne<doxid-classngraph_1_1pass_1_1_gelu_fusion_with_erf_one>`;
	class :ref:`GeluFusionWithErfThree<doxid-classngraph_1_1pass_1_1_gelu_fusion_with_erf_three>`;
	class :ref:`GeluFusionWithErfTwo<doxid-classngraph_1_1pass_1_1_gelu_fusion_with_erf_two>`;
	class :ref:`GroupConvolutionBackpropDataMultiplyFusion<doxid-classngraph_1_1pass_1_1_group_convolution_backprop_data_multiply_fusion>`;
	class :ref:`GroupConvolutionMultiplyFusion<doxid-classngraph_1_1pass_1_1_group_convolution_multiply_fusion>`;
	class :ref:`GroupedGatherElimination<doxid-classngraph_1_1pass_1_1_grouped_gather_elimination>`;
	class :ref:`GRUCellDecomposition<doxid-classngraph_1_1pass_1_1_g_r_u_cell_decomposition>`;
	class :ref:`HSigmoidDecomposition<doxid-classngraph_1_1pass_1_1_h_sigmoid_decomposition>`;
	class :ref:`HSigmoidFusionWithClampDiv<doxid-classngraph_1_1pass_1_1_h_sigmoid_fusion_with_clamp_div>`;
	class :ref:`HSigmoidFusionWithClampMul<doxid-classngraph_1_1pass_1_1_h_sigmoid_fusion_with_clamp_mul>`;
	class :ref:`HSigmoidFusionWithoutRelu<doxid-classngraph_1_1pass_1_1_h_sigmoid_fusion_without_relu>`;
	class :ref:`HSigmoidFusionWithReluDiv<doxid-classngraph_1_1pass_1_1_h_sigmoid_fusion_with_relu_div>`;
	class :ref:`HSigmoidFusionWithReluMul<doxid-classngraph_1_1pass_1_1_h_sigmoid_fusion_with_relu_mul>`;
	class :ref:`HSwishDecomposition<doxid-classngraph_1_1pass_1_1_h_swish_decomposition>`;
	class :ref:`HSwishFusionWithClamp<doxid-classngraph_1_1pass_1_1_h_swish_fusion_with_clamp>`;
	class :ref:`HSwishFusionWithHSigmoid<doxid-classngraph_1_1pass_1_1_h_swish_fusion_with_h_sigmoid>`;
	class :ref:`HSwishFusionWithReluDiv<doxid-classngraph_1_1pass_1_1_h_swish_fusion_with_relu_div>`;
	class :ref:`HSwishFusionWithReluMul<doxid-classngraph_1_1pass_1_1_h_swish_fusion_with_relu_mul>`;
	class :ref:`InitConstMask<doxid-classngraph_1_1pass_1_1_init_const_mask>`;
	class :ref:`InterpolateSequenceFusion<doxid-classngraph_1_1pass_1_1_interpolate_sequence_fusion>`;
	class :ref:`LeakyReluFusion<doxid-classngraph_1_1pass_1_1_leaky_relu_fusion>`;
	class :ref:`LogSoftmaxDecomposition<doxid-classngraph_1_1pass_1_1_log_softmax_decomposition>`;
	class :ref:`ConvertSubtractConstant<doxid-classngraph_1_1pass_1_1low__precision_1_1_convert_subtract_constant>`;
	class :ref:`LayerTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation>`;
	class :ref:`PullReshapeThroughDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_pull_reshape_through_dequantization>`;
	class :ref:`PullTransposeThroughDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_pull_transpose_through_dequantization>`;
	class :ref:`LSTMCellDecomposition<doxid-classngraph_1_1pass_1_1_l_s_t_m_cell_decomposition>`;
	class :ref:`MatMulConstTransposesExtraction<doxid-classngraph_1_1pass_1_1_mat_mul_const_transposes_extraction>`;
	class :ref:`MatMulMultiplyFusion<doxid-classngraph_1_1pass_1_1_mat_mul_multiply_fusion>`;
	class :ref:`MishFusion<doxid-classngraph_1_1pass_1_1_mish_fusion>`;
	class :ref:`MulFakeQuantizeFusion<doxid-classngraph_1_1pass_1_1_mul_fake_quantize_fusion>`;
	class :ref:`MultiplyConvolutionBackpropDataFusion<doxid-classngraph_1_1pass_1_1_multiply_convolution_backprop_data_fusion>`;
	class :ref:`MultiplyConvolutionFusion<doxid-classngraph_1_1pass_1_1_multiply_convolution_fusion>`;
	class :ref:`MultiplyGroupConvolutionBackpropDataFusion<doxid-classngraph_1_1pass_1_1_multiply_group_convolution_backprop_data_fusion>`;
	class :ref:`MultiplyGroupConvolutionFusion<doxid-classngraph_1_1pass_1_1_multiply_group_convolution_fusion>`;
	class :ref:`MultiplyMultiplyFusion<doxid-classngraph_1_1pass_1_1_multiply_multiply_fusion>`;
	class :ref:`MVN6Decomposition<doxid-classngraph_1_1pass_1_1_m_v_n6_decomposition>`;
	class :ref:`MVNFusionWithConstantsInside<doxid-classngraph_1_1pass_1_1_m_v_n_fusion_with_constants_inside>`;
	class :ref:`MVNFusionWithoutConstants<doxid-classngraph_1_1pass_1_1_m_v_n_fusion_without_constants>`;
	class :ref:`NearestNeighborUpsamplingFusion<doxid-classngraph_1_1pass_1_1_nearest_neighbor_upsampling_fusion>`;
	class :ref:`NormalizeL2Decomposition<doxid-classngraph_1_1pass_1_1_normalize_l2_decomposition>`;
	class :ref:`NormalizeL2Fusion<doxid-classngraph_1_1pass_1_1_normalize_l2_fusion>`;
	class :ref:`PadFusionAvgPool<doxid-classngraph_1_1pass_1_1_pad_fusion_avg_pool>`;
	class :ref:`PadFusionConvolution<doxid-classngraph_1_1pass_1_1_pad_fusion_convolution>`;
	class :ref:`PadFusionConvolutionBackpropData<doxid-classngraph_1_1pass_1_1_pad_fusion_convolution_backprop_data>`;
	class :ref:`PadFusionGroupConvolution<doxid-classngraph_1_1pass_1_1_pad_fusion_group_convolution>`;
	class :ref:`PadFusionGroupConvolutionBackpropData<doxid-classngraph_1_1pass_1_1_pad_fusion_group_convolution_backprop_data>`;
	class :ref:`PReluFusionMultiplyAdd<doxid-classngraph_1_1pass_1_1_p_relu_fusion_multiply_add>`;
	class :ref:`PReluFusionMultiplySub<doxid-classngraph_1_1pass_1_1_p_relu_fusion_multiply_sub>`;
	class :ref:`PReluFusionNegativeAdd<doxid-classngraph_1_1pass_1_1_p_relu_fusion_negative_add>`;
	class :ref:`PReluFusionNegativeSub<doxid-classngraph_1_1pass_1_1_p_relu_fusion_negative_sub>`;
	class :ref:`Proposal1Scales<doxid-classngraph_1_1pass_1_1_proposal1_scales>`;
	class :ref:`Proposal4Scales<doxid-classngraph_1_1pass_1_1_proposal4_scales>`;
	class :ref:`PullSqueezeThroughEltwise<doxid-classngraph_1_1pass_1_1_pull_squeeze_through_eltwise>`;
	class :ref:`PullTransposeThroughFQUp<doxid-classngraph_1_1pass_1_1_pull_transpose_through_f_q_up>`;
	class :ref:`RandomUniformFusion<doxid-classngraph_1_1pass_1_1_random_uniform_fusion>`;
	class :ref:`ReduceL1Decomposition<doxid-classngraph_1_1pass_1_1_reduce_l1_decomposition>`;
	class :ref:`ReduceL2Decomposition<doxid-classngraph_1_1pass_1_1_reduce_l2_decomposition>`;
	class :ref:`ReluFakeQuantizeFusion<doxid-classngraph_1_1pass_1_1_relu_fake_quantize_fusion>`;
	class :ref:`RemoveFilteringBoxesBySize<doxid-classngraph_1_1pass_1_1_remove_filtering_boxes_by_size>`;
	class :ref:`ReplaceConcatReduceByMinOrMax<doxid-classngraph_1_1pass_1_1_replace_concat_reduce_by_min_or_max>`;
	class :ref:`Reshape1DAvgPool<doxid-classngraph_1_1pass_1_1_reshape1_d_avg_pool>`;
	class :ref:`Reshape1DConvolution<doxid-classngraph_1_1pass_1_1_reshape1_d_convolution>`;
	class :ref:`Reshape1DMaxPool<doxid-classngraph_1_1pass_1_1_reshape1_d_max_pool>`;
	class :ref:`ReshapeAMatMul<doxid-classngraph_1_1pass_1_1_reshape_a_mat_mul>`;
	class :ref:`ReshapeBMatMul<doxid-classngraph_1_1pass_1_1_reshape_b_mat_mul>`;
	class :ref:`ReshapeFullyConnected<doxid-classngraph_1_1pass_1_1_reshape_fully_connected>`;
	class :ref:`ReshapeFullyConnectedFusion<doxid-classngraph_1_1pass_1_1_reshape_fully_connected_fusion>`;
	class :ref:`ReshapeSequenceFusion<doxid-classngraph_1_1pass_1_1_reshape_sequence_fusion>`;
	class :ref:`ReshapeTo1D<doxid-classngraph_1_1pass_1_1_reshape_to1_d>`;
	class :ref:`RNNCellDecomposition<doxid-classngraph_1_1pass_1_1_r_n_n_cell_decomposition>`;
	class :ref:`ShuffleChannelsFusion<doxid-classngraph_1_1pass_1_1_shuffle_channels_fusion>`;
	class :ref:`SkipGatherBeforeTransposeAndReshape<doxid-classngraph_1_1pass_1_1_skip_gather_before_transpose_and_reshape>`;
	class :ref:`SliceToStridedSlice<doxid-classngraph_1_1pass_1_1_slice_to_strided_slice>`;
	class :ref:`SoftmaxDecomposition<doxid-classngraph_1_1pass_1_1_softmax_decomposition>`;
	class :ref:`SoftmaxFusion<doxid-classngraph_1_1pass_1_1_softmax_fusion>`;
	class :ref:`SoftPlusDecomposition<doxid-classngraph_1_1pass_1_1_soft_plus_decomposition>`;
	class :ref:`SoftPlusFusion<doxid-classngraph_1_1pass_1_1_soft_plus_fusion>`;
	class :ref:`SoftPlusToMishFusion<doxid-classngraph_1_1pass_1_1_soft_plus_to_mish_fusion>`;
	class :ref:`SpaceToBatchFusion<doxid-classngraph_1_1pass_1_1_space_to_batch_fusion>`;
	class :ref:`SplitConcatPairToInterpolateFusion<doxid-classngraph_1_1pass_1_1_split_concat_pair_to_interpolate_fusion>`;
	class :ref:`SplitSqueezeConcatFusion<doxid-classngraph_1_1pass_1_1_split_squeeze_concat_fusion>`;
	class :ref:`SqueezeStridedSlice<doxid-classngraph_1_1pass_1_1_squeeze_strided_slice>`;
	class :ref:`StridedSliceSqueeze<doxid-classngraph_1_1pass_1_1_strided_slice_squeeze>`;
	class :ref:`SubtractFusion<doxid-classngraph_1_1pass_1_1_subtract_fusion>`;
	class :ref:`SupportedNodesStridesPropagation<doxid-classngraph_1_1pass_1_1_supported_nodes_strides_propagation>`;
	class :ref:`SwishFusionWithBeta<doxid-classngraph_1_1pass_1_1_swish_fusion_with_beta>`;
	class :ref:`SwishFusionWithoutBeta<doxid-classngraph_1_1pass_1_1_swish_fusion_without_beta>`;
	class :ref:`SwishFusionWithSigmoid<doxid-classngraph_1_1pass_1_1_swish_fusion_with_sigmoid>`;
	class :ref:`SwishFusionWithSigmoidWithBeta<doxid-classngraph_1_1pass_1_1_swish_fusion_with_sigmoid_with_beta>`;
	class :ref:`TransposeConvert<doxid-classngraph_1_1pass_1_1_transpose_convert>`;
	class :ref:`TransposeEltwise<doxid-classngraph_1_1pass_1_1_transpose_eltwise>`;
	class :ref:`TransposeFQReduction<doxid-classngraph_1_1pass_1_1_transpose_f_q_reduction>`;
	class :ref:`TransposeFuse<doxid-classngraph_1_1pass_1_1_transpose_fuse>`;
	class :ref:`TransposeMatMul<doxid-classngraph_1_1pass_1_1_transpose_mat_mul>`;
	class :ref:`TransposeReduction<doxid-classngraph_1_1pass_1_1_transpose_reduction>`;
	class :ref:`TransposeReshapeEliminationForMatmul<doxid-classngraph_1_1pass_1_1_transpose_reshape_elimination_for_matmul>`;
	class :ref:`TransposeToReshape<doxid-classngraph_1_1pass_1_1_transpose_to_reshape>`;
	class :ref:`UnsupportedNodesStridesPropagation<doxid-classngraph_1_1pass_1_1_unsupported_nodes_strides_propagation>`;
	class :ref:`WeightsDequantizeToFakeQuantize<doxid-classngraph_1_1pass_1_1_weights_dequantize_to_fake_quantize>`;
	class :ref:`WrapInterpolateIntoTransposes<doxid-classngraph_1_1pass_1_1_wrap_interpolate_into_transposes>`;
	class :ref:`ZeroPointOptimizer<doxid-classngraph_1_1pass_1_1_zero_point_optimizer>`;
	template :ref:`ConvertConstantsToScalars<doxid-classngraph_1_1snippets_1_1pass_1_1_convert_constants_to_scalars>`;
	class :ref:`ConvertPowerToPowerStatic<doxid-classngraph_1_1snippets_1_1pass_1_1_convert_power_to_power_static>`;
	template :ref:`InsertLoad<doxid-classngraph_1_1snippets_1_1pass_1_1_insert_load>`;
	template :ref:`InsertMoveBroadcast<doxid-classngraph_1_1snippets_1_1pass_1_1_insert_move_broadcast>`;
	template :ref:`InsertStore<doxid-classngraph_1_1snippets_1_1pass_1_1_insert_store>`;
	template :ref:`LoadMoveBroadcastToBroadcastLoad<doxid-classngraph_1_1snippets_1_1pass_1_1_load_move_broadcast_to_broadcast_load>`;
	template :ref:`ReplaceLoadsWithScalarLoads<doxid-classngraph_1_1snippets_1_1pass_1_1_replace_loads_with_scalar_loads>`;
	template :ref:`ReplaceStoresWithScalarStores<doxid-classngraph_1_1snippets_1_1pass_1_1_replace_stores_with_scalar_stores>`;
	template :ref:`TokenizeSnippets<doxid-classngraph_1_1snippets_1_1pass_1_1_tokenize_snippets>`;
	class :ref:`AddOldApiMapToParameters<doxid-classov_1_1pass_1_1_add_old_api_map_to_parameters>`;
	class :ref:`CompressFloatConstantsImpl<doxid-classov_1_1pass_1_1_compress_float_constants_impl>`;
	class :ref:`DisableDecompressionConvertConstantFolding<doxid-classov_1_1pass_1_1_disable_decompression_convert_constant_folding>`;
	class :ref:`DivisionByZeroFP16Resolver<doxid-classov_1_1pass_1_1_division_by_zero_f_p16_resolver>`;
	class :ref:`EnableDecompressionConvertConstantFolding<doxid-classov_1_1pass_1_1_enable_decompression_convert_constant_folding>`;
	class :ref:`RemoveConcatZeroDimInput<doxid-classov_1_1pass_1_1_remove_concat_zero_dim_input>`;
	class :ref:`RemoveMultiSubGraphOpDanglingParams<doxid-classov_1_1pass_1_1_remove_multi_sub_graph_op_dangling_params>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`;

		// methods
	
		bool :ref:`get_property<doxid-classov_1_1pass_1_1_pass_base_1a3107964f6c4d4bf1d3fbc2bf97ccc0b8>`(const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& prop_mask) const;
		void :ref:`set_name<doxid-classov_1_1pass_1_1_pass_base_1a78ddde2a8770041d2f23ce59af908f5d>`(const std::string& name);
		std::string :ref:`get_name<doxid-classov_1_1pass_1_1_pass_base_1a6cd527d2176f1350dd999dc4632a576b>`() const;
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_base_1a6a56827a1cf76be99289bab703982869>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_pass_base_1abe74bba4b563ad367f2fdc7836016391>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);
		std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> :ref:`get_pass_config<doxid-classov_1_1pass_1_1_pass_base_1a4902f6ed9322e0fd38810d701f4409df>`();
		bool :ref:`m_transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1a568e5b1f0e01f221d36dffabbf156b3d>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		bool :ref:`transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		virtual const :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`& :ref:`get_type_info<doxid-classov_1_1pass_1_1_pass_base_1ab7020db2fcebc9b6e0741a451778fb0c>`() const = 0;

.. _details-classov_1_1pass_1_1_matcher_pass:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` is a basic block for pattern based transformations. It describes pattern and action that is applied if pattern is matched.

:ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` consists of Matcher and matcher_pass_callback that needs to be implemented and finally registered by using



.. rubric:: See also:

:ref:`register_matcher <doxid-classov_1_1pass_1_1_matcher_pass_1af12b8f0f93b6a7825bcd74b7dd0f5f18>`. :ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` can be executed on node within

:ref:`apply <doxid-classov_1_1pass_1_1_matcher_pass_1afe5e71b978b3dc8274ea93bb6e7dcc23>` method. To run matcher :ref:`pass <doxid-namespaceov_1_1pass>` on Function use :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>`. In addition :ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` provides a way for adding new operations into :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` execution queue. That means that operations that were created inside transformation callback can be added for matching. To register node use

:ref:`register_new_node <doxid-classov_1_1pass_1_1_matcher_pass_1a6e14fcb5d87373bab47d5778ea39ba55>` method. :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` automatically takes registered nodes and put them to execution queue. If multiple nodes were register make sure that they were registered in topological order. Note: when implementing :ref:`pattern <doxid-namespaceov_1_1pass_1_1pattern>` for Matcher make sure that root node is an operation from opset or has :ref:`ov::pass::pattern::op::WrapType <doxid-classov_1_1pass_1_1pattern_1_1op_1_1_wrap_type>`. That will help :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` to execute matcher passes more efficient.


