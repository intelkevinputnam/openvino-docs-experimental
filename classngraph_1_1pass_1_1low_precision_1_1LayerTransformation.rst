.. index:: pair: class; ngraph::pass::low_precision::LayerTransformation
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation:

class ngraph::pass::low_precision::LayerTransformation
======================================================

.. toctree::
	:hidden:

	Params <classngraph_1_1pass_1_1low_precision_1_1LayerTransformation_1_1Params.rst>
	PrecisionDetails <classngraph_1_1pass_1_1low_precision_1_1LayerTransformation_1_1PrecisionDetails.rst>

Base class for low precision transformation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layer_transformation.hpp>
	
	class LayerTransformation: public :ref:`ov::pass::MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`
	{
	public:
		// classes
	
		class :ref:`Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>`;
		class :ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details>`;

		// construction
	
		:target:`LayerTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1add1465c89c31331eabeb26ebd809de3a>`(const :ref:`Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>`& params);

		// methods
	
		virtual bool :target:`transform<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a3627e6d74afd5f27b7d2dd1026b4ade4>`(
			:ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			:ref:`ngraph::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`& m
			) = 0;
	
		void :target:`setContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1afa651a113b1d038e0d4e86d4a3717002>`(:ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>` \* context);
		void :target:`setUpdatePrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a4225a64039ba8db1a7d55ccda6796b05>`(const bool updatePrecisions);
		void :target:`setDefaultPrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a52fbc288af478a2444b1debc4d0abc7e>`(const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions);
	
		virtual bool :target:`canBeTransformed<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a8ab1723ab94c2ce6bedb730e6ca4363a>`(
			const :ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer
			) const;
	
		bool :target:`canSubtractBeHandled<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a1c5845ce71e781aeeb7b4f681a0abd2f>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& op,
			const :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>`& dequantization
			) const;
	
		virtual bool :target:`isQuantized<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a33587b9f0d1b6fe28fd3deb50dae36fa>`(
			const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& layer,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions
			) const;
	
		virtual bool :target:`isPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a3dd681dfc8d7860085e316724282cf95>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer) const = 0;
	
		static bool :target:`canBeTransformedStatic<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a0b06240c74160bf5b03d50b9ea83d9f9>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& layer,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static :ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details>` :target:`getPrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a38575bbf3d48b7a3adaa1994272e0e1d>`(
			const size_t quantizationLevels,
			const std::vector<float>& outputLowValues,
			const std::vector<float>& outputHighValues
			);
	
		static :ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details>` :target:`getPrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a89f7c6b540f58296aa1efa3be3b7852f>`(const :ref:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details>`& quantizationDetails);
	
		static bool :target:`isAsymmetricQuantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a23155a77026a48988edbd0abec14b0d7>`(
			const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>` :target:`getDataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a818dbd529755b162c4a29f6c8ba75f39>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& layer,
			const :ref:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details>`& quantizationDetails,
			const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& requiredPrecisions
			);
	};

	// direct descendants

	class :ref:`AssignAndReadValueTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_assign_and_read_value_transformation>`;
	class :ref:`AvgPoolTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_avg_pool_transformation>`;
	class :ref:`ClampTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_clamp_transformation>`;
	class :ref:`ConcatTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_concat_transformation>`;
	class :ref:`ConvertTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_convert_transformation>`;
	class :ref:`EltwiseBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_eltwise_base_transformation>`;
	class :ref:`FakeQuantizeDecompositionTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_decomposition_transformation>`;
	class :ref:`FakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_transformation>`;
	class :ref:`FoldConvertTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fold_convert_transformation>`;
	class :ref:`FoldFakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fold_fake_quantize_transformation>`;
	class :ref:`FuseConvertTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fuse_convert_transformation>`;
	class :ref:`FuseMultiplyToFakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fuse_multiply_to_fake_quantize_transformation>`;
	class :ref:`FuseSubtractToFakeQuantizeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_fuse_subtract_to_fake_quantize_transformation>`;
	class :ref:`InterpolateTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_interpolate_transformation>`;
	class :ref:`MatMulTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_mat_mul_transformation>`;
	class :ref:`MaxPoolTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_max_pool_transformation>`;
	class :ref:`MoveFakeQuantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_move_fake_quantize>`;
	class :ref:`MultiplyToGroupConvolutionTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_multiply_to_group_convolution_transformation>`;
	class :ref:`MVNTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_m_v_n_transformation>`;
	class :ref:`NormalizeL2Transformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_normalize_l2_transformation>`;
	class :ref:`PadTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_pad_transformation>`;
	class :ref:`PReluTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_p_relu_transformation>`;
	class :ref:`ReduceBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reduce_base_transformation>`;
	class :ref:`ReluTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_relu_transformation>`;
	class :ref:`ReshapeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_reshape_transformation>`;
	class :ref:`ShuffleChannelsTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_shuffle_channels_transformation>`;
	class :ref:`SplitTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_split_transformation>`;
	class :ref:`SqueezeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_squeeze_transformation>`;
	class :ref:`StridedSliceTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_strided_slice_transformation>`;
	class :ref:`SubtractTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_subtract_transformation>`;
	class :ref:`TransparentBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_transparent_base_transformation>`;
	class :ref:`TransposeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_transpose_transformation>`;
	class :ref:`UnsqueezeTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_unsqueeze_transformation>`;
	class :ref:`WeightableLayerTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_weightable_layer_transformation>`;

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
		:ref:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_matcher_pass_1a525c64de11717629f6599042761eb844>`("ov::pass::MatcherPass");
		:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`& :ref:`operator =<doxid-classov_1_1pass_1_1_matcher_pass_1ae003cfdc27f2418f603f12b4f031ba3c>` (const :ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`&);
		bool :ref:`apply<doxid-classov_1_1pass_1_1_matcher_pass_1afe5e71b978b3dc8274ea93bb6e7dcc23>`(std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> node);
	
		template <typename T, class... Args>
		std::shared_ptr<T> :ref:`register_new_node<doxid-classov_1_1pass_1_1_matcher_pass_1a6e14fcb5d87373bab47d5778ea39ba55>`(Args&&... args);
	
		template <typename T>
		std::shared_ptr<T> :ref:`register_new_node<doxid-classov_1_1pass_1_1_matcher_pass_1acb4756e168d3130377473123783c16fa>`(const std::shared_ptr<T>& node);
	
		std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`register_new_node_<doxid-classov_1_1pass_1_1_matcher_pass_1ae343beb91a81a3a6b43670726c7e7abe>`(const std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>& node);
		const std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`get_new_nodes<doxid-classov_1_1pass_1_1_matcher_pass_1abf2e6b740f5e27a13589f19b47e934af>`();
		void :ref:`clear_new_nodes<doxid-classov_1_1pass_1_1_matcher_pass_1a9a3abba77cc94f47e1cdc4e064544d6a>`();
		std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`> :ref:`get_matcher<doxid-classov_1_1pass_1_1_matcher_pass_1a69329c064bb3cb7268ae397f374648e8>`();


