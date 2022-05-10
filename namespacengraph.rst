.. index:: pair: namespace; ngraph
.. _doxid-namespacengraph:

namespace ngraph
================

.. toctree::
	:hidden:

	builder <namespacengraph_1_1builder.rst>
	coordinates <namespacengraph_1_1coordinates.rst>
	descriptor <namespacengraph_1_1descriptor.rst>
	element <namespacengraph_1_1element.rst>
	file_util <namespacengraph_1_1file_util.rst>
	op <namespacengraph_1_1op.rst>
	opset1 <namespacengraph_1_1opset1.rst>
	opset2 <namespacengraph_1_1opset2.rst>
	opset3 <namespacengraph_1_1opset3.rst>
	opset4 <namespacengraph_1_1opset4.rst>
	opset5 <namespacengraph_1_1opset5.rst>
	opset6 <namespacengraph_1_1opset6.rst>
	opset7 <namespacengraph_1_1opset7.rst>
	opset8 <namespacengraph_1_1opset8.rst>
	opset9 <namespacengraph_1_1opset9.rst>
	pass <namespacengraph_1_1pass.rst>
	pattern <namespacengraph_1_1pattern.rst>
	reduction <namespacengraph_1_1reduction.rst>
	runtime <namespacengraph_1_1runtime.rst>
	snippets <namespacengraph_1_1snippets.rst>

Overview
~~~~~~~~

