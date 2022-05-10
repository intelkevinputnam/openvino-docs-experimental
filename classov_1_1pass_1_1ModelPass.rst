.. index:: pair: class; ov::pass::ModelPass
.. _doxid-classov_1_1pass_1_1_model_pass:

class ov::pass::ModelPass
=========================



Base class for :ref:`Model <doxid-classov_1_1_model>` passes.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <pass.hpp>
	
	class ModelPass: public :ref:`ov::pass::PassBase<doxid-classov_1_1pass_1_1_pass_base>`
	{
	public:
		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_model_pass_1a718f43e809339887547f5c96b84ea00a>`("ov::pass::ModelPass");
		virtual bool :target:`run_on_function<doxid-classov_1_1pass_1_1_model_pass_1a58cf259fa3f2d8b565e6929832656aa9>`(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> m);
		virtual bool :target:`run_on_model<doxid-classov_1_1pass_1_1_model_pass_1afdce6ef577b36b5127115dd574b6615e>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);
	};

	// direct descendants

	class :ref:`CommonOptimizations<doxid-classngraph_1_1pass_1_1_common_optimizations>`;
	class :ref:`ConvertOpSet1ToLegacy<doxid-classngraph_1_1pass_1_1_convert_op_set1_to_legacy>`;
	class :ref:`ConvertOpSet2ToOpSet1<doxid-classngraph_1_1pass_1_1_convert_op_set2_to_op_set1>`;
	class :ref:`ConvertOpSet3ToOpSet2<doxid-classngraph_1_1pass_1_1_convert_op_set3_to_op_set2>`;
	class :ref:`ConvertPrecision<doxid-classngraph_1_1pass_1_1_convert_precision>`;
	class :ref:`FixRtInfo<doxid-classngraph_1_1pass_1_1_fix_rt_info>`;
	class :ref:`GenerateMappingFile<doxid-classngraph_1_1pass_1_1_generate_mapping_file>`;
	class :ref:`GroupedStridedSliceOptimizer<doxid-classngraph_1_1pass_1_1_grouped_strided_slice_optimizer>`;
	class :ref:`InitNodeInfo<doxid-classngraph_1_1pass_1_1_init_node_info>`;
	class :ref:`AlignQuantizationIntervals<doxid-classngraph_1_1pass_1_1low__precision_1_1_align_quantization_intervals>`;
	class :ref:`AlignQuantizationParameters<doxid-classngraph_1_1pass_1_1low__precision_1_1_align_quantization_parameters>`;
	class :ref:`LowPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision>`;
	class :ref:`MarkupAvgPoolPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_avg_pool_precision_preserved>`;
	class :ref:`MarkupCanBeQuantized<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_can_be_quantized>`;
	class :ref:`MarkupOptimizations<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_optimizations>`;
	class :ref:`MarkupPrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions>`;
	class :ref:`MarkupQuantizationGranularity<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_quantization_granularity>`;
	class :ref:`PropagatePrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_precisions>`;

	template <class AttributeType>
	class :ref:`PropagateSharedValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_shared_value>`;

	class :ref:`MimicSetBatchSize<doxid-classngraph_1_1pass_1_1_mimic_set_batch_size>`;
	class :ref:`MOCTransformations<doxid-classngraph_1_1pass_1_1_m_o_c_transformations>`;
	class :ref:`POTTransformations<doxid-classngraph_1_1pass_1_1_p_o_t_transformations>`;
	class :ref:`Pruning<doxid-classngraph_1_1pass_1_1_pruning>`;
	class :ref:`ReverseInputChannelsFusion<doxid-classngraph_1_1pass_1_1_reverse_input_channels_fusion>`;
	class :ref:`SetBatchSize<doxid-classngraph_1_1pass_1_1_set_batch_size>`;
	class :ref:`SharedShapeOf<doxid-classngraph_1_1pass_1_1_shared_shape_of>`;
	class :ref:`SharedSqueeze<doxid-classngraph_1_1pass_1_1_shared_squeeze>`;
	class :ref:`SharedStridedSliceEraser<doxid-classngraph_1_1pass_1_1_shared_strided_slice_eraser>`;
	class :ref:`ShrinkWeights<doxid-classngraph_1_1pass_1_1_shrink_weights>`;
	class :ref:`SmartReshape<doxid-classngraph_1_1pass_1_1_smart_reshape>`;
	class :ref:`StridedSliceOptimization<doxid-classngraph_1_1pass_1_1_strided_slice_optimization>`;
	class :ref:`UnrollIf<doxid-classngraph_1_1pass_1_1_unroll_if>`;
	class :ref:`UnrollTensorIterator<doxid-classngraph_1_1pass_1_1_unroll_tensor_iterator>`;
	class :ref:`UselessStridedSliceEraser<doxid-classngraph_1_1pass_1_1_useless_strided_slice_eraser>`;
	template :ref:`AssignRegisters<doxid-classngraph_1_1snippets_1_1pass_1_1_assign_registers>`;
	template :ref:`EnumerateNodes<doxid-classngraph_1_1snippets_1_1pass_1_1_enumerate_nodes>`;
	class :ref:`ChangePlaceholderTypes<doxid-classov_1_1pass_1_1_change_placeholder_types>`;
	class :ref:`ConstantFolding<doxid-classov_1_1pass_1_1_constant_folding>`;
	class :ref:`ConvertCompressedOnlyToLegacy<doxid-classov_1_1pass_1_1_convert_compressed_only_to_legacy>`;
	class :ref:`ConvertFP32ToFP16<doxid-classov_1_1pass_1_1_convert_f_p32_to_f_p16>`;
	class :ref:`FindBatch<doxid-classov_1_1pass_1_1_find_batch>`;
	class :ref:`GraphRewrite<doxid-classov_1_1pass_1_1_graph_rewrite>`;
	class :ref:`Hash<doxid-classov_1_1pass_1_1_hash>`;
	class :ref:`LowLatency2<doxid-classov_1_1pass_1_1_low_latency2>`;
	class :ref:`MakeStateful<doxid-classov_1_1pass_1_1_make_stateful>`;
	class :ref:`MarkPrecisionSensitiveDivides<doxid-classov_1_1pass_1_1_mark_precision_sensitive_divides>`;
	class :ref:`MarkPrecisionSensitiveSubgraphs<doxid-classov_1_1pass_1_1_mark_precision_sensitive_subgraphs>`;
	class :ref:`MOCLegacyTransformations<doxid-classov_1_1pass_1_1_m_o_c_legacy_transformations>`;
	class :ref:`ResolveNameCollisions<doxid-classov_1_1pass_1_1_resolve_name_collisions>`;
	class :ref:`Serialize<doxid-classov_1_1pass_1_1_serialize>`;
	class :ref:`StreamSerialize<doxid-classov_1_1pass_1_1_stream_serialize>`;
	class :ref:`Validate<doxid-classov_1_1pass_1_1_validate>`;
	class :ref:`VisualizeTree<doxid-classov_1_1pass_1_1_visualize_tree>`;

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


