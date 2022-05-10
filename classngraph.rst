.. index:: pair: class; ngraph
.. _doxid-classngraph:

class ngraph
============

.. toctree::
	:hidden:

	LOG_TYPE <enumngraph_1_1LOG_TYPE.rst>
	NullLogger <structngraph_1_1NullLogger.rst>
	SlicePlan <structngraph_1_1SlicePlan.rst>
	AvgPoolPrecisionPreservedAttribute <classngraph_1_1AvgPoolPrecisionPreservedAttribute.rst>
	ConstString <classngraph_1_1ConstString.rst>
	CoordinateIterator <classngraph_1_1CoordinateIterator.rst>
	CoordinateTransformBasic <classngraph_1_1CoordinateTransformBasic.rst>
	FactoryRegistry <classngraph_1_1FactoryRegistry.rst>
	FusedNames <classngraph_1_1FusedNames.rst>
	HasTypeInfoMember <classngraph_1_1HasTypeInfoMember.rst>
	IntervalsAlignmentAttribute <classngraph_1_1IntervalsAlignmentAttribute.rst>
	IntervalsAlignmentSharedValue <classngraph_1_1IntervalsAlignmentSharedValue.rst>
	LogHelper <classngraph_1_1LogHelper.rst>
	Logger <classngraph_1_1Logger.rst>
	Mask <classngraph_1_1Mask.rst>
	OpSet <classngraph_1_1OpSet.rst>
	PrecisionPreservedAttribute <classngraph_1_1PrecisionPreservedAttribute.rst>
	PrecisionsAttribute <classngraph_1_1PrecisionsAttribute.rst>
	QuantizationAlignmentAttribute <classngraph_1_1QuantizationAlignmentAttribute.rst>
	QuantizationGranularityAttribute <classngraph_1_1QuantizationGranularityAttribute.rst>
	QuantizationModeAttribute <classngraph_1_1QuantizationModeAttribute.rst>
	VariantImpl <classngraph_1_1VariantImpl.rst>
	VariantWrapper <classngraph_1_1VariantWrapper.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <base_matcher_pass.hpp>
	
	class ngraph: private MatcherPass
	{
	public:
		// typedefs
	
		typedef :ref:`ov::AssertFailure<doxid-classov_1_1_assert_failure>` :target:`CheckFailure<doxid-classngraph_1abed4f9aea67e01a561fbb60c9595d168>`;
		typedef :ref:`ov::Exception<doxid-classov_1_1_exception>` :ref:`ngraph_error<doxid-classngraph_1a75e3dd6189921f9a652278b0e83a75e3>`;
		typedef :ref:`ov::Model<doxid-classov_1_1_model>` :target:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`;
		typedef runtime::HostTensor :target:`HostTensor<doxid-classngraph_1a5e81977ec811af60e0e015ffed3d7b75>`;
		typedef std::shared_ptr<:ref:`HostTensor<doxid-classngraph_1a5e81977ec811af60e0e015ffed3d7b75>`> :target:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`;
		typedef std::vector<:ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`> :target:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`;
		typedef std::vector<size_t> :target:`TensorLabel<doxid-classngraph_1af9061b59f5b1d59a958909824b2a2f7e>`;
		typedef std::vector<:ref:`TensorLabel<doxid-classngraph_1af9061b59f5b1d59a958909824b2a2f7e>`> :target:`TensorLabelVector<doxid-classngraph_1a4f8c22ba5d766448d0d0befda790ba89>`;
		typedef :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>` :target:`EvaluationContext<doxid-classngraph_1ae31fbf851a75ba5a8e5f31b06d4079d5>`;
		typedef std::vector<std::shared_ptr<:ref:`ngraph::op::v0::Result<doxid-classov_1_1op_1_1v0_1_1_result>`>> :target:`ResultVector<doxid-classngraph_1aedfbc99202fbf343071141f5e0e26eff>`;
		typedef std::unordered_map<:ref:`ngraph::Node<doxid-classov_1_1_node>` \*, std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>> :ref:`NodeMap<doxid-classngraph_1adfcd122fbb01e901bed02647a928140b>`;
		typedef :ref:`Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>` :target:`NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>`;
		typedef std::map<:ref:`RawNodeOutput<doxid-structov_1_1_raw_node_output>`, :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :target:`RawNodeOutputMap<doxid-classngraph_1ae90d6e6f0b09489992b9dcc346ed75e0>`;
		typedef std::vector<std::shared_ptr<op::Parameter>> :target:`ParameterVector<doxid-classngraph_1a8288ec615d4e98f673d38597891c6e49>`;
		typedef std::vector<std::shared_ptr<op::Result>> :target:`ResultVector<doxid-classngraph_1a4a5bac908579414ad47615d4a87c3a76>`;
		typedef std::vector<std::shared_ptr<op::Sink>> :target:`SinkVector<doxid-classngraph_1abbfdf43102ee28d39d06716ffeb36f66>`;
		typedef std::shared_ptr<Variable> :target:`VariablePtr<doxid-classngraph_1ae60447cf0566cb10da60eb87b489ba79>`;
		typedef std::vector<:ref:`VariablePtr<doxid-classngraph_1ae60447cf0566cb10da60eb87b489ba79>`> :target:`VariableVector<doxid-classngraph_1af343452d6f775c241bdb18f0ab916a68>`;
		typedef std::unordered_map<:ref:`VariablePtr<doxid-classngraph_1ae60447cf0566cb10da60eb87b489ba79>`, :ref:`VariableValuePtr<doxid-classngraph_1a5db76d0782e1a6e18dd9206e1e51d0da>`> :target:`VariableMap<doxid-classngraph_1a2cddd277377206e048774d7e89e61d16>`;
		typedef std::shared_ptr<VariableValue> :target:`VariableValuePtr<doxid-classngraph_1a5db76d0782e1a6e18dd9206e1e51d0da>`;
		typedef :ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` :target:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`;
		typedef :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :target:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`;
		typedef :ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :target:`VariantTypeInfo<doxid-classngraph_1a84fad368b695ad97fa630dc877de7cfd>`;
		typedef :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>` :target:`Variant<doxid-classngraph_1ac6b63b88aaff01196f0e557a6cd7c30f>`;
		typedef std::shared_ptr<runtime::HostTensor> :target:`HostTensorPtr<doxid-classngraph_1ae1969ffae3f0efe7e03f25a346a78f12>`;

		// enums
	
		enum :ref:`LOG_TYPE<doxid-classngraph_1a0cab963f56b737df2702865a13c17db7>`;

		// structs
	
		struct :ref:`NullLogger<doxid-structngraph_1_1_null_logger>`;
		struct :ref:`SlicePlan<doxid-structngraph_1_1_slice_plan>`;

		// classes
	
		class :ref:`AvgPoolPrecisionPreservedAttribute<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute>`;
		class :ref:`ConstString<doxid-classngraph_1_1_const_string>`;
		class :ref:`CoordinateIterator<doxid-classngraph_1_1_coordinate_iterator>`;
		class :ref:`CoordinateTransformBasic<doxid-classngraph_1_1_coordinate_transform_basic>`;
		template <typename BASE_TYPE>
		class :ref:`FactoryRegistry<doxid-classngraph_1_1_factory_registry>`;
		class :ref:`FusedNames<doxid-classngraph_1_1_fused_names>`;
		template <class T>
		class :ref:`HasTypeInfoMember<doxid-classngraph_1_1_has_type_info_member>`;
		class :ref:`IntervalsAlignmentAttribute<doxid-classngraph_1_1_intervals_alignment_attribute>`;
		class :ref:`IntervalsAlignmentSharedValue<doxid-classngraph_1_1_intervals_alignment_shared_value>`;
		class :ref:`LogHelper<doxid-classngraph_1_1_log_helper>`;
		class :ref:`Logger<doxid-classngraph_1_1_logger>`;
		class :ref:`Mask<doxid-classngraph_1_1_mask>`;
		class :ref:`OpSet<doxid-classngraph_1_1_op_set>`;
		class :ref:`PrecisionPreservedAttribute<doxid-classngraph_1_1_precision_preserved_attribute>`;
		class :ref:`PrecisionsAttribute<doxid-classngraph_1_1_precisions_attribute>`;
		class :ref:`QuantizationAlignmentAttribute<doxid-classngraph_1_1_quantization_alignment_attribute>`;
		class :ref:`QuantizationGranularityAttribute<doxid-classngraph_1_1_quantization_granularity_attribute>`;
		class :ref:`QuantizationModeAttribute<doxid-classngraph_1_1_quantization_mode_attribute>`;
		template <typename VT>
		class :ref:`VariantImpl<doxid-classngraph_1_1_variant_impl>`;
		template <typename VT>
		class :ref:`VariantWrapper<doxid-classngraph_1_1_variant_wrapper>`;
		template <>
		class :ref:`VariantWrapper<int64_t><doxid-classngraph_1_1_variant_wrapper_3_01int64__t_01_4>`;
		template <>
		class :ref:`VariantWrapper<std::string><doxid-classngraph_1_1_variant_wrapper_3_01std_1_1string_01_4>`;

		// fields
	
		:ref:`AttributeParameters<doxid-class_attribute_parameters>` :target:`params<doxid-classngraph_1a3a5c1d5039baba18043c36aebc89040a>`;
		const auto :target:`node_validation_failure_loc_string<doxid-classngraph_1a475a5d3afb259886ffda489705458262>` = ov::node_validation_failure_loc_string;
		const auto :target:`as_output_vector<doxid-classngraph_1a81c8a2f70d0718bfb0452b6750718f29>` = ov::as_output_vector;
		const auto :target:`as_node_vector<doxid-classngraph_1a1505814cb9ba87b6ea8f0c07596c0c6a>` = ov::as_node_vector;
		const auto :target:`as_result_vector<doxid-classngraph_1a2021519ed922d39525cd2d041b347fff>` = ov::as_result_vector;
		template :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`AxisVector<doxid-classov_1_1_axis_vector>` :target:`order<doxid-classngraph_1adcd6574d0dbf39a2cc31948812aecab4>`;
		template class :ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :target:`VariantImpl< int64_t ><doxid-classngraph_1a30520e4d655c33d6f0981de9188ec4f8>`;
		template class :ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :target:`VariantImpl< bool ><doxid-classngraph_1a2321b6436f182e93d8e6b42c987bf948>`;

		// methods
	
		:target:`BaseMatcherPass<doxid-classngraph_1a2e04f0aa0fdd22d6efd749c2d6135fa6>`(const :ref:`AttributeParameters<doxid-class_attribute_parameters>`& params = :ref:`AttributeParameters<doxid-class_attribute_parameters>`());
	};
.. _details-classngraph:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Typedefs
--------

.. _doxid-classngraph_1a75e3dd6189921f9a652278b0e83a75e3:
.. index:: pair: typedef; ngraph_error

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef :ref:`ov::Exception<doxid-classov_1_1_exception>` ngraph_error

Base error for ngraph runtime errors.

.. _doxid-classngraph_1adfcd122fbb01e901bed02647a928140b:
.. index:: pair: typedef; NodeMap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::unordered_map<:ref:`ngraph::Node<doxid-classov_1_1_node>` \*, std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>> NodeMap

Alias useful for cloning.