transformation aligns elementwise constant inputs ranks with its output rank :ref:`More...<details-namespacengraph>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace ngraph {

	// namespaces

	namespace :ref:`ngraph::builder<doxid-namespacengraph_1_1builder>`;
		namespace :ref:`ngraph::builder::opset1<doxid-namespacengraph_1_1builder_1_1opset1>`;
	namespace :ref:`ngraph::coordinates<doxid-namespacengraph_1_1coordinates>`;
	namespace :ref:`ngraph::descriptor<doxid-namespacengraph_1_1descriptor>`;
		namespace :ref:`ngraph::descriptor::layout<doxid-namespacengraph_1_1descriptor_1_1layout>`;
	namespace :ref:`ngraph::element<doxid-namespacengraph_1_1element>`;
	namespace :ref:`ngraph::file_util<doxid-namespacengraph_1_1file__util>`;
	namespace :ref:`ngraph::op<doxid-namespacengraph_1_1op>`;
		namespace :ref:`ngraph::op::internal<doxid-namespacengraph_1_1op_1_1internal>`;
		namespace :ref:`ngraph::op::util<doxid-namespacengraph_1_1op_1_1util>`;
			namespace :ref:`ngraph::op::util::detail<doxid-namespacengraph_1_1op_1_1util_1_1detail>`;
			namespace :ref:`ngraph::op::util::error<doxid-namespacengraph_1_1op_1_1util_1_1error>`;
		namespace :ref:`ngraph::op::v0<doxid-namespacengraph_1_1op_1_1v0>`;
		namespace :ref:`ngraph::op::v1<doxid-namespacengraph_1_1op_1_1v1>`;
		namespace :ref:`ngraph::op::v3<doxid-namespacengraph_1_1op_1_1v3>`;
		namespace :ref:`ngraph::op::v4<doxid-namespacengraph_1_1op_1_1v4>`;
		namespace :ref:`ngraph::op::v5<doxid-namespacengraph_1_1op_1_1v5>`;
		namespace :ref:`ngraph::op::v6<doxid-namespacengraph_1_1op_1_1v6>`;
		namespace :ref:`ngraph::op::v7<doxid-namespacengraph_1_1op_1_1v7>`;
		namespace :ref:`ngraph::op::v8<doxid-namespacengraph_1_1op_1_1v8>`;
		namespace :ref:`ngraph::op::v9<doxid-namespacengraph_1_1op_1_1v9>`;
	namespace :ref:`ngraph::opset1<doxid-namespacengraph_1_1opset1>`;
	namespace :ref:`ngraph::opset2<doxid-namespacengraph_1_1opset2>`;
	namespace :ref:`ngraph::opset3<doxid-namespacengraph_1_1opset3>`;
	namespace :ref:`ngraph::opset4<doxid-namespacengraph_1_1opset4>`;
	namespace :ref:`ngraph::opset5<doxid-namespacengraph_1_1opset5>`;
	namespace :ref:`ngraph::opset6<doxid-namespacengraph_1_1opset6>`;
	namespace :ref:`ngraph::opset7<doxid-namespacengraph_1_1opset7>`;
	namespace :ref:`ngraph::opset8<doxid-namespacengraph_1_1opset8>`;
	namespace :ref:`ngraph::opset9<doxid-namespacengraph_1_1opset9>`;
	namespace :ref:`ngraph::pass<doxid-namespacengraph_1_1pass>`;
		namespace :ref:`ngraph::pass::itt<doxid-namespacengraph_1_1pass_1_1itt>`;
			namespace :ref:`ngraph::pass::itt::domains<doxid-namespacengraph_1_1pass_1_1itt_1_1domains>`;
		namespace :ref:`ngraph::pass::low_precision<doxid-namespacengraph_1_1pass_1_1low__precision>`;
			namespace :ref:`ngraph::pass::low_precision::itt<doxid-namespacengraph_1_1pass_1_1low__precision_1_1itt>`;
				namespace :ref:`ngraph::pass::low_precision::itt::domains<doxid-namespacengraph_1_1pass_1_1low__precision_1_1itt_1_1domains>`;
			namespace :ref:`ngraph::pass::low_precision::precision_set<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set>`;
	namespace :ref:`ngraph::pattern<doxid-namespacengraph_1_1pattern>`;
		namespace :ref:`ngraph::pattern::op<doxid-namespacengraph_1_1pattern_1_1op>`;
	namespace :ref:`ngraph::reduction<doxid-namespacengraph_1_1reduction>`;
	namespace :ref:`ngraph::runtime<doxid-namespacengraph_1_1runtime>`;
		namespace :ref:`ngraph::runtime::opt_kernel<doxid-namespacengraph_1_1runtime_1_1opt__kernel>`;
		namespace :ref:`ngraph::runtime::reference<doxid-namespacengraph_1_1runtime_1_1reference>`;
			namespace :ref:`ngraph::runtime::reference::adaptive_pool<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool>`;
			namespace :ref:`ngraph::runtime::reference::detail<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail>`;
			namespace :ref:`ngraph::runtime::reference::details<doxid-namespacengraph_1_1runtime_1_1reference_1_1details>`;
			namespace :ref:`ngraph::runtime::reference::fake_quantize_details<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details>`;
			namespace :ref:`ngraph::runtime::reference::fft_common<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common>`;
			namespace :ref:`ngraph::runtime::reference::internal<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal>`;
			namespace :ref:`ngraph::runtime::reference::kernel<doxid-namespacengraph_1_1runtime_1_1reference_1_1kernel>`;
			namespace :ref:`ngraph::runtime::reference::nms_common<doxid-namespacengraph_1_1runtime_1_1reference_1_1nms__common>`;
	namespace :ref:`ngraph::snippets<doxid-namespacengraph_1_1snippets>`;
		namespace :ref:`ngraph::snippets::isa<doxid-namespacengraph_1_1snippets_1_1isa>`;
		namespace :ref:`ngraph::snippets::op<doxid-namespacengraph_1_1snippets_1_1op>`;
		namespace :ref:`ngraph::snippets::pass<doxid-namespacengraph_1_1snippets_1_1pass>`;

	// global functions

	std::ostream& :target:`operator <<<doxid-namespacengraph_1a461cab9b38ecd8444670821211782f92>` (std::ostream& s, const :ref:`ELTWISE_TYPE<doxid-eltwise_8hpp_1aca2b664f1fd62f182b07693d53c56611>`& type);
	std::ostream& :target:`operator <<<doxid-namespacengraph_1aa0004d575b809992fa0908ef162ad099>` (std::ostream& out, const Mask& mask);
	:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>` :target:`getMask<doxid-namespacengraph_1a276c2b8681a4b504811e60de7e816180>`(const :ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`>& output);
	:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>` :target:`getMask<doxid-namespacengraph_1a05638bcf6f6f98537598756059482817>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output);
	void :target:`setMask<doxid-namespacengraph_1af24645d58bd172a829caace1b33fbb4e>`(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> output, const :ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>`& mask);
	void :target:`setMask<doxid-namespacengraph_1a897b6691e5342b213713320ea759923c>`(:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`> node, const :ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>`& mask);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`getFusedNames<doxid-group__ie__runtime__attr__api_1ga6e1dc6900c46d5648f89f51e62654768>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<std::string> :ref:`getFusedNamesVector<doxid-group__ie__runtime__attr__api_1ga927345dceac1f145e05e7b7af4600946>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`getenv_string<doxid-namespacengraph_1ab0ca6f364225db677d077fb164c77d7c>`(const char \* env_var);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` int32_t :ref:`getenv_int<doxid-namespacengraph_1a8c8b6ed07aca0ab0d5edc3a2b29f7780>`(const char \* env_var, int32_t default_value = -1);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`getenv_bool<doxid-namespacengraph_1a57fc6df09621f16de308f9089e00b50f>`(const char \* env_var, bool default_value = false);

	template <typename V>
	class :ref:`NGRAPH_DEPRECATED<doxid-namespacengraph_1aaa7db090d250b5035ce49040a924630a>`("This class is deprecated and will be removed soon.");

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::mutex& :target:`get_registry_mutex<doxid-namespacengraph_1a9bc5d446f195eaac7ed867635f193f21>`();

	std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :target:`clone_function<doxid-namespacengraph_1a5f75e639342db986514594f167340d69>`(
		const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`& func,
		:ref:`ngraph::NodeMap<doxid-classngraph_1adfcd122fbb01e901bed02647a928140b>`& node_map
		);

	std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :target:`clone_function<doxid-namespacengraph_1a3aff10976f09264136616f62a644064e>`(const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`& func);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>` :target:`find_common_args<doxid-namespacengraph_1ace368e04bd652b3fd104969f41c82b51>`(
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> target,
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> replacement
		);

	template <typename T>
	std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`subgraph_topological_sort<doxid-namespacengraph_1a40f80f6e78fc65f28feec5b38f063246>`(T nodes);

	template <typename T>
	void :target:`validate_nodes_and_infer_types<doxid-namespacengraph_1a6305d752de2842bcac4d85daa81f31ca>`(const T& nodes);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_post_dominated<doxid-namespacengraph_1aaabf140993e4214f00dbbeebdbd8752b>`(:ref:`Node<doxid-classov_1_1_node>` \* X, :ref:`Node<doxid-classov_1_1_node>` \* Y);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_equal_to_const_value<doxid-namespacengraph_1a5429ff9da2c64fd86c2931a5628416d0>`(
		const std::string& const_value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduce_constant
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>> :target:`clone_nodes<doxid-namespacengraph_1a536cbde8c55f1355e45e48c3eece4591>`(
		const std::vector<std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>>& nodes,
		:ref:`NodeMap<doxid-classngraph_1adfcd122fbb01e901bed02647a928140b>`& node_map
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::list<std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>> :target:`clone_nodes<doxid-namespacengraph_1aa3a01fc3796252d2348960ade4e34ddc>`(
		const std::vector<std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>>& nodes,
		:ref:`RawNodeOutputMap<doxid-classngraph_1ae90d6e6f0b09489992b9dcc346ed75e0>`& node_map
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::pair<std::shared_ptr<:ref:`op::v0::Result<doxid-classov_1_1op_1_1v0_1_1_result>`>, std::shared_ptr<:ref:`op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>> :target:`insert_result_parameter_split<doxid-namespacengraph_1a8177ba9fdf8f1a61aee3feee5e35b6fa>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& src_node,
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& dst_node
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :target:`insert_new_node_between<doxid-namespacengraph_1aa24eb475393d1704311dc2e1c1753b6d>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& src_node,
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& dst_node,
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& new_node
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_zero<doxid-namespacengraph_1af426c7e2b9c41ffbd1f5175dfd0dc08c>`(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_constant_from_string<doxid-namespacengraph_1afadc9ad07911d71b7d67dd9d30838127>`(
		std::string val,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_zero<doxid-namespacengraph_1aba7364943b9b8a633448249675fb8361>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduce_constant);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>` :target:`get_subgraph_outputs<doxid-namespacengraph_1abbbec9783e2fefa07f2547981a1926fe>`(
		const :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& nodes,
		const :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& exclusions,
		bool ignore_unused = false,
		bool ignore_output_duplicates = true
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>` :target:`extract_subgraph<doxid-namespacengraph_1a664b7a0173b515b5ea0973d1b777f33e>`(
		const :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& results,
		const :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& args
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_one<doxid-namespacengraph_1a5ce61fef894522df802345ad700280bb>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduce_constant);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_used<doxid-namespacengraph_1a65c01f461a18a4e1de085059ffb87510>`(:ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` size_t :target:`get_user_count<doxid-namespacengraph_1a30d34647f1fcf9f3f1af06032250ac15>`(:ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`possibly_overwritten<doxid-namespacengraph_1a1b08ff15ae9a027a1bae174145c0c366>`(:ref:`Node<doxid-classov_1_1_node>` \* node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_strided<doxid-namespacengraph_1a09fb0bc882e2bb78deabc8a112b0410c>`(const :ref:`Strides<doxid-classov_1_1_strides>`& strides);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`is_valid_rank<doxid-namespacengraph_1a0c91d087c875b695482d5bbe101c9069>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
		std::vector<size_t> valid_ranks
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :target:`plot_graph<doxid-namespacengraph_1a0399ef98cb1ee2ee836f26e75f3ef83f>`(
		std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> f,
		const std::string& filename,
		std::function<void(const :ref:`Node<doxid-classov_1_1_node>`&node, std::vector<std::string>&attributes)> = nullptr
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`get_inputs_from<doxid-namespacengraph_1a0c41d11aa89654a7e3aee4f7c318c0b5>`(:ref:`Node<doxid-classov_1_1_node>`& src, :ref:`Node<doxid-classov_1_1_node>`& dst);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`get_outputs_to<doxid-namespacengraph_1a19143937fba22a1648a43b87319c1ecb>`(:ref:`Node<doxid-classov_1_1_node>`& src, :ref:`Node<doxid-classov_1_1_node>`& dst);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`check_for_cycles<doxid-namespacengraph_1a1857a59f0f932bb2fbaf1cb57256ccd2>`(
		const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` \* func,
		:ref:`ngraph::NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& cycle_nodes,
		bool& is_bkwd_cycle
		);

	constexpr const char \* :target:`find_last<doxid-namespacengraph_1ad569d6b694c1f407e7a094f9665aa73c>`(ConstString s, size_t offset, char ch);
	constexpr const char \* :target:`find_last<doxid-namespacengraph_1a682ea617c979d6216b17e7dc30ca1499>`(ConstString s, char ch);
	constexpr const char \* :target:`get_file_name<doxid-namespacengraph_1abe57e16bd6987a55446fe92cf97a539f>`(ConstString s);
	constexpr const char \* :target:`trim_file_name<doxid-namespacengraph_1af37633bb9cc1314a430902aa87790d53>`(ConstString root, ConstString s);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :target:`default_logger_handler_func<doxid-namespacengraph_1a3304edc619eab3ff163e507cfeb40941>`(const std::string& s);

	template <typename T>
	NullLogger&& :target:`operator <<<doxid-namespacengraph_1a0b7c924ccab46c19919df155cbea19f7>` (NullLogger&& logger, T&&);

	template <typename T>
	NullLogger&& :target:`operator <<<doxid-namespacengraph_1af5d702b4c0aaf882a6bb2618fe59e89a>` (NullLogger&& logger, const T&);

	NullLogger&& :target:`operator <<<doxid-namespacengraph_1acae20ad2d4c8bcddc047c6e5ef114f3c>` (
		NullLogger&& logger,
		std::basic_ostream<char, std::char_traits<char>>&&)(std::basic_ostream< char, std::char_traits< char >> &
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& :target:`check_single_output_arg<doxid-namespacengraph_1a5c50aefd3323b4c66bf8c1af1d15b85d>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
		size_t i
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` const :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& :target:`check_single_output_args<doxid-namespacengraph_1a059fc59d1da3f5f5c86149b1fbc08094>`(const :ref:`NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& args);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`operator -<doxid-namespacengraph_1a3e6ac6e027e41f4de54f7d6b5fe9b86e>` (const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg0);

	:ref:`AxisSet<doxid-classov_1_1_axis_set>` :ref:`get_normalized_axes_from_tensor<doxid-namespacengraph_1a7d5bf7330cecf6144535004936d05338>`(
		const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` tensor,
		const ngraph::Rank& rank,
		const std::string& node_description
		);

	SlicePlan :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :target:`make_slice_plan<doxid-namespacengraph_1a6c7f03d57a5ef085b357d062fcda71c4>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		const std::vector<int64_t>& begins,
		const std::vector<int64_t>& ends,
		const std::vector<int64_t>& strides,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& lower_bounds_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& upper_bounds_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& new_axis_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& shrink_axis_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& ellipsis_mask
		);

	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset1<doxid-namespacengraph_1ab955e8d090d5cc730363c4b725885f4c>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset2<doxid-namespacengraph_1a4642af652fbf8dd37a1db54e3daa8bbc>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset3<doxid-namespacengraph_1ab00af9ca66ae5ecbe7a262b94b94ec18>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset4<doxid-namespacengraph_1a7ef460b05345e195fec58e9b1d588b00>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset5<doxid-namespacengraph_1a7a785c204db1de65e46b933844ab3328>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset6<doxid-namespacengraph_1ab993bb0809075a30b1fa3c8dce27e14c>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset7<doxid-namespacengraph_1a4b2073fedfd5ffc3c22c7122177e1ef1>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset8<doxid-namespacengraph_1ac352851e62fa13cfef3ee4104ff2b8bd>`();
	const :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` OpSet& :target:`get_opset9<doxid-namespacengraph_1afeee5772f80ea89bc46592d1bf5ed118>`();

	template <typename AXIS_VALUES>
	AXIS_VALUES :target:`project<doxid-namespacengraph_1ac07213b09680c489f2459384ab36aaad>`(
		const AXIS_VALUES& axis_values,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& axes
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`project<doxid-namespacengraph_1ab67e6bc2dcb6bd71905a679ef2802610>`(const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& shape, const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& axes);

	template <typename AXIS_VALUES>
	AXIS_VALUES :target:`reduce<doxid-namespacengraph_1aca4b658093e49e8c5a503fcbebc3d931>`(
		const AXIS_VALUES& axis_values,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& deleted_axes,
		bool keep_dims
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`reduce<doxid-namespacengraph_1a3f1f8db043a7e0aba7a3e63fc41270f7>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& deleted_axes,
		bool keep_dims
		);

	template <typename AXIS_VALUES, typename AXIS_VALUE>
	AXIS_VALUES :target:`inject_pairs<doxid-namespacengraph_1a95e90249c1cf0c2dedd46b7df7543de6>`(
		const AXIS_VALUES& axis_values,
		std::vector<std::pair<size_t, AXIS_VALUE>> new_axis_pos_value_pairs
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`inject_pairs<doxid-namespacengraph_1a283bc96d773c79a5b4adcffa7d02c861>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& shape,
		std::vector<std::pair<size_t, :ref:`Dimension<doxid-classov_1_1_dimension>`>> new_axis_pos_value_pairs
		);

	template <typename AXIS_VALUES, typename AXIS_VALUE>
	AXIS_VALUES :target:`inject<doxid-namespacengraph_1a59bd47df869736103c2517fbe9c9b59f>`(
		const AXIS_VALUES& axis_values,
		size_t new_axis_pos,
		AXIS_VALUE new_axis_val
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`specialize_function<doxid-namespacengraph_1aeee37f3d43b3c41acf2b93c00b4fb2bb>`(
		std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> f,
		const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& parameter_element_types,
		const std::vector<:ref:`PartialShape<doxid-classov_1_1_partial_shape>`>& parameter_shapes,
		const std::vector<void \*>& parameter_values
		);

	size_t :ref:`compiler_byte_size<doxid-namespacengraph_1a51b2993b1c1c627a5b75b5ebbec6a3a8>`(element::Type_t et);

	template <typename T>
	std::string :target:`join<doxid-namespacengraph_1ad2f06feeb9a2c616bbb1d51f67d21147>`(
		const T& v,
		const std::string& sep = ", "
		);

	template <typename T>
	std::string :target:`vector_to_string<doxid-namespacengraph_1a7539123fc4727343234fd272ffbe2d0c>`(const T& v);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` size_t :target:`hash_combine<doxid-namespacengraph_1ad387fe752075925a8cc8b6536db13313>`(const std::vector<size_t>& list);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :target:`dump<doxid-namespacengraph_1a3755fb88b92d9e38b57ca8f7adc6a5ce>`(std::ostream& out, const void \*, size_t);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :target:`to_lower<doxid-namespacengraph_1a5cfeda5c8aa50566c495a117f01935e2>`(const std::string& s);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :target:`to_upper<doxid-namespacengraph_1aacf480f860f279a672e23645c042bffd>`(const std::string& s);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :target:`trim<doxid-namespacengraph_1a30f70ad798b32c02034950a69cbc23fd>`(const std::string& s);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<std::string> :target:`split<doxid-namespacengraph_1a62dce670c05bf7d9732478ec29392fb9>`(
		const std::string& s,
		char delimiter,
		bool trim = false
		);

	template <typename T>
	std::string :target:`locale_string<doxid-namespacengraph_1aa56775ffc4df1045dae8dff083624efd>`(T x);

	class :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :target:`NGRAPH_DEPRECATED<doxid-namespacengraph_1a886bd112b1bac6c0da3e84d2b78bf235>`("It is obsolete structure and will be removed soon");

	template <typename T>
	T :ref:`parse_string<doxid-namespacengraph_1a930c271c2c799f63f77ea702b1de1bb8>`(const std::string& s);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` float :ref:`parse_string< float ><doxid-namespacengraph_1afe54dd078f632c3dfb72a5b09a13b98c>`(const std::string& s);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` double :target:`parse_string< double ><doxid-namespacengraph_1ae652fa5d5db5d892e8b23e7a71230bb3>`(const std::string& s);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` int8_t :ref:`parse_string< int8_t ><doxid-namespacengraph_1aff8832558c00de38f38caf44ed02b173>`(const std::string& s);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` uint8_t :target:`parse_string< uint8_t ><doxid-namespacengraph_1a41c9cf89db24add343b0a7da241dfe3d>`(const std::string& s);

	template <typename T>
	std::vector<T> :ref:`parse_string<doxid-namespacengraph_1a14335cbdd13252ae9d0c790b2bb5009d>`(const std::vector<std::string>& ss);

	template <typename T>
	T :target:`ceil_div<doxid-namespacengraph_1ac97cb2fe49a89140cc6db2a6a4c22dae>`(const T& x, const T& y);

	template <typename T>
	T :target:`subtract_or_zero<doxid-namespacengraph_1aa1027e6d6f486b0375ad60f4d6fe24c9>`(T x, T y);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void \* :target:`ngraph_malloc<doxid-namespacengraph_1a6a80a036e93024d300119f7311dbc7d4>`(size_t size);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :target:`ngraph_free<doxid-namespacengraph_1a76784c27b0044e5d73ece701fcf3f8c1>`(void \*);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` size_t :target:`round_up<doxid-namespacengraph_1a929c0c3bb2c32b87169975cdcdaf98e9>`(size_t size, size_t alignment);

	bool :target:`is_valid_permutation<doxid-namespacengraph_1a21bdedd263959838f8e71f70789eb903>`(
		:ref:`ngraph::AxisVector<doxid-classov_1_1_axis_vector>` permutation,
		ngraph::Rank rank = Rank::dynamic()
		);

	template <typename T>
	T :target:`apply_permutation<doxid-namespacengraph_1ae75a2a158c27b4150f21e640c4ca3db5>`(T input, :ref:`ngraph::AxisVector<doxid-classov_1_1_axis_vector>` order);

	template :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :target:`NGRAPH_DEPRECATED<doxid-namespacengraph_1ac2f19c948c93d3a65402c543c8512fee>`("This method is deprecated and will be removed soon");
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`apply_permutation<doxid-namespacengraph_1a808823b6bccb6e0807ef05b688e7475d>`(:ref:`PartialShape<doxid-classov_1_1_partial_shape>` input, :ref:`AxisVector<doxid-classov_1_1_axis_vector>` order);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`AxisVector<doxid-classov_1_1_axis_vector>` :target:`get_default_order<doxid-namespacengraph_1a339b787475b309e06d15ba2b0a60c6ca>`(size_t rank);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`AxisVector<doxid-classov_1_1_axis_vector>` :target:`get_default_order<doxid-namespacengraph_1aa03da592d5e9cb5a068890c57c344742>`(const Rank& rank);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`AxisVector<doxid-classov_1_1_axis_vector>` :target:`get_default_order<doxid-namespacengraph_1a6d3284d222b7d63961d136889689aea6>`(const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`AxisVector<doxid-classov_1_1_axis_vector>` :target:`get_default_order<doxid-namespacengraph_1afc7a948a5af617a5b0cfa6405a064c36>`(const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& shape);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :ref:`parse_version_string<doxid-namespacengraph_1a764c66edf2a1d1ef91bee7c9c07822fa>`(
		std::string version,
		size_t& major,
		size_t& minor,
		size_t& patch,
		std::string& extra
		);

	template <typename T>
	T :target:`double_to_int<doxid-namespacengraph_1a017ad44e37db97e2bb5889fed87ad8f4>`(
		double x,
		double  float_to_int_converterdouble
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`Strides<doxid-classov_1_1_strides>` :target:`conv_default_strides<doxid-namespacengraph_1a8b27f10ffbdfb551b922d5258be1e987>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& data_batch_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& filters_shape
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>` :target:`conv_default_padding<doxid-namespacengraph_1a57be43c71c3fc7aae51791ac6f1e3aaa>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& data_batch_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& filters_shape
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`infer_windowed_reduction_output_shape<doxid-namespacengraph_1a088f9706e43c470ce056ce19f3c0059f>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& data_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& data_dilation,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& data_padding_below,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& data_padding_above,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& window_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_dilation,
		bool is_window_all_in_padding_allowed,
		bool ceil_mode = false
		);

	void :target:`validate_conv_params_spatial_dimensions<doxid-namespacengraph_1a51143565e337b37392fbb1db9b85acc6>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const size_t num_spatial_dims,
		const op::PadType auto_pad,
		:ref:`Strides<doxid-classov_1_1_strides>`& strides,
		:ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	:ref:`PartialShape<doxid-classov_1_1_partial_shape>` :ref:`validate_and_infer_convolution_forward_output_shape<doxid-namespacengraph_1a99742d5a15fa5052df2086facd7b79db>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const Rank& result_ps_rank,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& data_batch_pshape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& filters_pshape,
		const op::PadType auto_pad,
		:ref:`Strides<doxid-classov_1_1_strides>`& strides,
		:ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`infer_batched_pooling_forward<doxid-namespacengraph_1af6a1998ad45e6210a0d3e64d92f8079a>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& data_batch_shape,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& data_padding_below,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& data_padding_above,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& window_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_strides,
		bool is_window_all_in_padding_allowed,
		bool ceil_mode = false,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_dilation = :ref:`Strides<doxid-classov_1_1_strides>`{}
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::tuple<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`PartialShape<doxid-classov_1_1_partial_shape>`, :ref:`PartialShape<doxid-classov_1_1_partial_shape>`> :target:`infer_batch_norm_forward<doxid-namespacengraph_1a2398046691e3e497eade0e9c2a9a0d2c>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` input_element_type,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` gamma_element_type,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` beta_element_type,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` mean_element_type,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` variance_element_type,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& gamma_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& beta_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& mean_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& variance_shape
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::tuple<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`PartialShape<doxid-classov_1_1_partial_shape>`, :ref:`PartialShape<doxid-classov_1_1_partial_shape>`> :target:`infer_batch_norm_forward<doxid-namespacengraph_1aba449bdb3835543d708813ce93a3cca4>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` input_element_type,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` gamma_element_type,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` beta_element_type,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& gamma_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& beta_shape
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`try_apply_auto_padding<doxid-namespacengraph_1a3999c74a99e0c50098d8e812179ef336>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& image_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filter_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& filter_strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& filter_dilations,
		const op::PadType pad_type,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& padding_above,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& padding_below
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`infer_slice_shape<doxid-namespacengraph_1acfc810fc8c6f222ddec1b99dcc74d7fd>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		const std::vector<int64_t>& begin,
		const std::vector<int64_t>& end,
		const std::vector<int64_t>& strides,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& begin_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& end_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& new_axis_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& shrink_axis_mask,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& ellipsis_mask
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::pair<bool, uint64_t> :ref:`maximum_value<doxid-namespacengraph_1a32557cb4210f12fcbc013f9f0295fca7>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :ref:`evaluate_nodes<doxid-namespacengraph_1a431031a5e1fda4d6062cc7812aa9c4c8>`(
		std::map<:ref:`RawNodeOutput<doxid-structov_1_1_raw_node_output>`, :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`>& value_map,
		std::map<:ref:`RawNodeOutput<doxid-structov_1_1_raw_node_output>`, :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`>& output_tensor_map,
		const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& outputs,
		const :ref:`EvaluationContext<doxid-classngraph_1ae31fbf851a75ba5a8e5f31b06d4079d5>`& evaluation_context = :ref:`EvaluationContext<doxid-classngraph_1ae31fbf851a75ba5a8e5f31b06d4079d5>`()
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` :ref:`evaluate_lower_bound<doxid-namespacengraph_1a093ad38099720345ea6b42b1a207492a>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` :ref:`evaluate_upper_bound<doxid-namespacengraph_1a6a75bbb857ec7d22fe4d413ca8b19629>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::pair<:ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`, :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`> :ref:`evaluate_both_bounds<doxid-namespacengraph_1a1b94f22a15a9d50a8e27515bcb662e68>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`default_upper_bound_evaluator<doxid-namespacengraph_1a49a0a7c2f5332e7afcec5543498a0615>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& output_values
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`default_lower_bound_evaluator<doxid-namespacengraph_1a7eaca4fafe0ddd12d18ef9fb3c77dabc>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& output_values
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`interval_bound_evaluator<doxid-namespacengraph_1a2e367361e2505784298f4c2c52d5c6dc>`(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& lower_output_values,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& upper_output_values
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`host_tensor_is_positive<doxid-namespacengraph_1a867dbdcfb4796a8123a8e854a82578a8>`(const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& bound);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`has_and_set_equal_bounds<doxid-namespacengraph_1a2296853cca716ee1634e67045d5bdf98>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& source);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`> :ref:`get_constant_max_of_type<doxid-namespacengraph_1a00eab419b9d22f8907fc848cacdb138c>`(element::Type_t t);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`> :ref:`get_constant_min_of_type<doxid-namespacengraph_1a360d402dc334a0713aed21821435317f>`(element::Type_t t);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`> :ref:`get_constant_lowest_of_type<doxid-namespacengraph_1a9919f8556a71109d556e7fda25dbf4a9>`(element::Type_t t);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :ref:`validate_host_tensor_vector<doxid-namespacengraph_1aa911fe63c6c20d886284060f00d251a6>`(
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& v,
		const size_t& size
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool :target:`could_propagate<doxid-namespacengraph_1ab2a28a92e755184caeb9a028953463e7>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output,
		std::vector<:ref:`Node<doxid-classov_1_1_node>` \*>& order
		);

	template <typename T>
	std::shared_ptr<:ref:`Variant<doxid-classngraph_1ac6b63b88aaff01196f0e557a6cd7c30f>`> :target:`make_variant<doxid-namespacengraph_1a647833adf1f8d4cde0c46579de526e8f>`(const T& p);

	template <size_t N>
	std::shared_ptr<:ref:`Variant<doxid-classngraph_1ac6b63b88aaff01196f0e557a6cd7c30f>`> :target:`make_variant<doxid-namespacengraph_1a5c3f3e8475bffa1bdee30812e080c43d>`(const char(&) s[N]);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :ref:`get_version<doxid-namespacengraph_1a4717d7fa0e3c26b98e7d6d409b3072c1>`(
		size_t& major,
		size_t& minor,
		size_t& patch,
		std::string& extra
		);

	std::size_t :target:`coordinate_index<doxid-namespacengraph_1a1b26478d6f5c3ab3140edfe06e9048cf>`(const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& c, const :ref:`Shape<doxid-classov_1_1_shape>`& s);

	} // namespace ngraph
.. _details-namespacengraph:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

transformation aligns elementwise constant inputs ranks with its output rank

The Intel nGraph C++ API.

ngraph namespace

Resolves transpose_b key from MatMul operation if corresponding input is constant or FakeQuantize by inserting Transpose.

Global Functions
----------------

.. _doxid-namespacengraph_1ab0ca6f364225db677d077fb164c77d7c:
.. index:: pair: function; getenv_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string getenv_string(const char \* env_var)

Get the names environment variable as a string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- env_var

		- The string name of the environment variable to get.



.. rubric:: Returns:

Returns string by value or an empty string if the environment variable is not set.

.. _doxid-namespacengraph_1a8c8b6ed07aca0ab0d5edc3a2b29f7780:
.. index:: pair: function; getenv_int

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` int32_t getenv_int(const char \* env_var, int32_t default_value = -1)

Get the names environment variable as an integer. If the value is not a valid integer then an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- env_var

		- The string name of the environment variable to get.

	*
		- default_value

		- The value to return if the environment variable is not set.



.. rubric:: Returns:

Returns value or default_value if the environment variable is not set.

.. _doxid-namespacengraph_1a57fc6df09621f16de308f9089e00b50f:
.. index:: pair: function; getenv_bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool getenv_bool(const char \* env_var, bool default_value = false)

Get the names environment variable as a boolean. If the value is not a valid boolean then an exception is thrown. Valid booleans are one of 1, 0, on, off, true, false All values are case insensitive. If the environment variable is not set the default_value is returned.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- env_var

		- The string name of the environment variable to get.

	*
		- default_value

		- The value to return if the environment variable is not set.



.. rubric:: Returns:

Returns the boolean value of the environment variable.

.. _doxid-namespacengraph_1aaa7db090d250b5035ce49040a924630a:
.. index:: pair: function; NGRAPH_DEPRECATED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename V>
	class NGRAPH_DEPRECATED("This class is deprecated and will be removed soon.")

Execute handlers on a subgraph to compute values.

.. _doxid-namespacengraph_1a40f80f6e78fc65f28feec5b38f063246:
.. index:: pair: function; subgraph_topological_sort

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> subgraph_topological_sort(T nodes)

Topological sort of just nodes.

.. _doxid-namespacengraph_1a0c41d11aa89654a7e3aee4f7c318c0b5:
.. index:: pair: function; get_inputs_from

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> get_inputs_from(:ref:`Node<doxid-classov_1_1_node>`& src, :ref:`Node<doxid-classov_1_1_node>`& dst)



.. rubric:: Returns:

A vector containing handles for each input of dst that is connected to an output of ``src``.

.. _doxid-namespacengraph_1a19143937fba22a1648a43b87319c1ecb:
.. index:: pair: function; get_outputs_to

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> get_outputs_to(:ref:`Node<doxid-classov_1_1_node>`& src, :ref:`Node<doxid-classov_1_1_node>`& dst)



.. rubric:: Returns:

A vector containing a handle for each output of src that is connected to an input of ``dst``.

.. _doxid-namespacengraph_1a1857a59f0f932bb2fbaf1cb57256ccd2:
.. index:: pair: function; check_for_cycles

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool check_for_cycles(
		const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` \* func,
		:ref:`ngraph::NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& cycle_nodes,
		bool& is_bkwd_cycle
		)

Checks the func for graph cycles starting from results going backwards, then from parameters going forward. It returns true if a cycle is found and the first cycle encountered.

.. _doxid-namespacengraph_1a7d5bf7330cecf6144535004936d05338:
.. index:: pair: function; get_normalized_axes_from_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`AxisSet<doxid-classov_1_1_axis_set>` get_normalized_axes_from_tensor(
		const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` tensor,
		const ngraph::Rank& rank,
		const std::string& node_description
		)

Extracts the tensor data and returns a set of normalized axes created out of it.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- A pointer to a HostTensor object containing the raw axes data

	*
		- rank

		- Rank of an operator's input data tensor (used to normalize the axes)

	*
		- node_description

		- An identifier of the operator's node (used to report errors)



.. rubric:: Returns:

Normalized (positive only) axes as an AxisSet object.

.. _doxid-namespacengraph_1aeee37f3d43b3c41acf2b93c00b4fb2bb:
.. index:: pair: function; specialize_function

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> specialize_function(
		std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> f,
		const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& parameter_element_types,
		const std::vector<:ref:`PartialShape<doxid-classov_1_1_partial_shape>`>& parameter_shapes,
		const std::vector<void \*>& parameter_values
		)

Creates a "specialized" clone of a function. The partial shapes and element types of the function's parameters may be narrowed to more specific shapes and element types, and constant values may optionally be substituted for any or all of the parameters.

Creates a "specialized" clone of an nGraph Function.

For example, suppose that a function f has three parameters with partial shapes:

.. ref-code-block:: cpp

	param0: ?
	param1: {1,?,3}
	param2: {?,?,4}

Shape specialization would allow us to create a clone of f where the shapes are (for example):

.. ref-code-block:: cpp

	param0: {1,2}
	param1: {1,5,3}
	param2: {3,?,4}

But not (for example):

.. ref-code-block:: cpp

	param1: {1,5,3,4}  // rank doesn't match {1,?,3}
	param1: {2,?,3}    // the "2" doesn't match the "1"
	param1: {?,?,3}    // the new shape is too relaxed: it doesn't require 1 for the first dim

Note that validation errors can potentially occur during cloning. For example:

.. ref-code-block:: cpp

	n = Parameter{shape=?}
	m = Parameter{shape=?}
	x = n + m
	f = Function(x,{n,m})

If we specialize n to the shape ``{1,2,3}`` and m to the shape ``{4,5,6}``, cloning will fail because when we reconstruct the new x node, it will see that the shapes are inconsistent for elementwise add.

Specialization of element types is also possible: ``element::dynamic`` can be specialized to a concrete element type or left dynamic; but a concrete element type can only be specialized to itself (e.g., specialization does not allow you to change ``element::i32`` to ``element::i64``).

Finally, it is possible to specialize parameter values. If the ith element of ``parameter_values`` is not ``nullptr``, and fully static element type and shape has been specified for the ith parameter, a ``Constant`` node will be created and substituted for the ith parameter, with its data drawn from ``parameter_values[i]``. Note that the Parameter node remains (in order to maintain the arity of the function), but will no longer have any users.

It is required that:

#. The length of parameter_element_types, parameter_shapes, and parameter_values is the same as the number of f's parameters.

#. Each shape in parameter_shapes is a refinement of the shape of the corresponding parameter of f. Roughly speaking, a shape s1 is said to "refine" s2 if s1 can be obtained from s2 by filling in s2's question marks. See :ref:`PartialShape::refines <doxid-classov_1_1_partial_shape_1a44f771b339b315adbd52cdc4d99dfa78>` for more details.

#. For all i, either the element type of fp_i is dynamic, or fp_i is the same as parameter_element_types[i]. (Here fp_i is the ith parameter of f.)

#. For all i where parameter_values[i] != nullptr and parameter_element_types[i] is static and parameter_shapes[i] is static, parameter_values[i] points to a buffer from which a Constant node with element type parameter_element_types[i] and shape parameter_shapes[i] can be created.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- f

		- The function to be cloned.

	*
		- parameter_element_types

		- The new parameter element types to substitute. Length must be equal to the number of parameters of f.

	*
		- parameter_shapes

		- The new parameter shapes to substitute. Length must be equal to the number of parameters of f.

	*
		- parameter_values

		- Parameter values to substitute. Length must be equal to the number of parameters of f, with nullptr indicating that no substitution is to be made for the corresponding parameter.

	*
		- CheckFailure

		- if parameter_element_types, parameter_shapes is not valid (see details).

	*
		- NodeValidationError

		- if node validation fails as the clone is being constructed.



.. rubric:: Returns:

A clone of f, with the parameter element types, shapes, and values specialized.

.. _doxid-namespacengraph_1a51b2993b1c1c627a5b75b5ebbec6a3a8:
.. index:: pair: function; compiler_byte_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t compiler_byte_size(element::Type_t et)

Return the number of bytes in the compile-time representation of the element type.

.. _doxid-namespacengraph_1a930c271c2c799f63f77ea702b1de1bb8:
.. index:: pair: function; parse_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	T parse_string(const std::string& s)

Parses a string containing a literal of the underlying type.

.. _doxid-namespacengraph_1afe54dd078f632c3dfb72a5b09a13b98c:
.. index:: pair: function; parse_string< float >

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` float parse_string< float >(const std::string& s)

template specializations for float and double to handle INFINITY, -INFINITY and NaN values.

.. _doxid-namespacengraph_1aff8832558c00de38f38caf44ed02b173:
.. index:: pair: function; parse_string< int8_t >

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` int8_t parse_string< int8_t >(const std::string& s)

template specializations for int8_t and uint8_t to handle the fact that default implementation ends up treating values as characters so that the number "0" turns into the parsed value 48, which is it's ASCII value

.. _doxid-namespacengraph_1a14335cbdd13252ae9d0c790b2bb5009d:
.. index:: pair: function; parse_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	std::vector<T> parse_string(const std::vector<std::string>& ss)

Parses a list of strings containing literals of the underlying type.

.. _doxid-namespacengraph_1a764c66edf2a1d1ef91bee7c9c07822fa:
.. index:: pair: function; parse_version_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void parse_version_string(
		std::string version,
		size_t& major,
		size_t& minor,
		size_t& patch,
		std::string& extra
		)

Function to query parsed version information of the version of ngraph which contains this function. Version information strictly follows Semantic Versioning `http://semver.org <http://semver.org>`__.

Throws a runtime_error if there is an error during parsing



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- version

		- The major part of the version

	*
		- major

		- Returns the major part of the version

	*
		- minor

		- Returns the minor part of the version

	*
		- patch

		- Returns the patch part of the version

	*
		- extra

		- Returns the extra part of the version. This includes everything following the patch version number.

.. _doxid-namespacengraph_1a99742d5a15fa5052df2086facd7b79db:
.. index:: pair: function; validate_and_infer_convolution_forward_output_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PartialShape<doxid-classov_1_1_partial_shape>` validate_and_infer_convolution_forward_output_shape(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const Rank& result_ps_rank,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& data_batch_pshape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& filters_pshape,
		const op::PadType auto_pad,
		:ref:`Strides<doxid-classov_1_1_strides>`& strides,
		:ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		)

Validates input shape ranks and infers convolution forward output shape.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- Node with convolution operation.

	*
		- data_batch_pshape

		- Partial shape of data batch input.

	*
		- filters_pshape

		- Partial shape of filters input.

	*
		- auto_pad

		- Type of padding.

	*
		- strides

		- Strides.

	*
		- dilations

		- Dilations.

	*
		- pads_begin

		- Pads begin.

	*
		- pads_end

		- Pads end.



.. rubric:: Returns:

Partial shape of the output.

.. _doxid-namespacengraph_1a3999c74a99e0c50098d8e812179ef336:
.. index:: pair: function; try_apply_auto_padding

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool try_apply_auto_padding(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& image_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filter_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& filter_strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& filter_dilations,
		const op::PadType pad_type,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& padding_above,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& padding_below
		)

Apply auto padding to padding_above and padding_below inputs if all needed informations are known.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- image_shape

		- The shape of input image.

	*
		- filter_shape

		- The shape of filter input.

	*
		- filter_strides

		- The strides of applied padding.

	*
		- filter_dilations

		- The dilations of applied padding.

	*
		- pad_type

		- The type of padding. Auto padding is applied only for SAME_UPPER and SAME_LOWER mode.

	*
		- padding_above

		- The beginning of padding shape.

	*
		- end

		- The beginning of padding shape.



.. rubric:: Returns:

true if auto padding was applied successfully (all needed informations such as spatial dims are known), false otherwise.

.. _doxid-namespacengraph_1a32557cb4210f12fcbc013f9f0295fca7:
.. index:: pair: function; maximum_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::pair<bool, uint64_t> maximum_value(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value)

Try to compute the maximum value of value.

Deprecated Use evaluate_upper_bound instead



.. rubric:: Returns:

(true, max_value) if can be determined, or (false, :ref:`numeric_limits\<uint64_t>::max() <doxid-namespacengraph_1_1runtime_1_1reference_1a92cfabd79e866544fb35d44884e7adfd>`) if not.

.. _doxid-namespacengraph_1a431031a5e1fda4d6062cc7812aa9c4c8:
.. index:: pair: function; evaluate_nodes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void evaluate_nodes(
		std::map<:ref:`RawNodeOutput<doxid-structov_1_1_raw_node_output>`, :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`>& value_map,
		std::map<:ref:`RawNodeOutput<doxid-structov_1_1_raw_node_output>`, :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`>& output_tensor_map,
		const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& outputs,
		const :ref:`EvaluationContext<doxid-classngraph_1ae31fbf851a75ba5a8e5f31b06d4079d5>`& evaluation_context = :ref:`EvaluationContext<doxid-classngraph_1ae31fbf851a75ba5a8e5f31b06d4079d5>`()
		)

Evaluates outputs, treating values in value_map as already computed. value_map is updated.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value_map

		- Key is RawNodeOutput in graph, value is the computed value. Updated by the function.

	*
		- output_tensor_map

		- Tensors to use for particular outputs

	*
		- outputs

		- Root set of values to try to compute

	*
		- evaluation_context

		- Storage of additional settings and attributes that can be used when evaluating the function. This additional information can be shared across nodes.

.. _doxid-namespacengraph_1a093ad38099720345ea6b42b1a207492a:
.. index:: pair: function; evaluate_lower_bound

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` evaluate_lower_bound(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output)

Evaluates lower value estimation of the output tensor. Traverses graph up to deduce estimation through it.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Node

		- output pointing to the tensor for estimation.



.. rubric:: Returns:

HostTensorPtr to estimated value if can be determined, or nullptr.

.. _doxid-namespacengraph_1a6a75bbb857ec7d22fe4d413ca8b19629:
.. index:: pair: function; evaluate_upper_bound

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` evaluate_upper_bound(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output)

Evaluates lower value estimation of the output tensor. Traverses graph up to deduce estimation through it.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output

		- Tensor to be estimated.



.. rubric:: Returns:

HostTensorPtr to estimated value if can be determined, or nullptr.

.. _doxid-namespacengraph_1a1b94f22a15a9d50a8e27515bcb662e68:
.. index:: pair: function; evaluate_both_bounds

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::pair<:ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`, :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`> evaluate_both_bounds(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& output)

Evaluates lower and upper value estimations of the output tensor. Traverses graph up to deduce estimation through it.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output

		- Node output pointing to the tensor for estimation.



.. rubric:: Returns:

pair with HostTensorPtrs for lower and upper value estimation. Each object in pair could be HostTensorPtr to estimated value if particular bound can be determined, or nullptr.

.. _doxid-namespacengraph_1a49a0a7c2f5332e7afcec5543498a0615:
.. index:: pair: function; default_upper_bound_evaluator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool default_upper_bound_evaluator(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& output_values
		)

Estimates upper bound for node output tensors using only upper bounds of the nodes inputs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- Operation to be performed

	*
		- output_values

		- Vector of HostTensorPtrs representing resulting upper value estimations



.. rubric:: Returns:

boolean status if value evaluation was successful.

.. _doxid-namespacengraph_1a7eaca4fafe0ddd12d18ef9fb3c77dabc:
.. index:: pair: function; default_lower_bound_evaluator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool default_lower_bound_evaluator(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& output_values
		)

Estimates lower bound for node output tensors using only lower bounds of the nodes inputs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- Operation to be performed

	*
		- output_values

		- Vector of HostTensorPtrs representing resulting lower value estimations



.. rubric:: Returns:

boolean status if value evaluation was successful.

.. _doxid-namespacengraph_1a2e367361e2505784298f4c2c52d5c6dc:
.. index:: pair: function; interval_bound_evaluator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool interval_bound_evaluator(
		const :ref:`Node<doxid-classov_1_1_node>` \* node,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& lower_output_values,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& upper_output_values
		)

Estimates both bounds for node output tensors using both bounds of inputs. Works for operations with two inputs (in_1 and in_2). Brute forces all the pairs of bounds for inputs and evaluates all of them: {in_1_lower, in_2 lower}, {in_1_lower, in_2 upper}, {in_1_upper, in_2_lower}, {in_1_upper, in_2_upper}. Lower and upper values are selected from all the outputs calculated using input pairs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- Operation to be performed

	*
		- output_values

		- Vector of HostTensorPtrs representing resulting lower value estimations



.. rubric:: Returns:

boolean status if value evaluation was successful.

.. _doxid-namespacengraph_1a867dbdcfb4796a8123a8e854a82578a8:
.. index:: pair: function; host_tensor_is_positive

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool host_tensor_is_positive(const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& bound)

Checks if all the elements of the bound HostTensor are positive.

.. _doxid-namespacengraph_1a2296853cca716ee1634e67045d5bdf98:
.. index:: pair: function; has_and_set_equal_bounds

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool has_and_set_equal_bounds(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& source)

Checks if lower and upper bounds of the corresponding tensor are set (not nullptr) and pointers are the same. It doesn't check if lower and upper values are the same relying only on pointers comparison.

.. _doxid-namespacengraph_1a00eab419b9d22f8907fc848cacdb138c:
.. index:: pair: function; get_constant_max_of_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`> get_constant_max_of_type(element::Type_t t)

Returns a Constant storing scalar value equal to :ref:`std::numeric_limits\<t>::max() <doxid-namespacengraph_1_1runtime_1_1reference_1a92cfabd79e866544fb35d44884e7adfd>`

.. _doxid-namespacengraph_1a360d402dc334a0713aed21821435317f:
.. index:: pair: function; get_constant_min_of_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`> get_constant_min_of_type(element::Type_t t)

Returns a Constant storing scalar value equal to :ref:`std::numeric_limits\<t>::min() <doxid-namespacengraph_1_1runtime_1_1reference_1abc42885cb896b121ab5ac214cbf60935>`

.. _doxid-namespacengraph_1a9919f8556a71109d556e7fda25dbf4a9:
.. index:: pair: function; get_constant_lowest_of_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`> get_constant_lowest_of_type(element::Type_t t)

Returns a Constant storing scalar value equal to std::numeric_limits<t>::lowest()

.. _doxid-namespacengraph_1aa911fe63c6c20d886284060f00d251a6:
.. index:: pair: function; validate_host_tensor_vector

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` bool validate_host_tensor_vector(
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& v,
		const size_t& size
		)

Checks if size of HostTensorVector is the same as passed size attribute. Then checks that all the HostTensorPtrs are not equal to nullptr.

.. _doxid-namespacengraph_1a4717d7fa0e3c26b98e7d6d409b3072c1:
.. index:: pair: function; get_version

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void get_version(
		size_t& major,
		size_t& minor,
		size_t& patch,
		std::string& extra
		)

Function to query parsed version information of the version of ngraph which contains this function. Version information strictly follows Semantic Versioning `http://semver.org <http://semver.org>`__.

Throws a runtime_error if there is an error during parsing



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- major

		- Returns the major part of the version

	*
		- minor

		- Returns the minor part of the version

	*
		- patch

		- Returns the patch part of the version

	*
		- extra

		- Returns the extra part of the version. This includes everything following the patch version number.

