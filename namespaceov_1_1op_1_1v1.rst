.. index:: pair: namespace; ov::op::v1
.. _doxid-namespaceov_1_1op_1_1v1:

namespace ov::op::v1
====================

.. toctree::
	:hidden:

	AvgPool <classov_1_1op_1_1v1_1_1AvgPool.rst>
	GroupConvolution <classov_1_1op_1_1v1_1_1GroupConvolution.rst>
	GroupConvolutionBackpropData <classov_1_1op_1_1v1_1_1GroupConvolutionBackpropData.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v1 {

	// classes

	class :ref:`Add<doxid-classov_1_1op_1_1v1_1_1_add>`;
	class :ref:`AvgPool<doxid-classov_1_1op_1_1v1_1_1_avg_pool>`;
	class :ref:`BatchToSpace<doxid-classov_1_1op_1_1v1_1_1_batch_to_space>`;
	class :ref:`BinaryConvolution<doxid-classov_1_1op_1_1v1_1_1_binary_convolution>`;
	class :ref:`Broadcast<doxid-classov_1_1op_1_1v1_1_1_broadcast>`;
	class :ref:`ConvertLike<doxid-classov_1_1op_1_1v1_1_1_convert_like>`;
	class :ref:`Convolution<doxid-classov_1_1op_1_1v1_1_1_convolution>`;
	class :ref:`ConvolutionBackpropData<doxid-classov_1_1op_1_1v1_1_1_convolution_backprop_data>`;
	class :ref:`DeformableConvolution<doxid-classov_1_1op_1_1v1_1_1_deformable_convolution>`;
	class :ref:`DeformablePSROIPooling<doxid-classov_1_1op_1_1v1_1_1_deformable_p_s_r_o_i_pooling>`;
	class :ref:`Divide<doxid-classov_1_1op_1_1v1_1_1_divide>`;
	class :ref:`Equal<doxid-classov_1_1op_1_1v1_1_1_equal>`;
	class :ref:`FloorMod<doxid-classov_1_1op_1_1v1_1_1_floor_mod>`;
	class :ref:`Gather<doxid-classov_1_1op_1_1v1_1_1_gather>`;
	class :ref:`GatherTree<doxid-classov_1_1op_1_1v1_1_1_gather_tree>`;
	class :ref:`Greater<doxid-classov_1_1op_1_1v1_1_1_greater>`;
	class :ref:`GreaterEqual<doxid-classov_1_1op_1_1v1_1_1_greater_equal>`;
	class :ref:`GroupConvolution<doxid-classov_1_1op_1_1v1_1_1_group_convolution>`;
	class :ref:`GroupConvolutionBackpropData<doxid-classov_1_1op_1_1v1_1_1_group_convolution_backprop_data>`;
	class :ref:`Less<doxid-classov_1_1op_1_1v1_1_1_less>`;
	class :ref:`LessEqual<doxid-classov_1_1op_1_1v1_1_1_less_equal>`;
	class :ref:`LogicalAnd<doxid-classov_1_1op_1_1v1_1_1_logical_and>`;
	class :ref:`LogicalNot<doxid-classov_1_1op_1_1v1_1_1_logical_not>`;
	class :ref:`LogicalOr<doxid-classov_1_1op_1_1v1_1_1_logical_or>`;
	class :ref:`LogicalXor<doxid-classov_1_1op_1_1v1_1_1_logical_xor>`;
	class :ref:`MaxPool<doxid-classov_1_1op_1_1v1_1_1_max_pool>`;
	class :ref:`Maximum<doxid-classov_1_1op_1_1v1_1_1_maximum>`;
	class :ref:`Minimum<doxid-classov_1_1op_1_1v1_1_1_minimum>`;
	class :ref:`Mod<doxid-classov_1_1op_1_1v1_1_1_mod>`;
	class :ref:`Multiply<doxid-classov_1_1op_1_1v1_1_1_multiply>`;
	class :ref:`NonMaxSuppression<doxid-classov_1_1op_1_1v1_1_1_non_max_suppression>`;
	class :ref:`NotEqual<doxid-classov_1_1op_1_1v1_1_1_not_equal>`;
	class :ref:`OneHot<doxid-classov_1_1op_1_1v1_1_1_one_hot>`;
	class :ref:`Pad<doxid-classov_1_1op_1_1v1_1_1_pad>`;
	class :ref:`Power<doxid-classov_1_1op_1_1v1_1_1_power>`;
	class :ref:`ReduceLogicalAnd<doxid-classov_1_1op_1_1v1_1_1_reduce_logical_and>`;
	class :ref:`ReduceLogicalOr<doxid-classov_1_1op_1_1v1_1_1_reduce_logical_or>`;
	class :ref:`ReduceMax<doxid-classov_1_1op_1_1v1_1_1_reduce_max>`;
	class :ref:`ReduceMean<doxid-classov_1_1op_1_1v1_1_1_reduce_mean>`;
	class :ref:`ReduceMin<doxid-classov_1_1op_1_1v1_1_1_reduce_min>`;
	class :ref:`ReduceProd<doxid-classov_1_1op_1_1v1_1_1_reduce_prod>`;
	class :ref:`ReduceSum<doxid-classov_1_1op_1_1v1_1_1_reduce_sum>`;
	class :ref:`Reshape<doxid-classov_1_1op_1_1v1_1_1_reshape>`;
	class :ref:`Reverse<doxid-classov_1_1op_1_1v1_1_1_reverse>`;
	class :ref:`Select<doxid-classov_1_1op_1_1v1_1_1_select>`;
	class :ref:`Softmax<doxid-classov_1_1op_1_1v1_1_1_softmax>`;
	class :ref:`SpaceToBatch<doxid-classov_1_1op_1_1v1_1_1_space_to_batch>`;
	class :ref:`Split<doxid-classov_1_1op_1_1v1_1_1_split>`;
	class :ref:`StridedSlice<doxid-classov_1_1op_1_1v1_1_1_strided_slice>`;
	class :ref:`Subtract<doxid-classov_1_1op_1_1v1_1_1_subtract>`;
	class :ref:`TopK<doxid-classov_1_1op_1_1v1_1_1_top_k>`;
	class :ref:`Transpose<doxid-classov_1_1op_1_1v1_1_1_transpose>`;
	class :ref:`VariadicSplit<doxid-classov_1_1op_1_1v1_1_1_variadic_split>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a4836ad671836b670df36c0c7319b0eff>`(
		const :ref:`ov::op::v1::BatchToSpace<doxid-classov_1_1op_1_1v1_1_1_batch_to_space>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1ad687bc0836889c0124b235520beedb53>`(
		const :ref:`ov::op::v1::Broadcast<doxid-classov_1_1op_1_1v1_1_1_broadcast>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class ConvType>
	int64_t :target:`calculate_num_spatial<doxid-namespaceov_1_1op_1_1v1_1a0ce70b41ed4a95b0de7eb28f716e30e2>`(
		const ConvType \* op,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& filters_shape,
		const int64_t& num_non_spatial_data_dims,
		const int64_t& num_non_spatial_filter_dims
		);

	template <class ConvType>
	void :target:`update_and_validate_attributes<doxid-namespaceov_1_1op_1_1v1_1a0f825332d734c423e558e03e742491a4>`(ConvType \* op);

	template <class T>
	bool :target:`dynamic_check<doxid-namespaceov_1_1op_1_1v1_1a5e9d721ebd86e9768a7dac1ef659f34a>`(const int64_t& num_spatial);

	bool :target:`dynamic_check< PartialShape ><doxid-namespaceov_1_1op_1_1v1_1aa1e143eba4dd6bbe6b56ceaecac9a4a7>`(const int64_t& num_spatial);

	template <class ConvType, class ShapeType>
	bool :target:`resolve_auto_pad_for_shape<doxid-namespaceov_1_1op_1_1v1_1a5a72537784af720d01fc782b082bf7ba>`(
		const ConvType \* op,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const std::vector<ShapeType>& input_shapes,
		const int64_t& num_non_spatial_data_dims,
		const int64_t& num_non_spatial_filter_dims
		);

	template <class ConvType, class ShapeType>
	void :target:`calculate_output_spatial_dims_for_convolution<doxid-namespaceov_1_1op_1_1v1_1af70737ecdc19d1e8a5f4ab1b6842ba35>`(
		const ConvType \* op,
		const ShapeType& input_shape,
		const ShapeType& filters_shape,
		ShapeType& output_shape,
		const int64_t& num_spatial,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const int64_t& num_non_spatial_data_dims,
		const int64_t& num_non_spatial_filter_dims
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1abdb1ac579fb58bcb8f9703299cae05b2>`(
		const :ref:`Convolution<doxid-classov_1_1op_1_1v1_1_1_convolution>` \* op,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1ad351dc535f821698753bebf8bebbad44>`(
		const :ref:`GroupConvolution<doxid-classov_1_1op_1_1v1_1_1_group_convolution>` \* op,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class ConvType>
	int64_t :target:`calculate_num_spatial<doxid-namespaceov_1_1op_1_1v1_1a9638cb0dca66f99286d150c71bb22830>`(
		const ConvType \* op,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& filters_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& output_shapes_shape,
		const int64_t& num_non_spatial_data_dims,
		const int64_t& num_non_spatial_filter_dims
		);

	template <class ConvType>
	void :target:`update_and_validate_attributes_back_prop<doxid-namespaceov_1_1op_1_1v1_1abb92085bdae283789bcfbbf3594c5114>`(ConvType \* op);

	template <class ConvType, class ShapeType>
	bool :target:`resolve_auto_pad_for_shape_back_prop<doxid-namespaceov_1_1op_1_1v1_1a0025c8b9995790206884918ef47736c8>`(
		const ConvType \* op,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const std::vector<ShapeType>& input_shapes,
		ShapeType& output_spatial_shape,
		const int64_t& num_non_spatial_data_dims,
		const int64_t& num_non_spatial_filter_dims
		);

	template <class ConvType, class ShapeType>
	void :target:`calculate_output_spatial_dims_for_convolution_back_prop_data<doxid-namespaceov_1_1op_1_1v1_1aec25c20dc29beacdb0b47365ef3a6963>`(
		const ConvType \* op,
		const ShapeType& input_shape,
		const ShapeType& filters_shape,
		const ShapeType& output_rank,
		ShapeType& output_shape,
		const int64_t& num_spatial,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& output_padding,
		const int64_t& num_non_spatial_data_dims,
		const int64_t& num_non_spatial_filter_dims
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a3dd0ee5cefb16da37333be285cf400c1>`(
		const :ref:`ConvolutionBackpropData<doxid-classov_1_1op_1_1v1_1_1_convolution_backprop_data>` \* op,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const T& output_shape_from_input,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1aa0356d3db7b267738de88c86fb34b4cb>`(
		const :ref:`GroupConvolutionBackpropData<doxid-classov_1_1op_1_1v1_1_1_group_convolution_backprop_data>` \* op,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const T& output_shape_from_input,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a9c0604f37714538a888b59de6ff0ef35>`(
		const :ref:`GatherTree<doxid-classov_1_1op_1_1v1_1_1_gather_tree>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	void :target:`resolve_axis<doxid-namespaceov_1_1op_1_1v1_1ae393f14f901ba09749a07c0e6ad2121a>`(:ref:`OneHot<doxid-classov_1_1op_1_1v1_1_1_one_hot>` \* op);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a9c9599d1566f27083d20238acdaf1a75>`(
		const :ref:`OneHot<doxid-classov_1_1op_1_1v1_1_1_one_hot>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1ac31906860e9c4b0a33a5abd86c1962e8>`(
		const :ref:`Pad<doxid-classov_1_1op_1_1v1_1_1_pad>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a914875262ea6f985111fce2bc1b89440>`(
		const :ref:`Select<doxid-classov_1_1op_1_1v1_1_1_select>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a751050f2d2af9f02d4211200dd42cf16>`(
		const :ref:`ov::op::v1::SpaceToBatch<doxid-classov_1_1op_1_1v1_1_1_space_to_batch>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <typename T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a9638dcae06177d6df097eaf9a8c50331>`(
		const :ref:`Split<doxid-classov_1_1op_1_1v1_1_1_split>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a5a1b830259344d9c04d3954e0f7ea77d>`(
		const :ref:`StridedSlice<doxid-classov_1_1op_1_1v1_1_1_strided_slice>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <typename T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1ab5a2706ecbd6bd36272679c44abaa6d1>`(
		const :ref:`TopK<doxid-classov_1_1op_1_1v1_1_1_top_k>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <typename T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v1_1a05c37d65228e2f045deb6bc221a61f26>`(
		const :ref:`VariadicSplit<doxid-classov_1_1op_1_1v1_1_1_variadic_split>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	} // namespace v1
