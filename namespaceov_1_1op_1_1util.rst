.. index:: pair: namespace; ov::op::util
.. _doxid-namespaceov_1_1op_1_1util:

namespace ov::op::util
======================

.. toctree::
	:hidden:

	detail <namespaceov_1_1op_1_1util_1_1detail.rst>
	error <namespaceov_1_1op_1_1util_1_1error.rst>
	rfft_common_validation <namespaceov_1_1op_1_1util_1_1rfft_common_validation.rst>
	LSTMPeepholesFormat <enumov_1_1op_1_1util_1_1LSTMPeepholesFormat.rst>
	LSTMWeightsFormat <enumov_1_1op_1_1util_1_1LSTMWeightsFormat.rst>
	VariableInfo <structov_1_1op_1_1util_1_1VariableInfo.rst>
	ActivationFunction <classov_1_1op_1_1util_1_1ActivationFunction.rst>
	ArithmeticReduction <classov_1_1op_1_1util_1_1ArithmeticReduction.rst>
	ArithmeticReductionKeepDims <classov_1_1op_1_1util_1_1ArithmeticReductionKeepDims.rst>
	AssignBase <classov_1_1op_1_1util_1_1AssignBase.rst>
	BinaryElementwiseArithmetic <classov_1_1op_1_1util_1_1BinaryElementwiseArithmetic.rst>
	BinaryElementwiseComparison <classov_1_1op_1_1util_1_1BinaryElementwiseComparison.rst>
	BinaryElementwiseLogical <classov_1_1op_1_1util_1_1BinaryElementwiseLogical.rst>
	BroadcastBase <classov_1_1op_1_1util_1_1BroadcastBase.rst>
	ConvertColorI420Base <classov_1_1op_1_1util_1_1ConvertColorI420Base.rst>
	ConvertColorNV12Base <classov_1_1op_1_1util_1_1ConvertColorNV12Base.rst>
	DeformableConvolutionBase <classov_1_1op_1_1util_1_1DeformableConvolutionBase.rst>
	DetectionOutputBase <classov_1_1op_1_1util_1_1DetectionOutputBase.rst>
	EmbeddingBagOffsetsBase <classov_1_1op_1_1util_1_1EmbeddingBagOffsetsBase.rst>
	EmbeddingBagPackedBase <classov_1_1op_1_1util_1_1EmbeddingBagPackedBase.rst>
	FFTBase <classov_1_1op_1_1util_1_1FFTBase.rst>
	FrameworkNode <classov_1_1op_1_1util_1_1FrameworkNode.rst>
	FrameworkNodeAttrs <classov_1_1op_1_1util_1_1FrameworkNodeAttrs.rst>
	GatherBase <classov_1_1op_1_1util_1_1GatherBase.rst>
	GatherNDBase <classov_1_1op_1_1util_1_1GatherNDBase.rst>
	IndexReduction <classov_1_1op_1_1util_1_1IndexReduction.rst>
	LogicalReduction <classov_1_1op_1_1util_1_1LogicalReduction.rst>
	LogicalReductionKeepDims <classov_1_1op_1_1util_1_1LogicalReductionKeepDims.rst>
	MaxPoolBase <classov_1_1op_1_1util_1_1MaxPoolBase.rst>
	MultiSubGraphOp <classov_1_1op_1_1util_1_1MultiSubGraphOp.rst>
	NmsBase <classov_1_1op_1_1util_1_1NmsBase.rst>
	RNNCellBase <classov_1_1op_1_1util_1_1RNNCellBase.rst>
	ReadValueBase <classov_1_1op_1_1util_1_1ReadValueBase.rst>
	ReductionBase <classov_1_1op_1_1util_1_1ReductionBase.rst>
	ScatterBase <classov_1_1op_1_1util_1_1ScatterBase.rst>
	ScatterNDBase <classov_1_1op_1_1util_1_1ScatterNDBase.rst>
	SubGraphOp <classov_1_1op_1_1util_1_1SubGraphOp.rst>
	UnaryElementwiseArithmetic <classov_1_1op_1_1util_1_1UnaryElementwiseArithmetic.rst>
	Variable <classov_1_1op_1_1util_1_1Variable.rst>
	VariableContext <classov_1_1op_1_1util_1_1VariableContext.rst>
	VariableExtension <classov_1_1op_1_1util_1_1VariableExtension.rst>
	VariableValue <classov_1_1op_1_1util_1_1VariableValue.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace util {

	// namespaces

	namespace :ref:`ov::op::util::detail<doxid-namespaceov_1_1op_1_1util_1_1detail>`;
	namespace :ref:`ov::op::util::error<doxid-namespaceov_1_1op_1_1util_1_1error>`;
	namespace :ref:`ov::op::util::rfft_common_validation<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation>`;

	// typedefs

	typedef std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>(\*)(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>&, float, float) :target:`ActivationFunctionType<doxid-namespaceov_1_1op_1_1util_1a9f70582388f029216424805b5f53343a>`;
	typedef std::vector<:ref:`util::SubGraphOp::InputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a750d0d553f8c4d59c87775f8ba335568>`> :target:`InputDescriptionVector<doxid-namespaceov_1_1op_1_1util_1a79283e6f2274c1e15487a40fa77bbd5e>`;
	typedef std::vector<:ref:`util::SubGraphOp::OutputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a53043b195b0af5f636fc35d5c8a501bc>`> :target:`OutputDescriptionVector<doxid-namespaceov_1_1op_1_1util_1a41bc8e0a7030353e60a1a1349b1a7ae4>`;
	typedef std::vector<:ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`> :target:`VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`;
	typedef std::unordered_map<:ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`, :ref:`VariableValue::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_value_1ac02453613047e3fc37b568870c7fb643>`> :target:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`;

	// enums

	enum :ref:`LSTMPeepholesFormat<doxid-namespaceov_1_1op_1_1util_1a7acc3984a9429d328eb064613c0008c0>`;
	enum :ref:`LSTMWeightsFormat<doxid-namespaceov_1_1op_1_1util_1a60f43f9a60503870550101be5f6f2f48>`;

	// structs

	struct :ref:`VariableInfo<doxid-structov_1_1op_1_1util_1_1_variable_info>`;

	// classes

	class :ref:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function>`;
	class :ref:`ArithmeticReduction<doxid-classov_1_1op_1_1util_1_1_arithmetic_reduction>`;
	class :ref:`ArithmeticReductionKeepDims<doxid-classov_1_1op_1_1util_1_1_arithmetic_reduction_keep_dims>`;
	class :ref:`AssignBase<doxid-classov_1_1op_1_1util_1_1_assign_base>`;
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
	class :ref:`FrameworkNodeAttrs<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs>`;
	class :ref:`GatherBase<doxid-classov_1_1op_1_1util_1_1_gather_base>`;
	class :ref:`GatherNDBase<doxid-classov_1_1op_1_1util_1_1_gather_n_d_base>`;
	class :ref:`IndexReduction<doxid-classov_1_1op_1_1util_1_1_index_reduction>`;
	class :ref:`LogicalReduction<doxid-classov_1_1op_1_1util_1_1_logical_reduction>`;
	class :ref:`LogicalReductionKeepDims<doxid-classov_1_1op_1_1util_1_1_logical_reduction_keep_dims>`;
	class :ref:`MaxPoolBase<doxid-classov_1_1op_1_1util_1_1_max_pool_base>`;
	class :ref:`MultiSubGraphOp<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`;
	class :ref:`NmsBase<doxid-classov_1_1op_1_1util_1_1_nms_base>`;
	class :ref:`RNNCellBase<doxid-classov_1_1op_1_1util_1_1_r_n_n_cell_base>`;
	class :ref:`ReadValueBase<doxid-classov_1_1op_1_1util_1_1_read_value_base>`;
	class :ref:`ReductionBase<doxid-classov_1_1op_1_1util_1_1_reduction_base>`;
	class :ref:`ScatterBase<doxid-classov_1_1op_1_1util_1_1_scatter_base>`;
	class :ref:`ScatterNDBase<doxid-classov_1_1op_1_1util_1_1_scatter_n_d_base>`;
	class :ref:`SubGraphOp<doxid-classov_1_1op_1_1util_1_1_sub_graph_op>`;
	class :ref:`UnaryElementwiseArithmetic<doxid-classov_1_1op_1_1util_1_1_unary_elementwise_arithmetic>`;
	class :ref:`Variable<doxid-classov_1_1op_1_1util_1_1_variable>`;
	class :ref:`VariableContext<doxid-classov_1_1op_1_1util_1_1_variable_context>`;
	class :ref:`VariableExtension<doxid-classov_1_1op_1_1util_1_1_variable_extension>`;
	class :ref:`VariableValue<doxid-classov_1_1op_1_1util_1_1_variable_value>`;

	// global functions

	:ref:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function>` :ref:`get_activation_func_by_name<doxid-namespaceov_1_1op_1_1util_1abe9db8bb903e840de4664208710897dc>`(const std::string& func_name);

	std::tuple<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`PartialShape<doxid-classov_1_1_partial_shape>`> :target:`validate_and_infer_elementwise_args<doxid-namespaceov_1_1op_1_1util_1ad54a600bb2d0e57668d5546ce3ad9d05>`(
		:ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob = :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`()
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_unary_elementwise_arithmetic<doxid-namespaceov_1_1op_1_1util_1a2fdec8deea491b78e527d6f1df5a63ca>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_binary_elementwise_arithmetic<doxid-namespaceov_1_1op_1_1util_1aca9184de38916605290c7d392ad0a28e>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_binary_elementwise_comparison<doxid-namespaceov_1_1op_1_1util_1a52bba87fbd6f2db23e186db6971353d5>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_binary_elementwise_logical<doxid-namespaceov_1_1op_1_1util_1ae2228f11cf4eab7702e362eccf98d0f0>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`supports_auto_broadcast<doxid-namespaceov_1_1op_1_1util_1a7f2a3e163e26c22106b8c73eb2545a84>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_op<doxid-namespaceov_1_1op_1_1util_1a3331ffdb76f997e04fded8ac5c56f194>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_parameter<doxid-namespaceov_1_1op_1_1util_1a3661dace12ff612e64d1c6e9a1221213>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_output<doxid-namespaceov_1_1op_1_1util_1acbc7b08408d076757bfa4d8c70e1f7bd>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_sink<doxid-namespaceov_1_1op_1_1util_1a717f9222468d7e050368576c3eaa7f44>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_constant<doxid-namespaceov_1_1op_1_1util_1ab4c248ad8ea86edd3aa31919265fe261>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_commutative<doxid-namespaceov_1_1op_1_1util_1a03d39bb838bae0a426346ea00f1356bc>`(const :ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_unary_elementwise_arithmetic<doxid-namespaceov_1_1op_1_1util_1ad52664b015e593e85e9d6ad41c4691d4>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_binary_elementwise_arithmetic<doxid-namespaceov_1_1op_1_1util_1a8e1f1be2366ca746c582ceff5dac2768>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_binary_elementwise_comparison<doxid-namespaceov_1_1op_1_1util_1a1e49ddf895baf0b1735dbf51cacbc434>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_binary_elementwise_logical<doxid-namespaceov_1_1op_1_1util_1a55725114cf7d0a388a6ca66453b0d148>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`supports_auto_broadcast<doxid-namespaceov_1_1op_1_1util_1a8073bd978c3789e331d8c57e2bf23b32>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_op<doxid-namespaceov_1_1op_1_1util_1ae39759b8b1bdca8a3eb4d612d4a09f47>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_parameter<doxid-namespaceov_1_1op_1_1util_1ae0c1efe3f4adb75c7af1d534187e4b3f>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_output<doxid-namespaceov_1_1op_1_1util_1a30b18b3498eee28d9ea5f93e340f7579>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_sink<doxid-namespaceov_1_1op_1_1util_1a004a50974bd0be73f634304061f54776>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_constant<doxid-namespaceov_1_1op_1_1util_1ae65e0a33485419c4b1ada68696d18168>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :target:`is_commutative<doxid-namespaceov_1_1op_1_1util_1a67f2242ce672e746f4c88acfd1a772be>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`convert_lstm_node_format<doxid-namespaceov_1_1op_1_1util_1a519a34c9b749c3b44b35d57c33ad1e56>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		:ref:`LSTMWeightsFormat<doxid-namespaceov_1_1op_1_1util_1a60f43f9a60503870550101be5f6f2f48>` from_format,
		:ref:`LSTMWeightsFormat<doxid-namespaceov_1_1op_1_1util_1a60f43f9a60503870550101be5f6f2f48>` to_format = LSTMWeightsFormat::FICO,
		int64_t axis = 0
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :target:`convert_lstm_peepholes_format<doxid-namespaceov_1_1op_1_1util_1a4a979a53794937c87e6a16309454346c>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		:ref:`LSTMPeepholesFormat<doxid-namespaceov_1_1op_1_1util_1a7acc3984a9429d328eb064613c0008c0>` from_format,
		:ref:`LSTMPeepholesFormat<doxid-namespaceov_1_1op_1_1util_1a7acc3984a9429d328eb064613c0008c0>` to_format = LSTMPeepholesFormat::FIO,
		int64_t axis = 0
		);

	template <typename T>
	void :target:`validate_target_shape_none<doxid-namespaceov_1_1op_1_1util_1a536eda5f3260ea047adf2684a2ecffea>`(
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		const T& arg_shape,
		const :ref:`AxisVector<doxid-classov_1_1_axis_vector>`& axes_mapping_val,
		const T& target_shape
		);

	template <typename T>
	void :target:`validate_target_shape_numpy<doxid-namespaceov_1_1op_1_1util_1a5ee8a7ae1d92516296d0f8d3170990cf>`(
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		const T& arg_shape,
		const T& target_shape
		);

	template <typename T>
	void :target:`set_result_shape_pdpd<doxid-namespaceov_1_1op_1_1util_1adfaaaab6bdf07b2dee3147512a1f40f0>`(
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		const T& arg0_shape,
		const T& target_shape,
		T& result_shape,
		const :ref:`ov::op::BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`set_result_shape_bidirectional<doxid-namespaceov_1_1op_1_1util_1ad241c06df4699ae3a4922813fc5c06ee>`(
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		const T& arg_shape,
		T& target_shape,
		T& result_shape
		);

	template <class T>
	void :target:`broadcase_base_shape_infer<doxid-namespaceov_1_1op_1_1util_1a29f03ec24b56efa33449df184ebafb2a>`(
		const :ref:`ov::op::util::BroadcastBase<doxid-classov_1_1op_1_1util_1_1_broadcast_base>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <
		typename T,
		typename V = typename std::iterator_traits<typename T::iterator>::value_type::value_type
		>
	void :target:`compute_num_classes<doxid-namespaceov_1_1op_1_1util_1ac3c048ad66982ce4dc5c80888e25ba5f>`(
		const :ref:`DetectionOutputBase<doxid-classov_1_1op_1_1util_1_1_detection_output_base>` \* op,
		const :ref:`DetectionOutputBase::AttributesBase<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base>`& attrs,
		const std::vector<T>& input_shapes,
		V& num_classes,
		V& num_prior_boxes
		);

	template <class T>
	void :target:`shape_infer_base<doxid-namespaceov_1_1op_1_1util_1a26de5f19fd64339141488ee8298d6007>`(
		const :ref:`DetectionOutputBase<doxid-classov_1_1op_1_1util_1_1_detection_output_base>` \* op,
		const :ref:`DetectionOutputBase::AttributesBase<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base>`& attrs,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		int64_t attribute_num_classes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1util_1ab0569238be0b66a44af0f5e2b6542001>`(
		const :ref:`ov::op::util::EmbeddingBagOffsetsBase<doxid-classov_1_1op_1_1util_1_1_embedding_bag_offsets_base>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`check_1D_or_scalar_shape<doxid-namespaceov_1_1op_1_1util_1a333f4136c1845b36906e1105ea4c0cdf>`(
		const :ref:`ov::op::v9::Eye<doxid-classov_1_1op_1_1v9_1_1_eye>` \* op,
		const T& input_shape,
		const std::string name
		);

	template <class T>
	void :target:`check_batch_shape_shape<doxid-namespaceov_1_1op_1_1util_1acce3a4e3e170d7d63012de586d09dbf0>`(
		const :ref:`ov::op::v9::Eye<doxid-classov_1_1op_1_1v9_1_1_eye>` \* op,
		const T& input_shape
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1util_1a2d457678a3eaa4cf0ebd3b7e3ef31cd3>`(
		const :ref:`ov::op::util::FFTBase<doxid-classov_1_1op_1_1util_1_1_f_f_t_base>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1util_1aed9753a63c834b62292c4ea936f6ac6a>`(
		const :ref:`GatherBase<doxid-classov_1_1op_1_1util_1_1_gather_base>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`irdft_shape_infer<doxid-namespaceov_1_1op_1_1util_1a46819e2f5b3952922e76811a1e3079a2>`(
		const :ref:`ov::op::v9::IRDFT<doxid-classov_1_1op_1_1v9_1_1_i_r_d_f_t>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <typename B>
	B :target:`get_ouput_dimension_bound<doxid-namespaceov_1_1op_1_1util_1a82d4b3ed793098b41d1745594d60afd1>`(B b);

	template <class DimType>
	DimType :target:`get_rdft_output_dimension<doxid-namespaceov_1_1op_1_1util_1a1e82b672aa0df8beaef99a3de338ca50>`(DimType d);

	template <class T>
	void :target:`rdft_shape_infer<doxid-namespaceov_1_1op_1_1util_1afcc06942cc20dca4638289d00b9c24a6>`(
		const :ref:`ov::op::v9::RDFT<doxid-classov_1_1op_1_1v9_1_1_r_d_f_t>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	} // namespace util
.. _details-namespaceov_1_1op_1_1util:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespaceov_1_1op_1_1util_1abe9db8bb903e840de4664208710897dc:
.. index:: pair: function; get_activation_func_by_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function>` get_activation_func_by_name(const std::string& func_name)

Gets the activation function by name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- func_name

		- The function name

	*
		- UnknownActivationFunction

		- When provided func_name is unknown.



.. rubric:: Returns:

The activation function object.

.. _doxid-namespaceov_1_1op_1_1util_1a519a34c9b749c3b44b35d57c33ad1e56:
.. index:: pair: function; convert_lstm_node_format

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` convert_lstm_node_format(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		:ref:`LSTMWeightsFormat<doxid-namespaceov_1_1op_1_1util_1a60f43f9a60503870550101be5f6f2f48>` from_format,
		:ref:`LSTMWeightsFormat<doxid-namespaceov_1_1op_1_1util_1a60f43f9a60503870550101be5f6f2f48>` to_format = LSTMWeightsFormat::FICO,
		int64_t axis = 0
		)

Change data format of provided node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The input node to be permuted.

	*
		- from_format

		- Original node weights format.

	*
		- to_format

		- Weights format to convert to.



.. rubric:: Returns:

:ref:`Node <doxid-classov_1_1_node>` representing reshaped tensor according to ``to_format`` weights format.

