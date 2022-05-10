.. index:: pair: class; ngraph::pass::low_precision::AddTransformation
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation:

class ngraph::pass::low_precision::AddTransformation
====================================================



Overview
~~~~~~~~

:ref:`AddTransformation <doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation>` propagates dequantization subtraction from one input branch to another and propagates dequantization multiplication from the same branch through Add operation. :ref:`More...<details-classngraph_1_1pass_1_1low__precision_1_1_add_transformation>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <add.hpp>
	
	class AddTransformation: public :ref:`ngraph::pass::low_precision::EltwiseBaseTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_eltwise_base_transformation>`
	{
	public:
		// construction
	
		:target:`AddTransformation<doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation_1a813ec2b381ddd3fb205e615c66add9a8>`(const :ref:`Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>`& params = :ref:`Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>`());

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation_1a6cd6ce0d7760c5883c1aff44b260282e>`("AddTransformation", "0");
	
		virtual bool :target:`transform<doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation_1aa280b25d520c4fe421081884eb3e86c4>`(
			:ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			:ref:`ngraph::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`& m
			);
	
		virtual bool :target:`canBeTransformed<doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation_1ae5d18fb8d559b23284bc5b0e96dfc951>`(
			const :ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer
			) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`;

		// classes
	
		class :ref:`Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>`;
		class :ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details>`;

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
	
		virtual bool :ref:`transform<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a3627e6d74afd5f27b7d2dd1026b4ade4>`(
			:ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			:ref:`ngraph::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`& m
			) = 0;
	
		void :ref:`setContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1afa651a113b1d038e0d4e86d4a3717002>`(:ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>` \* context);
		void :ref:`setUpdatePrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a4225a64039ba8db1a7d55ccda6796b05>`(const bool updatePrecisions);
		void :ref:`setDefaultPrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a52fbc288af478a2444b1debc4d0abc7e>`(const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions);
	
		virtual bool :ref:`canBeTransformed<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a8ab1723ab94c2ce6bedb730e6ca4363a>`(
			const :ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer
			) const;
	
		bool :ref:`canSubtractBeHandled<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a1c5845ce71e781aeeb7b4f681a0abd2f>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& op,
			const :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>`& dequantization
			) const;
	
		virtual bool :ref:`isQuantized<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a33587b9f0d1b6fe28fd3deb50dae36fa>`(
			const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& layer,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions
			) const;
	
		virtual bool :ref:`isPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a3dd681dfc8d7860085e316724282cf95>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer) const = 0;
	
		static bool :ref:`canBeTransformedStatic<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a0b06240c74160bf5b03d50b9ea83d9f9>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& layer,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static :ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details>` :ref:`getPrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a38575bbf3d48b7a3adaa1994272e0e1d>`(
			const size_t quantizationLevels,
			const std::vector<float>& outputLowValues,
			const std::vector<float>& outputHighValues
			);
	
		static :ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details>` :ref:`getPrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a89f7c6b540f58296aa1efa3be3b7852f>`(const :ref:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details>`& quantizationDetails);
	
		static bool :ref:`isAsymmetricQuantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a23155a77026a48988edbd0abec14b0d7>`(
			const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>` :ref:`getDataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1a818dbd529755b162c4a29f6c8ba75f39>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& layer,
			const :ref:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details>`& quantizationDetails,
			const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& requiredPrecisions
			);
	
		virtual bool :ref:`canBeTransformed<doxid-classngraph_1_1pass_1_1low__precision_1_1_eltwise_base_transformation_1ad9812d3c841216d844127005a273e80e>`(
			const :ref:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>`& context,
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer
			) const;
	
		virtual bool :ref:`isPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_eltwise_base_transformation_1a6c624e13d5530649ff778aab2dbbb109>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer) const;
		static bool :ref:`isBroadcasted<doxid-classngraph_1_1pass_1_1low__precision_1_1_eltwise_base_transformation_1afbd48d74d3f6fa95a408af1c7f500402>`(const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& shape);

.. _details-classngraph_1_1pass_1_1low__precision_1_1_add_transformation:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`AddTransformation <doxid-classngraph_1_1pass_1_1low__precision_1_1_add_transformation>` propagates dequantization subtraction from one input branch to another and propagates dequantization multiplication from the same branch through Add operation.

For more details about the transformation, refer to :ref:`AddTransformation <doxid-openvino_docs__o_v__u_g_lpt__add_transformation>` page in the Inference Engine Developer Guide.


