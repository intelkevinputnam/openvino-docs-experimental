.. index:: pair: namespace; ov::pass
.. _doxid-namespaceov_1_1pass:

namespace ov::pass
==================

.. toctree::
	:hidden:

	pattern <namespaceov_1_1pass_1_1pattern.rst>
	PassProperty <enumov_1_1pass_1_1PassProperty.rst>
	Attributes <classov_1_1pass_1_1Attributes.rst>
	BackwardGraphRewrite <classov_1_1pass_1_1BackwardGraphRewrite.rst>
	ChangePlaceholderTypes <classov_1_1pass_1_1ChangePlaceholderTypes.rst>
	DisableConstantFolding <classov_1_1pass_1_1DisableConstantFolding.rst>
	FindBatch <classov_1_1pass_1_1FindBatch.rst>
	Hash <classov_1_1pass_1_1Hash.rst>
	MOCLegacyTransformations <classov_1_1pass_1_1MOCLegacyTransformations.rst>
	RemoveMultiSubGraphOpDanglingParams <classov_1_1pass_1_1RemoveMultiSubGraphOpDanglingParams.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace pass {

	// namespaces

	namespace :ref:`ov::pass::pattern<doxid-namespaceov_1_1pass_1_1pattern>`;
		namespace :ref:`ov::pass::pattern::op<doxid-namespaceov_1_1pass_1_1pattern_1_1op>`;

	// typedefs

	typedef :ref:`ov::EnumMask<doxid-classov_1_1_enum_mask>`<:ref:`PassProperty<doxid-namespaceov_1_1pass_1afb326b1cdca8f8b1602590c947cf997e>`> :target:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`;
	typedef std::function<bool(const std::shared_ptr<const :::ref:`ov::Node<doxid-classov_1_1_node>`>)> :target:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`;
	typedef std::map<:ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`, :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`> :target:`param_callback_map<doxid-namespaceov_1_1pass_1a5649425e4a043c291d9cefa33ae34fbd>`;

	// enums

	enum :ref:`PassProperty<doxid-namespaceov_1_1pass_1afb326b1cdca8f8b1602590c947cf997e>`;

	// classes

	class :ref:`AddOldApiMapToParameters<doxid-classov_1_1pass_1_1_add_old_api_map_to_parameters>`;
	class :ref:`Attributes<doxid-classov_1_1pass_1_1_attributes>`;
	class :ref:`BackwardGraphRewrite<doxid-classov_1_1pass_1_1_backward_graph_rewrite>`;
	class :ref:`ChangePlaceholderTypes<doxid-classov_1_1pass_1_1_change_placeholder_types>`;
	class :ref:`CompressFloatConstants<doxid-classov_1_1pass_1_1_compress_float_constants>`;
	class :ref:`CompressFloatConstantsImpl<doxid-classov_1_1pass_1_1_compress_float_constants_impl>`;
	class :ref:`ConstantFolding<doxid-classov_1_1pass_1_1_constant_folding>`;
	class :ref:`ConvertCompressedOnlyToLegacy<doxid-classov_1_1pass_1_1_convert_compressed_only_to_legacy>`;
	class :ref:`ConvertFP32ToFP16<doxid-classov_1_1pass_1_1_convert_f_p32_to_f_p16>`;
	class :ref:`DisableConstantFolding<doxid-classov_1_1pass_1_1_disable_constant_folding>`;
	class :ref:`DisableDecompressionConvertConstantFolding<doxid-classov_1_1pass_1_1_disable_decompression_convert_constant_folding>`;
	class :ref:`DivisionByZeroFP16Resolver<doxid-classov_1_1pass_1_1_division_by_zero_f_p16_resolver>`;
	class :ref:`EnableDecompressionConvertConstantFolding<doxid-classov_1_1pass_1_1_enable_decompression_convert_constant_folding>`;
	class :ref:`FindBatch<doxid-classov_1_1pass_1_1_find_batch>`;
	class :ref:`GraphRewrite<doxid-classov_1_1pass_1_1_graph_rewrite>`;
	class :ref:`Hash<doxid-classov_1_1pass_1_1_hash>`;
	class :ref:`LowLatency2<doxid-classov_1_1pass_1_1_low_latency2>`;
	class :ref:`MOCLegacyTransformations<doxid-classov_1_1pass_1_1_m_o_c_legacy_transformations>`;
	class :ref:`MakeStateful<doxid-classov_1_1pass_1_1_make_stateful>`;
	class :ref:`Manager<doxid-classov_1_1pass_1_1_manager>`;
	class :ref:`MarkPrecisionSensitiveDivides<doxid-classov_1_1pass_1_1_mark_precision_sensitive_divides>`;
	class :ref:`MarkPrecisionSensitiveSubgraphs<doxid-classov_1_1pass_1_1_mark_precision_sensitive_subgraphs>`;
	class :ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`;
	class :ref:`ModelPass<doxid-classov_1_1pass_1_1_model_pass>`;
	class :ref:`PassBase<doxid-classov_1_1pass_1_1_pass_base>`;
	class :ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`;
	class :ref:`RemoveConcatZeroDimInput<doxid-classov_1_1pass_1_1_remove_concat_zero_dim_input>`;
	class :ref:`RemoveMultiSubGraphOpDanglingParams<doxid-classov_1_1pass_1_1_remove_multi_sub_graph_op_dangling_params>`;
	class :ref:`ResolveNameCollisions<doxid-classov_1_1pass_1_1_resolve_name_collisions>`;
	class :ref:`Serialize<doxid-classov_1_1pass_1_1_serialize>`;
	class :ref:`StreamSerialize<doxid-classov_1_1pass_1_1_stream_serialize>`;
	class :ref:`Validate<doxid-classov_1_1pass_1_1_validate>`;
	class :ref:`VisualizeTree<doxid-classov_1_1pass_1_1_visualize_tree>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void :ref:`disable_constant_folding<doxid-group__ov__pass__cpp__api_1ga39583fbe9bf1dc98c7d203bdaa7b4275>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void :target:`enable_constant_folding<doxid-namespaceov_1_1pass_1a7d3bebe252d7ebdaa95875b831075c97>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`constant_folding_is_disabled<doxid-namespaceov_1_1pass_1a9440404651306f3c88d52ae50ae63d08>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

	} // namespace pass
