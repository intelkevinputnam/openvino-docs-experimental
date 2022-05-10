.. index:: pair: namespace; ngraph::pass::low_precision
.. _doxid-namespacengraph_1_1pass_1_1low__precision:

namespace ngraph::pass::low_precision
=====================================

.. toctree::
	:hidden:

	itt <namespacengraph_1_1pass_1_1low_precision_1_1itt.rst>
	precision_set <namespacengraph_1_1pass_1_1low_precision_1_1precision_set.rst>
	levels <enumngraph_1_1pass_1_1low_precision_1_1levels.rst>
	AssignAndReadValueTransformation <classngraph_1_1pass_1_1low_precision_1_1AssignAndReadValueTransformation.rst>
	ConvertTransformation <classngraph_1_1pass_1_1low_precision_1_1ConvertTransformation.rst>
	DataPrecision <classngraph_1_1pass_1_1low_precision_1_1DataPrecision.rst>
	Exception <classngraph_1_1pass_1_1low_precision_1_1Exception.rst>
	FakeQuantizeDequantization <classngraph_1_1pass_1_1low_precision_1_1FakeQuantizeDequantization.rst>
	InferenceEngineLptException <classngraph_1_1pass_1_1low_precision_1_1InferenceEngineLptException.rst>
	LowPrecision <classngraph_1_1pass_1_1low_precision_1_1LowPrecision.rst>
	MarkupOptimizations <classngraph_1_1pass_1_1low_precision_1_1MarkupOptimizations.rst>
	MoveFakeQuantize <classngraph_1_1pass_1_1low_precision_1_1MoveFakeQuantize.rst>
	NetworkHelper <classngraph_1_1pass_1_1low_precision_1_1NetworkHelper.rst>
	PortQuantizationGranularityRestriction <classngraph_1_1pass_1_1low_precision_1_1PortQuantizationGranularityRestriction.rst>
	PrecisionsRestriction <classngraph_1_1pass_1_1low_precision_1_1PrecisionsRestriction.rst>
	QuantizationDetails <classngraph_1_1pass_1_1low_precision_1_1QuantizationDetails.rst>
	QuantizationGranularityRestriction <classngraph_1_1pass_1_1low_precision_1_1QuantizationGranularityRestriction.rst>
	TypeRelaxedReplacer <classngraph_1_1pass_1_1low_precision_1_1TypeRelaxedReplacer.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace low_precision {

	// namespaces

	namespace :ref:`ngraph::pass::low_precision::itt<doxid-namespacengraph_1_1pass_1_1low__precision_1_1itt>`;
		namespace :ref:`ngraph::pass::low_precision::itt::domains<doxid-namespacengraph_1_1pass_1_1low__precision_1_1itt_1_1domains>`;
	namespace :ref:`ngraph::pass::low_precision::precision_set<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set>`;

	// typedefs

	typedef std::tuple<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :target:`FakeQuantizeDequantizationValues<doxid-namespacengraph_1_1pass_1_1low__precision_1aca276710287c1a293770619348ca5054>`;
	typedef std::shared_ptr<:ref:`LayerTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation>`> :target:`LayerTransformationPtr<doxid-namespacengraph_1_1pass_1_1low__precision_1a1a825855bf397cff490e51672b30218a>`;

	// enums

	enum :ref:`levels<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950d>`;

	// classes

	class :ref:`AddTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation>`;
	class :ref:`AlignQuantizationIntervals<doxid-classngraph_1_1pass_1_1low__precision_1_1_align_quantization_intervals>`;
	class :ref:`AlignQuantizationParameters<doxid-classngraph_1_1pass_1_1low__precision_1_1_align_quantization_parameters>`;
	class :ref:`AssignAndReadValueTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_assign_and_read_value_transformation>`;
	class :ref:`AvgPoolTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_avg_pool_transformation>`;
	class :ref:`ClampTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_clamp_transformation>`;
	class :ref:`ConcatTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_concat_transformation>`;
	class :ref:`ConvertSubtractConstant<doxid-classngraph_1_1pass_1_1low__precision_1_1_convert_subtract_constant>`;
	class :ref:`ConvertTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_convert_transformation>`;
	class :ref:`ConvolutionBackpropDataTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_convolution_backprop_data_transformation>`;
	class :ref:`ConvolutionTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_convolution_transformation>`;
	template <
		typename AttributeType,
		typename OperationType = ngraph::pattern::op::Label
		>
	class :ref:`CreateAttribute<doxid-classngraph_1_1pass_1_1low__precision_1_1_create_attribute>`;
	template <typename AttributeType, typename OperationType>
	class :ref:`CreatePrecisionsDependentAttribute<doxid-classngraph_1_1pass_1_1low__precision_1_1_create_precisions_dependent_attribute>`;
	class :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`;
	class :ref:`DepthToSpaceTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_depth_to_space_transformation>`;
	class :ref:`EltwiseBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_eltwise_base_transformation>`;
	class :ref:`Exception<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception>`;
	class :ref:`FakeQuantizeDecompositionTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_decomposition_transformation>`;
	class :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>`;
	class :ref:`FakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_transformation>`;
	class :ref:`FoldConvertTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fold_convert_transformation>`;
	class :ref:`FoldFakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fold_fake_quantize_transformation>`;
	class :ref:`FuseConvertTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fuse_convert_transformation>`;
	class :ref:`FuseMultiplyToFakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fuse_multiply_to_fake_quantize_transformation>`;
	class :ref:`FuseSubtractToFakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fuse_subtract_to_fake_quantize_transformation>`;
	class :ref:`GroupConvolutionTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_group_convolution_transformation>`;
	class :ref:`InferenceEngineLptException<doxid-classngraph_1_1pass_1_1low__precision_1_1_inference_engine_lpt_exception>`;
	class :ref:`InterpolateTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_interpolate_transformation>`;
	class :ref:`LayerTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation>`;
	class :ref:`LowPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision>`;
	class :ref:`MVNTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_m_v_n_transformation>`;
	class :ref:`MarkupAvgPoolPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_avg_pool_precision_preserved>`;
	class :ref:`MarkupCanBeQuantized<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_can_be_quantized>`;
	class :ref:`MarkupOptimizations<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_optimizations>`;
	class :ref:`MarkupPrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions>`;
	class :ref:`MarkupQuantizationGranularity<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity>`;
	class :ref:`MatMulTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_mat_mul_transformation>`;
	class :ref:`MaxPoolTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_max_pool_transformation>`;
	class :ref:`MoveFakeQuantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_move_fake_quantize>`;
	class :ref:`MultiplyToGroupConvolutionTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_multiply_to_group_convolution_transformation>`;
	class :ref:`MultiplyTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_multiply_transformation>`;
	class :ref:`NetworkHelper<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper>`;
	class :ref:`NormalizeL2Transformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_normalize_l2_transformation>`;
	class :ref:`PReluTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_p_relu_transformation>`;
	class :ref:`PadTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_pad_transformation>`;
	class :ref:`PortQuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_port_quantization_granularity_restriction>`;
	class :ref:`PrecisionsRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction>`;
	class :ref:`PropagatePrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_precisions>`;
	template <class AttributeType>
	class :ref:`PropagateSharedValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_shared_value>`;
	template <typename AttributeType>
	class :ref:`PropagateThroughPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved>`;
	template <typename AttributeType>
	class :ref:`PropagateToInput<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input>`;
	class :ref:`PullReshapeThroughDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_pull_reshape_through_dequantization>`;
	class :ref:`PullTransposeThroughDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_pull_transpose_through_dequantization>`;
	class :ref:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details>`;
	class :ref:`QuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction>`;
	class :ref:`ReduceBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reduce_base_transformation>`;
	class :ref:`ReduceMaxTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reduce_max_transformation>`;
	class :ref:`ReduceMeanTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reduce_mean_transformation>`;
	class :ref:`ReduceMinTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reduce_min_transformation>`;
	class :ref:`ReduceSumTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reduce_sum_transformation>`;
	class :ref:`ReluTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_relu_transformation>`;
	class :ref:`ReshapeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reshape_transformation>`;
	class :ref:`ShuffleChannelsTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_shuffle_channels_transformation>`;
	class :ref:`SplitTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_split_transformation>`;
	class :ref:`SqueezeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_squeeze_transformation>`;
	class :ref:`StridedSliceTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_strided_slice_transformation>`;
	class :ref:`SubtractTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_subtract_transformation>`;
	class :ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`;
	class :ref:`TransparentBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_transparent_base_transformation>`;
	class :ref:`TransposeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_transpose_transformation>`;
	class :ref:`TypeRelaxedReplacer<doxid-classngraph_1_1pass_1_1low__precision_1_1_type_relaxed_replacer>`;
	class :ref:`UnsqueezeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_unsqueeze_transformation>`;
	template <
		typename AttributeType,
		typename ExpectedAttributeType = AttributeType
		>
	class :ref:`UpdateSharedPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved>`;
	class :ref:`VariadicSplitTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_variadic_split_transformation>`;
	class :ref:`WeightableLayerTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_weightable_layer_transformation>`;

	// global variables

	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`AlignQuantizationIntervals<doxid-namespacengraph_1_1pass_1_1low__precision_1a3f18cb312617fe35ce977111d80db4c0>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`AlignQuantizationParameters<doxid-namespacengraph_1_1pass_1_1low__precision_1a939bfc93787da0a3c8b2c4658d8a1759>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`BaseMatcherPass<doxid-namespacengraph_1_1pass_1_1low__precision_1a7af48c37e655e44615ea0155d1a7e336>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`ConvertSubtractConstant<doxid-namespacengraph_1_1pass_1_1low__precision_1aab56f59c86042f4bf0c32ac6cc4a2f08>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`TypeRelaxedReplacer<doxid-namespacengraph_1_1pass_1_1low__precision_1a04fb6bc0b2aee4f90f832dd8e7975ada>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`MarkupOptimizations<doxid-namespacengraph_1_1pass_1_1low__precision_1af96d42c6cb0599578ec0c3a288209f00>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`LowPrecision<doxid-namespacengraph_1_1pass_1_1low__precision_1a5c942b2cb1d5ae3e95a46d22b640569d>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`MarkupAvgPoolPrecisionPreserved<doxid-namespacengraph_1_1pass_1_1low__precision_1a33091924af8a6eba4b19fcd9f67217f3>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`MarkupCanBeQuantized<doxid-namespacengraph_1_1pass_1_1low__precision_1a9f80e506518f764f819495781b4cf648>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`MarkupPrecisions<doxid-namespacengraph_1_1pass_1_1low__precision_1a3ad0998fffa609dfbb131b7cf9f23309>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`MarkupQuantizationGranularity<doxid-namespacengraph_1_1pass_1_1low__precision_1ab88307a00e07269b22be5c063455f4bc>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`PropagatePrecisions<doxid-namespacengraph_1_1pass_1_1low__precision_1a2bbd65f294f8d2eea3a0aba22f17ab25>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`PropagateSharedValue<doxid-namespacengraph_1_1pass_1_1low__precision_1ac4c8401e6013c0f8a04979e427879d08>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`PullReshapeThroughDequantization<doxid-namespacengraph_1_1pass_1_1low__precision_1a03e607cbea46d15c24ab15b52e7d083d>`;
	class :ref:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>` :target:`PullTransposeThroughDequantization<doxid-namespacengraph_1_1pass_1_1low__precision_1a0028f9e7af5acc67a74984df17e24ce9>`;

	// global functions

	bool :target:`operator ==<doxid-namespacengraph_1_1pass_1_1low__precision_1ad06ac6d3beadc0d2071026ef99c09b2a>` (const :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`& value1, const :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`& value2);
	bool :target:`operator !=<doxid-namespacengraph_1_1pass_1_1low__precision_1a745ebf3edb6c81423a0d4187f26ad24a>` (const :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`& value1, const :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`& value2);
	std::ostream& :target:`operator <<<doxid-namespacengraph_1_1pass_1_1low__precision_1a026bb74dff21087e85d2fdb11f0287b7>` (std::ostream& os, const :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`& value);

	template <typename T>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_op_pattern<doxid-namespacengraph_1_1pass_1_1low__precision_1a78197e2a1dae227df709d06f7e81e113>`(const :ref:`ngraph::NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& args);

	template <typename T, typename... Args>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`fold<doxid-namespacengraph_1_1pass_1_1low__precision_1a8028a8546ab5dc37ba7614f9bff648d1>`(Args&&... args);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`foldConvert<doxid-namespacengraph_1_1pass_1_1low__precision_1ad8fd140652f6003193ca1120a772faa5>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` targetPrecision
		);

	template <typename T, typename... Args>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`fold_reshape<doxid-namespacengraph_1_1pass_1_1low__precision_1a3948d330eef96eb0dd520b2ba871ec8f>`(Args&&... args);

	template <typename T>
	:ref:`ov::Any<doxid-classov_1_1_any>` :target:`getAttribute<doxid-namespacengraph_1_1pass_1_1low__precision_1a4b9be189e57c60fecacf646eabbe5575>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

	template <typename T>
	:ref:`ov::Any<doxid-classov_1_1_any>` :target:`getAttribute<doxid-namespacengraph_1_1pass_1_1low__precision_1ad5ed8f2f377f7de406c20167fa4cea36>`(const :ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>& input);

	template <typename T>
	:ref:`ov::Any<doxid-classov_1_1_any>` :target:`getAttributeFromOutput<doxid-namespacengraph_1_1pass_1_1low__precision_1ae119795439130f88b49e84f025dafc38>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output);

	bool :target:`isDisabled<doxid-namespacengraph_1_1pass_1_1low__precision_1a623a572dbf8b6f1ca14c5b1ed7e52beb>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	std::ostream& :target:`operator <<<doxid-namespacengraph_1_1pass_1_1low__precision_1a5e0dc19a4813091a14f4232e1869ba68>` (std::ostream& os, const :ref:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details>`& value);

	} // namespace low_precision
