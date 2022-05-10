.. _global:
.. index:: pair: namespace; global

Global Namespace
================

.. toctree::
	:hidden:

	InferenceEngine <namespaceInferenceEngine.rst>
	cv <namespacecv.rst>
	std <namespacestd.rst>
	AttributeSource <enumAttributeSource.rst>
	CONVERSION_RESULT <enumCONVERSION_RESULT.rst>
	ELTWISE_TYPE <enumELTWISE_TYPE.rst>
	AttributeParameters <classAttributeParameters.rst>
	BlobFactory <classBlobFactory.rst>
	ConvertReduceBase <classConvertReduceBase.rst>
	MemorySolver <classMemorySolver.rst>
	SharedAttribute <classSharedAttribute.rst>
	logstreambuf <classlogstreambuf.rst>
	ngraph <classngraph.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`ExecGraphInfoSerialization<doxid-namespace_exec_graph_info_serialization>`;
	namespace :ref:`FileUtils<doxid-namespace_file_utils>`;
	namespace :ref:`InferenceEngine<doxid-namespace_inference_engine>`;
		namespace :ref:`InferenceEngine::CLDNNConfigParams<doxid-namespace_inference_engine_1_1_c_l_d_n_n_config_params>`;
		namespace :ref:`InferenceEngine::G<doxid-namespace_inference_engine_1_1_g>`;
		namespace :ref:`InferenceEngine::GNAConfigParams<doxid-namespace_inference_engine_1_1_g_n_a_config_params>`;
		namespace :ref:`InferenceEngine::GPUConfigParams<doxid-namespace_inference_engine_1_1_g_p_u_config_params>`;
		namespace :ref:`InferenceEngine::GPUContextParams<doxid-namespace_inference_engine_1_1_g_p_u_context_params>`;
		namespace :ref:`InferenceEngine::HeteroConfigParams<doxid-namespace_inference_engine_1_1_hetero_config_params>`;
		namespace :ref:`InferenceEngine::Metrics<doxid-namespace_inference_engine_1_1_metrics>`;
		namespace :ref:`InferenceEngine::MultiDeviceConfigParams<doxid-namespace_inference_engine_1_1_multi_device_config_params>`;
		namespace :ref:`InferenceEngine::NetPass<doxid-namespace_inference_engine_1_1_net_pass>`;
		namespace :ref:`InferenceEngine::PluginConfigInternalParams<doxid-namespace_inference_engine_1_1_plugin_config_internal_params>`;
		namespace :ref:`InferenceEngine::PluginConfigParams<doxid-namespace_inference_engine_1_1_plugin_config_params>`;
		namespace :ref:`InferenceEngine::PrecisionUtils<doxid-namespace_inference_engine_1_1_precision_utils>`;
			namespace :ref:`InferenceEngine::PrecisionUtils::details<doxid-namespace_inference_engine_1_1_precision_utils_1_1details>`;
		namespace :ref:`InferenceEngine::gapi<doxid-namespace_inference_engine_1_1gapi>`;
			namespace :ref:`InferenceEngine::gapi::kernels<doxid-namespace_inference_engine_1_1gapi_1_1kernels>`;
				namespace :ref:`InferenceEngine::gapi::kernels::areaDownscale32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_downscale32f>`;
				namespace :ref:`InferenceEngine::gapi::kernels::areaDownscale8u<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_downscale8u>`;
				namespace :ref:`InferenceEngine::gapi::kernels::areaUpscale<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_upscale>`;
				namespace :ref:`InferenceEngine::gapi::kernels::areaUpscale32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f>`;
				namespace :ref:`InferenceEngine::gapi::kernels::avx<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx>`;
				namespace :ref:`InferenceEngine::gapi::kernels::avx512<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512>`;
				namespace :ref:`InferenceEngine::gapi::kernels::linear<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1linear>`;
				namespace :ref:`InferenceEngine::gapi::kernels::linear32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1linear32f>`;
				namespace :ref:`InferenceEngine::gapi::kernels::neon<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon>`;
		namespace :ref:`InferenceEngine::gpu<doxid-namespace_inference_engine_1_1gpu>`;
		namespace :ref:`InferenceEngine::itt<doxid-namespace_inference_engine_1_1itt>`;
			namespace :ref:`InferenceEngine::itt::domains<doxid-namespace_inference_engine_1_1itt_1_1domains>`;
	namespace :ref:`XMLParseUtils<doxid-namespace_x_m_l_parse_utils>`;
	namespace :ref:`cv<doxid-namespacecv>`;
	namespace :ref:`ngraph<doxid-namespacengraph>`;
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
	namespace :ref:`openvino<doxid-namespaceopenvino>`;
		namespace :ref:`openvino::cc<doxid-namespaceopenvino_1_1cc>`;
			namespace :ref:`openvino::cc::internal<doxid-namespaceopenvino_1_1cc_1_1internal>`;
		namespace :ref:`openvino::itt<doxid-namespaceopenvino_1_1itt>`;
	namespace :ref:`ov<doxid-namespaceov>`;
		namespace :ref:`ov::batch_util<doxid-namespaceov_1_1batch__util>`;
		namespace :ref:`ov::descriptor<doxid-namespaceov_1_1descriptor>`;
		namespace :ref:`ov::detail<doxid-namespaceov_1_1detail>`;
		namespace :ref:`ov::device<doxid-namespaceov_1_1device>`;
			namespace :ref:`ov::device::capability<doxid-namespaceov_1_1device_1_1capability>`;
		namespace :ref:`ov::element<doxid-namespaceov_1_1element>`;
		namespace :ref:`ov::frontend<doxid-namespaceov_1_1frontend>`;
		namespace :ref:`ov::hint<doxid-namespaceov_1_1hint>`;
		namespace :ref:`ov::intel_gna<doxid-namespaceov_1_1intel__gna>`;
		namespace :ref:`ov::intel_gpu<doxid-namespaceov_1_1intel__gpu>`;
			namespace :ref:`ov::intel_gpu::capability<doxid-namespaceov_1_1intel__gpu_1_1capability>`;
			namespace :ref:`ov::intel_gpu::hint<doxid-namespaceov_1_1intel__gpu_1_1hint>`;
			namespace :ref:`ov::intel_gpu::memory_type<doxid-namespaceov_1_1intel__gpu_1_1memory__type>`;
			namespace :ref:`ov::intel_gpu::ocl<doxid-namespaceov_1_1intel__gpu_1_1ocl>`;
		namespace :ref:`ov::intel_myriad<doxid-namespaceov_1_1intel__myriad>`;
			namespace :ref:`ov::intel_myriad::hddl<doxid-namespaceov_1_1intel__myriad_1_1hddl>`;
		namespace :ref:`ov::layout<doxid-namespaceov_1_1layout>`;
		namespace :ref:`ov::log<doxid-namespaceov_1_1log>`;
		namespace :ref:`ov::op<doxid-namespaceov_1_1op>`;
			namespace :ref:`ov::op::ShapeInferLSTM<doxid-namespaceov_1_1op_1_1_shape_infer_l_s_t_m>`;
			namespace :ref:`ov::op::ShapeInferRange<doxid-namespaceov_1_1op_1_1_shape_infer_range>`;
			namespace :ref:`ov::op::util<doxid-namespaceov_1_1op_1_1util>`;
				namespace :ref:`ov::op::util::detail<doxid-namespaceov_1_1op_1_1util_1_1detail>`;
				namespace :ref:`ov::op::util::error<doxid-namespaceov_1_1op_1_1util_1_1error>`;
				namespace :ref:`ov::op::util::rfft_common_validation<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation>`;
			namespace :ref:`ov::op::v0<doxid-namespaceov_1_1op_1_1v0>`;
			namespace :ref:`ov::op::v1<doxid-namespaceov_1_1op_1_1v1>`;
			namespace :ref:`ov::op::v3<doxid-namespaceov_1_1op_1_1v3>`;
			namespace :ref:`ov::op::v4<doxid-namespaceov_1_1op_1_1v4>`;
			namespace :ref:`ov::op::v5<doxid-namespaceov_1_1op_1_1v5>`;
			namespace :ref:`ov::op::v6<doxid-namespaceov_1_1op_1_1v6>`;
			namespace :ref:`ov::op::v7<doxid-namespaceov_1_1op_1_1v7>`;
			namespace :ref:`ov::op::v8<doxid-namespaceov_1_1op_1_1v8>`;
			namespace :ref:`ov::op::v9<doxid-namespaceov_1_1op_1_1v9>`;
		namespace :ref:`ov::opset1<doxid-namespaceov_1_1opset1>`;
		namespace :ref:`ov::opset2<doxid-namespaceov_1_1opset2>`;
		namespace :ref:`ov::opset3<doxid-namespaceov_1_1opset3>`;
		namespace :ref:`ov::opset4<doxid-namespaceov_1_1opset4>`;
		namespace :ref:`ov::opset5<doxid-namespaceov_1_1opset5>`;
		namespace :ref:`ov::opset6<doxid-namespaceov_1_1opset6>`;
		namespace :ref:`ov::opset7<doxid-namespaceov_1_1opset7>`;
		namespace :ref:`ov::opset8<doxid-namespaceov_1_1opset8>`;
		namespace :ref:`ov::opset9<doxid-namespaceov_1_1opset9>`;
		namespace :ref:`ov::pass<doxid-namespaceov_1_1pass>`;
			namespace :ref:`ov::pass::pattern<doxid-namespaceov_1_1pass_1_1pattern>`;
				namespace :ref:`ov::pass::pattern::op<doxid-namespaceov_1_1pass_1_1pattern_1_1op>`;
		namespace :ref:`ov::preprocess<doxid-namespaceov_1_1preprocess>`;
		namespace :ref:`ov::runtime<doxid-namespaceov_1_1runtime>`;
		namespace :ref:`ov::streams<doxid-namespaceov_1_1streams>`;
		namespace :ref:`ov::util<doxid-namespaceov_1_1util>`;
	namespace :ref:`std<doxid-namespacestd>`;

	// typedefs

	typedef std::unordered_map<std::shared_ptr<ov::opset1::Parameter>, std::unordered_set<size_t>> :target:`P2Btype<doxid-dimension__tracking_8hpp_1a186714ea70622d6cbc526d6f9bc65d24>`;
	typedef std::unordered_map<:ref:`ngraph::NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>`, std::function<bool(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>&, :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`, size_t idx)>> :ref:`type_to_fuse_map<doxid-group__ie__transformation__common__api_1ga0ebebd180aa26711fad395f5f8a60a1d>`;
	typedef std::vector<std::pair<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>> :target:`precisions_array<doxid-convert__precision_8hpp_1a4a87a7ac5af13aa6efaf3f00dadea5e1>`;
	typedef std::unordered_map<:ref:`ov::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`, std::function<void(const :ref:`ov::Node<doxid-classov_1_1_node>`&, std::ostream&ss)>> :target:`visualize_tree_ops_map_t<doxid-openvino_2pass_2visualize__tree_8hpp_1a2b6f709a98f49287ebb440f9b88ce8e7>`;

	// enums

	enum :ref:`AttributeSource<doxid-create__attribute_8hpp_1a78c045d573f15c7ad7bfb0accb0c162e>`;
	enum :ref:`CONVERSION_RESULT<doxid-convert__mul__add__to__scaleshift__or__power_8hpp_1a91a58c317f14f99fcb8660c5c69d9683>`;
	enum :ref:`ELTWISE_TYPE<doxid-eltwise_8hpp_1aca2b664f1fd62f182b07693d53c56611>`;

	// structs

	struct :ref:`parse_result<doxid-structparse__result>`;

	// classes

	class :ref:`AttributeParameters<doxid-class_attribute_parameters>`;
	template <InferenceEngine::Precision::ePrecision precision>
	class :ref:`BlobFactory<doxid-class_blob_factory>`;
	class :ref:`ConvertReduceBase<doxid-class_convert_reduce_base>`;
	class :ref:`MemorySolver<doxid-class_memory_solver>`;
	template <class T>
	class :ref:`SharedAttribute<doxid-class_shared_attribute>`;
	class :ref:`logstreambuf<doxid-classlogstreambuf>`;
	class :ref:`ngraph<doxid-classngraph>`;

	// global variables

	std::vector<int> :target:`strides<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1a971d047e7b3290908654e5b6a9c6794d>`;
	std::vector<int> :target:`dilation<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1ad7755135882ca7e19eb022defaf426a0>`;
	std::vector<int> :target:`pads_begin<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1a209fe97eb55ca08bd27be6304a67ce43>`;
	std::vector<int> :target:`pads_end<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1a9567ea499043c8933d9f033a2df072d8>`;
	std::vector<int> :target:`output_padding<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1a14891dbf0955c3b6c2328c3dd7011629>`;
	int :target:`N<doxid-ie__preprocess__gapi_8cpp_1a7722c8ecbb62d99aee7ce68b1752f337>`;
	int :target:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`;
	int :target:`H<doxid-ie__preprocess__gapi_8cpp_1affa487e8e3cc48473cfc05c0ce0165e9>`;
	int :target:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>`;
	Dims :target:`d<doxid-ie__preprocess__gapi_8cpp_1a9fde4026bb8d1fd3665712f8c1c7af46>`;
	Strides :target:`s<doxid-ie__preprocess__gapi_8cpp_1afc7998e50661eed237070df8aab0f2d6>`;
	int :target:`prec<doxid-ie__preprocess__gapi_8cpp_1a5bfbd3b409ebe4bc09f9ed58d177c2bd>`;
	cv::gapi::GKernelPackage& :target:`pckg<doxid-ie__preprocess__gapi__kernels_8cpp_1a35ad17062e8c505f41a7dde67d60a80d>`;
	:ref:`NGRAPH_EXTERN_C<doxid-ngraph__visibility_8hpp_1a16bc7e0d40a95f0a2e251f5f230eac77>` :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` const char \* :target:`NGRAPH_VERSION_NUMBER<doxid-ngraph_2version_8hpp_1ad3f867b253e9ed04eadfc352d18797cf>`;

	// global functions

	:target:`OV_CC_DOMAINS<doxid-conditional__compilation_2include_2openvino_2cc_2pass_2itt_8hpp_1abbdaa2233a69c2ae5c92acbce13296de>`(ov_pass);
	:target:`OV_CC_DOMAINS<doxid-snippets_2include_2snippets_2itt_8hpp_1a6da8bde711ff53dfb09f7d2784fc9ca4>`(internal_op);

	:ref:`CONVERSION_RESULT<doxid-convert__mul__add__to__scaleshift__or__power_8hpp_1a91a58c317f14f99fcb8660c5c69d9683>` :target:`check_constant<doxid-convert__mul__add__to__scaleshift__or__power_8hpp_1a0064a41857d89cb3aa24373156ec0cc4>`(
		const std::shared_ptr<:ref:`ngraph::op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`>& constant,
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& shape
		);

	template <class T>
	void :target:`shape_infer<doxid-core_2shape__inference_2include_2fake__quantize_8hpp_1a9a4eb4ea8f39e7fd9c6e17f998c9bb0c>`(
		const :ref:`ov::op::v0::FakeQuantize<doxid-classov_1_1op_1_1v0_1_1_fake_quantize>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <typename T>
	static auto :target:`remark<doxid-remarks_8hpp_1afcc9caf0b8dae78424d26d3509ff6af1>`(T x);

	template <class OpType, class T>
	void :target:`copy_shape_infer<doxid-core_2shape__inference_2include_2utils_8hpp_1a778e36d92e2d152f7c5d115146361bc7>`(
		const OpType \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class OpType, class T>
	void :target:`first_input_passthrough_infer<doxid-core_2shape__inference_2include_2utils_8hpp_1a9ff8b1ba2569ed500b244ed26333a93a>`(
		const OpType \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class OpType, class T>
	void :target:`eltwise_shape_infer<doxid-core_2shape__inference_2include_2utils_8hpp_1a022913dd32731a9d995615ef80033660>`(
		const OpType \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	bool :target:`get_data_as_int64<doxid-core_2shape__inference_2include_2utils_8hpp_1a73f9743a5a6207f16f92910a6d9291c3>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		std::vector<int64_t>& axes_value,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	bool :target:`get_data_as_int64< ov::PartialShape ><doxid-core_2shape__inference_2include_2utils_8hpp_1a189e0b90daafc057121d91fd5d16452c>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		std::vector<int64_t>& axes_value,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	bool :target:`get_data_as_float<doxid-core_2shape__inference_2include_2utils_8hpp_1a94bbbf7b2f83222f743d1fd127f52951>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		std::vector<float>& axes_value,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	bool :target:`get_data_as_float< ov::PartialShape ><doxid-core_2shape__inference_2include_2utils_8hpp_1ad94ee19ab9d76f04c74c7d0628124042>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		std::vector<float>& axes_value,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	bool :target:`get_data_as_shape<doxid-core_2shape__inference_2include_2utils_8hpp_1aefc933bf19b077ae8c9fedc740c1a634>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		T& shape,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	bool :target:`get_data_as_shape< ov::PartialShape ><doxid-core_2shape__inference_2include_2utils_8hpp_1af221fa6e26b740fdb1554da6dc348b22>`(
		size_t idx,
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& shape,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	void :target:`check_divided_result<doxid-core_2shape__inference_2include_2utils_8hpp_1a77867f8fd8086e15509644932cad080d>`(
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		const T& res,
		const T& divided,
		const typename T::value_type& divisor
		);

	void :target:`check_divided_result< ov::Dimension ><doxid-core_2shape__inference_2include_2utils_8hpp_1a64d2610e91960f67dedfce2e6a111f16>`(
		const :ref:`ov::Node<doxid-classov_1_1_node>` \* op,
		const :ref:`ov::Dimension<doxid-classov_1_1_dimension>`& res,
		const :ref:`ov::Dimension<doxid-classov_1_1_dimension>`& divided,
		const typename :ref:`ov::Dimension::value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>`& divisor
		);

	template <typename T>
	std::vector<T> :target:`read_vector<doxid-core_2include_2ngraph_2util_8hpp_1a21fc498e70c7fd0b1d3b4d9b2587242f>`(std::shared_ptr<:ref:`ngraph::runtime::Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`> tv);

	template <typename T>
	std::vector<T> :target:`host_tensor_2_vector<doxid-core_2include_2ngraph_2util_8hpp_1a8577d004922f15c1d608faf4afbcf570>`(:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` tensor);

	std::vector<float> :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :target:`read_float_vector<doxid-core_2include_2ngraph_2util_8hpp_1a446b3b780ec9e6528a57ba2827a720fe>`(std::shared_ptr<:ref:`ngraph::runtime::Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`> tv);
	std::vector<int64_t> :ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` :target:`read_index_vector<doxid-core_2include_2ngraph_2util_8hpp_1a3dc83efc18dd95650559a8953a855789>`(std::shared_ptr<:ref:`ngraph::runtime::Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`> tv);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::ostream& :target:`operator <<<doxid-core_2include_2ngraph_2util_8hpp_1a920e81daad0923523d473d171700fe06>` (
		std::ostream& os,
		const :ref:`ngraph::NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& nv
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` const char \* :target:`get_ngraph_version_string<doxid-ngraph_2version_8hpp_1a36336622816db5295cd3ee9eee300e04>`();

	template <class T>
	void :target:`dynamic_inference<doxid-reduce__shape__inference_8hpp_1a917554eb02813b0f1b8a082f76c49bd7>`(
		const T& input_shape,
		T& output_shape,
		bool keep_dims
		);

	void :target:`dynamic_inference< ov::PartialShape ><doxid-reduce__shape__inference_8hpp_1ab4b779a798e2c37e07e6fe678c5b7cb9>`(
		const :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& output_shape,
		bool keep_dims
		);

	template <class T>
	void :target:`reduce_shape_infer<doxid-reduce__shape__inference_8hpp_1a8e85516b6b9b72c1c0bbf15e958c260b>`(
		const :ref:`ov::op::util::ReductionBase<doxid-classov_1_1op_1_1util_1_1_reduction_base>` \* op,
		bool keep_dims,
		const T& input_shape,
		T& output_shape,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-reduce__shape__inference_8hpp_1ad3b54c89be82a9f60478c502c5df3d58>`(
		const :ref:`ov::op::util::ArithmeticReductionKeepDims<doxid-classov_1_1op_1_1util_1_1_arithmetic_reduction_keep_dims>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-reduce__shape__inference_8hpp_1a5b0d45306669162f127a8e7f25de8948>`(
		const :ref:`ov::op::util::LogicalReductionKeepDims<doxid-classov_1_1op_1_1util_1_1_logical_reduction_keep_dims>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-scatter__nd__base__shape__inference_8hpp_1aff058a4cce0958177ec91c379af480a8>`(
		const :ref:`ov::op::util::ScatterNDBase<doxid-classov_1_1op_1_1util_1_1_scatter_n_d_base>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-shape__nodes_8hpp_1a8f8707956c3fb316aa519c0cf31fc42e>`(
		const ov::opset1::Reshape \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	void :target:`shape_infer< ov::PartialShape ><doxid-shape__nodes_8hpp_1a860045eb9b81b492cc1a5ac3f041cdf9>`(
		const ov::opset1::Reshape \* op,
		const std::vector<:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& input_shapes,
		std::vector<:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	void :target:`shape_infer<doxid-shape__nodes_8hpp_1ae37598e343c54af783febbb787353eb1>`(
		const ov::opset1::Squeeze \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	void :target:`shape_infer< ov::PartialShape ><doxid-shape__nodes_8hpp_1aab2fc6db5fd186e82dfee2066a14fac2>`(
		const ov::opset1::Squeeze \* op,
		const std::vector<:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& input_shapes,
		std::vector<:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	void :target:`shape_infer<doxid-shape__nodes_8hpp_1ad339c6afa4715dfa0c2fd1ffa2e15c30>`(
		const ov::opset1::Unsqueeze \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	void :target:`shape_infer< ov::PartialShape ><doxid-shape__nodes_8hpp_1a0e9c45dce1cd87d05a3e3d85bf68de73>`(
		const ov::opset1::Unsqueeze \* op,
		const std::vector<:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& input_shapes,
		std::vector<:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	void :target:`dynamic_shape<doxid-shape__nodes_8hpp_1aadccff6786e62821ab147c6a8c4e9751>`(T& output_shape);

	void :target:`dynamic_shape< ov::PartialShape ><doxid-shape__nodes_8hpp_1a5001782edc078a52d6b614f820e57429>`(:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& output_shape);

	template <class T>
	void :target:`shape_of_shape_infer<doxid-shape__nodes_8hpp_1a342a95883933f414d9d692b9074f06e4>`(
		const T& input_shape,
		T& output_shape
		);

	template <class T>
	void :target:`shape_infer<doxid-shape__nodes_8hpp_1a3cc4c7a47a1ee51158f36a6c5a8bd50c>`(
		const ov::opset1::ShapeOf \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-shape__nodes_8hpp_1a61af23944e6dcd3ec81e2bf81b34df11>`(
		const ov::opset3::ShapeOf \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1gaadd202fa37fcc6b9d70730a234dd4462>`(const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1ga10da7f895f6cd2913584bde98b086efb>`(
		const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		void \* ptr
		);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1ga4abc8b57f26279d43b011a1a854f5409>`(
		const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
		const std::shared_ptr<:ref:`InferenceEngine::IAllocator<doxid-class_inference_engine_1_1_i_allocator>`>& alloc
		);

	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_plain_blob<doxid-group__ie__dev__api__memory_1ga1129ba1b599e4c0c8c781332bd67b681>`(
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` prec,
		const :ref:`InferenceEngine::SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>` dims
		);

	template <class... Args>
	:ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`make_blob_with_precision<doxid-group__ie__dev__api__memory_1ga8f4ac3993c12237c05c69d374d6bc724>`(
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` precision,
		Args&&... args
		);

	template <typename T>
	void :ref:`CopyVectorToBlob<doxid-group__ie__dev__api__memory_1gae5d15938c3ed40428c2611eed62ed5f9>`(
		const :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` outputBlob,
		const std::vector<T>& inputVector
		);

	int :ref:`ie_memcpy<doxid-group__ie__dev__api__memory_1gabe0c99cd9de11e89f0bdebc3023e6083>`(void \* dest, size_t destsz, void const \* src, size_t count);
	:ref:`parse_result<doxid-structparse__result>` :ref:`ParseXml<doxid-group__ie__dev__api__xml_1gae75292063abf9fa018da463f1960a846>`(const char \* file_path);

	// macros

	#define :ref:`AUTO_CONFIG_KEY<doxid-ie__plugin__config_8hpp_1a7c9db10b002aa799ba6d198c61c5c743>`(name)
	#define :ref:`BWDCMP_RTTI_DECLARATION<doxid-rtti_8hpp_1a95c39aa70e3b5ce8055a31a5df9c4875>`
	#define :target:`BWDCMP_RTTI_DEFINITION<doxid-rtti_8hpp_1a970a03cb8ee809158f0914256e0aacea>`(CLASS)
	#define :target:`CALL_OVERLOAD<doxid-openvino_2core_2except_8hpp_1a4bd526b7fc3f94a8e802c3a4ab57611d>`(name, exc_class, ctx, ...)
	#define :ref:`CLDNN_CONFIG_KEY<doxid-cldnn__config_8hpp_1ad2e237cf3c04453361a0a6f743d0a719>`(name)
	#define :target:`CL_HPP_MINIMUM_OPENCL_VERSION<doxid-gpu__ocl__wrapper_8hpp_1a2053025c576bcf48e249dd20e884a560>`
	#define :target:`CL_HPP_TARGET_OPENCL_VERSION<doxid-gpu__ocl__wrapper_8hpp_1a37ea07405ca286c1570612b42d43b345>`
	#define :ref:`CONFIG_KEY<doxid-ie__plugin__config_8hpp_1aad09cfba062e8ec9fb7ab9383f656ec7>`(name)
	#define :ref:`CONFIG_KEY_INTERNAL<doxid-group__ie__dev__api__plugin__api_1ga467101d10535ee20c68d110957c75334>`(name)
	#define :ref:`CONFIG_VALUE<doxid-ie__plugin__config_8hpp_1a2b1801501dc6436ffa1a9ed9c6333b40>`(name)
	#define :ref:`CONFIG_VALUE_INTERNAL<doxid-group__ie__dev__api__plugin__api_1ga698a6c9b92df3c0cd02d89c17b07d8c3>`(name)
	#define :target:`COPY_TENSOR<doxid-eval__copy_8hpp_1a9e0de6e69d358cf6ff996a4398e0636f>`(a)
	#define :target:`COUNT_ARGS_MAXN<doxid-openvino_2core_2except_8hpp_1a03379093102361991e3355418a64ba1c>`(...)
	#define :target:`CPU_SIMD<doxid-ie__preprocess__gapi__kernels__impl_8hpp_1a4bc3c36d20772df00268e35d25532ec9>`
	#define :target:`CV_AVX2<doxid-ie__preprocess__gapi__kernels__avx2_8cpp_1afbdfb44f2fffc0a3a5ef2f632f9610c2>`
	#define :target:`CV_AVX512_SKX<doxid-ie__preprocess__gapi__kernels__avx512_8cpp_1a40295f2dfc24e1458bf35b20d2a0510f>`
	#define :target:`CV_CPU_HAS_SUPPORT_SSE2<doxid-ie__preprocess__gapi__kernels__avx2_8cpp_1ac955709ab048b6a9a44eed739da04761>`
	#define :target:`CV_CPU_HAS_SUPPORT_SSE2<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1ac955709ab048b6a9a44eed739da04761>`
	#define :target:`CV_CPU_HAS_SUPPORT_SSE2<doxid-ie__preprocess__gapi__kernels__avx512_8cpp_1ac955709ab048b6a9a44eed739da04761>`
	#define :target:`CV_NEON<doxid-ie__preprocess__gapi__kernels__neon_8cpp_1ad9832551140b180854524a738a6ac728>`
	#define :target:`CV_SIMD128<doxid-ie__preprocess__gapi__kernels__neon_8cpp_1ad953f90887e4eb9a12657e6a1f86d01b>`
	#define :target:`CV_SIMD128<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1ad953f90887e4eb9a12657e6a1f86d01b>`
	#define :target:`CV_SIMD256<doxid-ie__preprocess__gapi__kernels__avx2_8cpp_1af9b7ce8e57aeb415af75f31fd4a33aec>`
	#define :target:`CV_SIMD512<doxid-ie__preprocess__gapi__kernels__avx512_8cpp_1aae046dce22790e9d40874766ea9e4214>`
	#define :target:`CV_SSE<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1a70eb1f83a29647a5b687f1679494bfa6>`
	#define :target:`CV_SSE2<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1a78a9711c63bbde857223017dc18b28f8>`
	#define :target:`CV_SSE3<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1ae60b5062750990a226adb984179d393b>`
	#define :target:`CV_SSE4_1<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1a61df95f4c6eb42819e88083d7052336b>`
	#define :target:`CV_SSE4_2<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1a3a9f59ec4dacd78b8dabfc5f1f41147b>`
	#define :target:`CV_SSSE3<doxid-ie__preprocess__gapi__kernels__sse42_8cpp_1a94cb438fa65b9a844870eca8c18d95e8>`
	#define :ref:`DECLARE_GPU_PARAM_KEY<doxid-gpu__params_8hpp_1a7c86c40f2e7948bb6c5de3adc8be196c>`(name, ...)
	#define :ref:`DECLARE_GPU_PARAM_VALUE<doxid-gpu__params_8hpp_1a060c89ece9f8f5a1182dd03fdf57d5ea>`(name)
	#define :ref:`DEFINE_PROP<doxid-ie__layers_8h_1ad266549c8747e8451c058de008f2331e>`(prop_name)
	#define :ref:`EXEC_NETWORK_METRIC_KEY<doxid-ie__plugin__config_8hpp_1adb48efa632ae9bacfa86b8a3a0d9541e>`(name)
	#define :target:`EXPAND_ARGS<doxid-openvino_2core_2except_8hpp_1a7ebef3481d8ef1c43ecd71a44dd5c0cb>`(args)
	#define :ref:`FOREACH_CHILD<doxid-group__ie__dev__api__xml_1ga1ea10f15c23d651affba4c9ec3c910b4>`(c, p, tag)
	#define :target:`FRONTEND_API<doxid-frontends_2common_2include_2openvino_2frontend_2visibility_8hpp_1acfd11755e29560fd36ce5369ba155288>`
	#define :target:`FRONTEND_C_API<doxid-frontends_2common_2include_2openvino_2frontend_2visibility_8hpp_1add76080470af5187f995abf5d75f2e0a>`
	#define :ref:`FRONT_END_CHECK_IMPLEMENTED<doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1addbb9b81cba65edbb9156def7b9dcdfe>`(COND, NAME)
	#define :ref:`FRONT_END_GENERAL_CHECK<doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1ae8c595f7a105bb22f095247bcb78bba4>`(...)
	#define :ref:`FRONT_END_INITIALIZATION_CHECK<doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1aee169f84aff92500e8aba1fe3f48e7bf>`(...)
	#define :ref:`FRONT_END_NOT_IMPLEMENTED<doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1a5e008e66e26d93062e3fa10835dfb8bc>`(NAME)
	#define :ref:`FRONT_END_OP_CONVERSION_CHECK<doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1a80d6bce097f283d05d39913b61900c51>`(...)
	#define :ref:`FRONT_END_THROW<doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1a58b0ba5a2a92e3cdb97aa0bdf68fcd5b>`(MSG)
	#define :target:`GLUE<doxid-openvino_2core_2except_8hpp_1ab1561dd2afc88075c7a3b010f5f6b857>`(x, y)
	#define :ref:`GNA_CONFIG_KEY<doxid-gna__config_8hpp_1a8124b15c4055e25f8c5792f2afe1e822>`(name)
	#define :ref:`GNA_CONFIG_VALUE<doxid-gna__config_8hpp_1a208a60b02fdd02d379486a1625bf5ebc>`(name)
	#define :ref:`GPU_CONFIG_KEY<doxid-gpu__config_8hpp_1a13885ca77f3ccedfe592638155fea12f>`(name)
	#define :ref:`GPU_METRIC_KEY<doxid-gpu__config_8hpp_1a466af595ab1b49582c27d8f6fff87b16>`(name)
	#define :ref:`GPU_PARAM_KEY<doxid-gpu__params_8hpp_1a7aedafe279f57c6fca380e3fe8538993>`(name)
	#define :ref:`GPU_PARAM_VALUE<doxid-gpu__params_8hpp_1ae3caba30e291cdbfc5b2959b7289699b>`(name)
	#define :ref:`HETERO_CONFIG_KEY<doxid-hetero__plugin__config_8hpp_1aa455ce33b7e7a245be639015625a9768>`(name)
	#define :target:`HSUM<doxid-ie__preprocess__gapi__kernels__simd__impl_8hpp_1ae1a8809125608159b2562979537dde2f>`(xmaxdf)
	#define :ref:`IE_ASSERT<doxid-ie__common_8h_1af7eb522bba9d110ae52c00dc1ef2f28a>`(EXPRESSION)
	#define :ref:`IE_CREATE_EXTENSION<doxid-ie__iextension_8h_1ad45c2c4e5155992e79925d0e2ba5138b>`
	#define :ref:`IE_CREATE_PLUGIN<doxid-group__ie__dev__api__plugin__api_1ga99b18089a6c2b980a7b68538886041ae>`
	#define :ref:`IE_DEFINE_EXTENSION_CREATE_FUNCTION<doxid-ie__iextension_8h_1a9138b9e722336fddd0f92bad2a55d809>`(ExtensionType)
	#define :target:`IE_DEFINE_EXTENSION_CREATE_FUNCTION_DECLARATION<doxid-ie__iplugin__internal_8hpp_1a0261475afe9c4a6f9e4b54a4cecbe5c6>`(_IE_CREATE_EXTENSION_FUNC)
	#define :ref:`IE_DEFINE_PLUGIN_CREATE_FUNCTION<doxid-group__ie__dev__api__plugin__api_1ga06b197cbe37f59f94b15a7d861e17d4e>`(PluginType, version, ...)
	#define :target:`IE_DEFINE_PLUGIN_CREATE_FUNCTION_DECLARATION<doxid-ie__iplugin__internal_8hpp_1af683e8ed9b37a597dda5410a5d47b11b>`(_IE_CREATE_PLUGIN_FUNC)
	#define :ref:`IE_EXCEPTION_SWITCH<doxid-ie__common_8h_1a2cecd150192b914ca06109942ce35c17>`(STATUS, TYPE_ALIAS, ...)
	#define :ref:`IE_SET_METRIC_RETURN<doxid-group__ie__dev__api_1gad59db954d9dfcbd6f490d5cbadd3a91d>`(name, ...)
	#define :ref:`IE_THROW<doxid-ie__common_8h_1a643ef2aa5e1c6b7523e55cc4396e3e02>`(...)
	#define :ref:`IE_VERSION_MAJOR<doxid-ie__version_8hpp_1a0a2d5226e0373446c5d8d034bbeb2e75>`
	#define :ref:`IE_VERSION_MINOR<doxid-ie__version_8hpp_1adfa9ccfc2f67d4d66890433e29dc7e8e>`
	#define :ref:`IE_VERSION_PATCH<doxid-ie__version_8hpp_1a9e7a9f9e8c6b963d51bab07e89b15206>`
	#define :target:`ITT_FUNCTION_NAME<doxid-function__name_8hpp_1ae29f9510fc7e8bb2bb2a73264dc26368>`
	#define :target:`LP_TRANSFORMATIONS_API<doxid-lpt__visibility_8hpp_1ae2bce57c581a107062bfc8672c002f48>`
	#define :target:`MANUAL_SIMD<doxid-ie__preprocess__gapi__kernels__impl_8hpp_1a5688e3cf23b2658c1fce2a5336a5c956>`
	#define :target:`MATCHER_SCOPE<doxid-conditional__compilation_2include_2openvino_2cc_2pass_2itt_8hpp_1a3d1377542bcf3e305c33a1b683cc77df>`(region)
	#define :ref:`METRIC_KEY<doxid-ie__plugin__config_8hpp_1a69d0efa20c5b2bec020a706279f0c7be>`(name)
	#define :ref:`METRIC_VALUE<doxid-ie__plugin__config_8hpp_1ad6dd157c1a4d27888bfdcdf1b64cfdb2>`(name)
	#define :ref:`MULTI_CONFIG_KEY<doxid-multi__device__config_8hpp_1aa887cd604b772a3a51ba73f9652ae6c4>`(name)
	#define :target:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>`
	#define :target:`NGRAPH_API_C<doxid-ngraph__visibility_8hpp_1a29d32bf9bba6283f5d31c48674a124f0>`
	#define :target:`NGRAPH_CHECK<doxid-check_8hpp_1a78178cbea0b16cd91a8b9d78bcc7d6aa>`(...)
	#define :target:`NGRAPH_CHECK_HELPER<doxid-check_8hpp_1a13c512cf91ada94121568cc44afa67e0>`(exc_class, ctx, ...)
	#define :target:`NGRAPH_CHECK_HELPER1<doxid-check_8hpp_1a96ecae0f9668d2301c174890a4936792>`(exc_class, ctx, check)
	#define :target:`NGRAPH_CHECK_HELPER2<doxid-check_8hpp_1a9ffba01fa7c0141b8e41066a75e90977>`(exc_class, ctx, check, ...)
	#define :target:`NGRAPH_DEBUG<doxid-core_2include_2ngraph_2log_8hpp_1a64b99dc9fe7e6ae5771796a3fe43b2e7>`
	#define :target:`NGRAPH_DEPRECATED<doxid-ngraph_2deprecated_8hpp_1ac2e70f5d068a06fafc17d3a4ee0c4bc0>`(msg)
	#define :target:`NGRAPH_ENUM_DEPRECATED<doxid-ngraph_2deprecated_8hpp_1ad59a2f6f26befae0bc58f38eb103d351>`(msg)
	#define :target:`NGRAPH_ERR<doxid-core_2include_2ngraph_2log_8hpp_1a2b88eac0af3891f694ba87cb853817c9>`
	#define :target:`NGRAPH_EXTERN_C<doxid-ngraph__visibility_8hpp_1a16bc7e0d40a95f0a2e251f5f230eac77>`
	#define :target:`NGRAPH_HELPER_DLL_EXPORT<doxid-core_2include_2ngraph_2visibility_8hpp_1ae697dc9472bcd9a6855fa6eebc109703>`
	#define :target:`NGRAPH_HELPER_DLL_IMPORT<doxid-core_2include_2ngraph_2visibility_8hpp_1aab59302496f54a24abf8ac427718befe>`
	#define :target:`NGRAPH_INFO<doxid-core_2include_2ngraph_2log_8hpp_1a7c3c72351be141c0f4b1763e624ae861>`
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset1_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset2_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset8_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset3_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset5_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset4_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset6_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset9_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-snippets__isa_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :target:`NGRAPH_OP<doxid-ngraph_2opsets_2opset7_8hpp_1a924031188a855320871a76f179e190e6>`(a, b)
	#define :ref:`NGRAPH_RTTI_DECLARATION<doxid-ngraph_2node_8hpp_1a479e20cfdaf3d59d557207ea9033f4a0>`
	#define :target:`NGRAPH_RTTI_DEFINITION<doxid-ngraph_2node_8hpp_1ae2db7e538b0564dea208fbceb77b0b2b>`(...)
	#define :target:`NGRAPH_SUPPRESS_DEPRECATED_END<doxid-ngraph_2deprecated_8hpp_1a2269e92d442f8e165baa175083398bf1>`
	#define :target:`NGRAPH_SUPPRESS_DEPRECATED_START<doxid-ngraph_2deprecated_8hpp_1a801c992c38d3ade2284e3c5a3734e67f>`
	#define :target:`NGRAPH_UNREACHABLE<doxid-check_8hpp_1a29a82f9233ba70cb8b46a5ad3dccb742>`(...)
	#define :target:`NGRAPH_WARN<doxid-core_2include_2ngraph_2log_8hpp_1a52d7295458e6dbd60869fbd1a1036295>`
	#define :target:`NODE_VALIDATION_CHECK<doxid-openvino_2core_2node_8hpp_1ae50bd22e1aad9498757a6dbfa3759123>`(node, ...)
	#define :target:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>`
	#define :target:`OPENVINO_API_C<doxid-core__visibility_8hpp_1a51ad39a7c986460139f7dce0ee0ffc3d>`(...)
	#define :ref:`OPENVINO_ASSERT<doxid-openvino_2core_2except_8hpp_1a7ff78e5accf3159b30b4b32bbb72d272>`(...)
	#define :target:`OPENVINO_ASSERT_HELPER<doxid-openvino_2core_2except_8hpp_1a912224f9dac2a0e93ab30803a29c2aae>`(exc_class, ctx, ...)
	#define :target:`OPENVINO_ASSERT_HELPER1<doxid-openvino_2core_2except_8hpp_1a5da68c3a6cccbd15236e250feb8db363>`(exc_class, ctx, check)
	#define :target:`OPENVINO_ASSERT_HELPER2<doxid-openvino_2core_2except_8hpp_1afdf925bb11bc3014ad76924446950d45>`(exc_class, ctx, check, ...)
	#define :ref:`OPENVINO_CREATE_EXTENSIONS<doxid-core_2include_2openvino_2core_2extension_8hpp_1acdadcfa0eff763d8b4dadb8a9cb6f6e6>`(extensions)
	#define :target:`OPENVINO_DEBUG<doxid-common_2util_2include_2openvino_2util_2log_8hpp_1a94e1b1d83810782106336c9f68fe88e5>`
	#define :target:`OPENVINO_ERR<doxid-common_2util_2include_2openvino_2util_2log_8hpp_1a03aef89a1252bc2da4ef14443f53d751>`
	#define :target:`OPENVINO_EXTENSION_API<doxid-core_2include_2openvino_2core_2extension_8hpp_1a1af3c70880424d539c5ccb56ebbfe781>`
	#define :target:`OPENVINO_EXTENSION_C_API<doxid-core_2include_2openvino_2core_2extension_8hpp_1a082013202dec7824df2d71650035dc2f>`
	#define :target:`OPENVINO_FRAMEWORK_MAP<doxid-frontends_2common_2include_2openvino_2frontend_2extension_2op_8hpp_1a7c6aeac48d78bb1f8df0930011653d50>`(FRAMEWORK, ...)
	#define :target:`OPENVINO_INFO<doxid-common_2util_2include_2openvino_2util_2log_8hpp_1aa4238f569cf919d9bc40d12a5b6626a0>`
	#define :target:`OPENVINO_NOT_IMPLEMENTED<doxid-openvino_2core_2except_8hpp_1a2ba30768d4f5f983d2ed11f9aefefdd1>`
	#define :target:`OPENVINO_OP<doxid-core_2include_2openvino_2op_2op_8hpp_1afe347dcc52f829ca1c7693241f35957b>`(...)
	#define :ref:`OPENVINO_RTTI<doxid-rtti_8hpp_1a00d4d2c156da8f59cbc4e671b0e2ff33>`(...)
	#define :ref:`OPENVINO_UNREACHABLE<doxid-openvino_2core_2except_8hpp_1af19405fcee2589306ccc9288fe253b62>`(...)
	#define :ref:`OPENVINO_VERSION_MAJOR<doxid-openvino_2core_2version_8hpp_1a8cf5c3a5fcc3032007ac29e160f2b8b0>`
	#define :ref:`OPENVINO_VERSION_MINOR<doxid-openvino_2core_2version_8hpp_1a9886d64c4de9b93730bc318cf8437b18>`
	#define :ref:`OPENVINO_VERSION_PATCH<doxid-openvino_2core_2version_8hpp_1ad0ff746021e0e7f76ddb964be244f29e>`
	#define :target:`OPENVINO_WARN<doxid-common_2util_2include_2openvino_2util_2log_8hpp_1a592cc23944ab100b07a811ad0a4c6667>`
	#define :target:`OVERLOAD_MACRO<doxid-openvino_2core_2except_8hpp_1a05efee9239b4c9ed9f3a31883ed9e503>`(name, count)
	#define :target:`OVERLOAD_MACRO1<doxid-openvino_2core_2except_8hpp_1a60d0ad1d8fb2875ec803daf7a449a363>`(name, count)
	#define :target:`OVERLOAD_MACRO2<doxid-openvino_2core_2except_8hpp_1aea6524a745d3d53fc56fd8a306ee2721>`(name, count)
	#define :target:`OV_CASE<doxid-selective__build_8h_1a35a931b8e94f048c628b74aefea0ca57>`(Case, Type)
	#define :target:`OV_CASE2<doxid-selective__build_8h_1ae4583e5d67b0ee999c4ebdb5335f0467>`(Case1, Case2, Type1, Type2)
	#define :target:`OV_CC_CAT<doxid-selective__build_8h_1af31abe0b92137027c5e869f26c60976a>`
	#define :target:`OV_CC_EXPAND<doxid-selective__build_8h_1a348bc7ecb457a1ab7c7552108e56240d>`
	#define :target:`OV_CC_TOSTRING<doxid-selective__build_8h_1a5c12061937e6a0d540b64669c79da682>`
	#define :target:`OV_COLLECT_ATTACHED_EXTENSIONS<doxid-op__extension_8hpp_1a02f66e3df3c4a5444a862d5a16b6b254>`(FRAMEWORK)
	#define :target:`OV_FRONTEND_API_VERSION<doxid-frontends_2common_2include_2openvino_2frontend_2visibility_8hpp_1aa16ffbdbee1b30f4a5145ba75992e47e>`
	#define :ref:`OV_ITT_DOMAIN<doxid-group__ie__dev__profiling_1ga83ad6f539c8e1aef944160e37fcfcb4d>`(...)
	#define :target:`OV_ITT_GROUP<doxid-itt_2include_2openvino_2itt_8hpp_1a18c28b85b57620668504727782c9b178>`(group)
	#define :ref:`OV_ITT_SCOPE<doxid-group__ie__dev__profiling_1gab36eff302250b41b12848597e5684d68>`(group, ...)
	#define :ref:`OV_ITT_SCOPED_TASK<doxid-group__ie__dev__profiling_1gac1e4b5bdc6097e2afd26b75d05dfe1ef>`(...)
	#define :target:`OV_ITT_SCOPE_CHAIN<doxid-itt_2include_2openvino_2itt_8hpp_1afc17d40d323323971eedbdbf34c824d4>`(group, ...)
	#define :ref:`OV_ITT_SCOPE_NEXT<doxid-group__ie__dev__profiling_1ga47367f3d199b8f71534fd3f7fb9b2464>`(group, ...)
	#define :ref:`OV_ITT_SCOPE_SKIP<doxid-group__ie__dev__profiling_1gadde35caedd8df731ec882463b4f812be>`(group, chainId)
	#define :ref:`OV_ITT_TASK_CHAIN<doxid-group__ie__dev__profiling_1gaa9f15503cbc6a9fe20091ded356e17dd>`(...)
	#define :ref:`OV_ITT_TASK_NEXT<doxid-group__ie__dev__profiling_1ga319de5d71d3550d2638188e9fb7be3b5>`(...)
	#define :ref:`OV_ITT_TASK_SKIP<doxid-group__ie__dev__profiling_1ga1381f651372b35303eea8009a7ebbd2e>`(chainId)
	#define :target:`OV_PP_ARG_N<doxid-pp_8hpp_1a5e790d25cbcfd253dac495d6ae89ebc7>`(_0, _1, _2, _3, _4, N, ...)
	#define :target:`OV_PP_ARG_PLACEHOLDER_1<doxid-pp_8hpp_1a56db69686159de0b40bb476890e809fb>`
	#define :target:`OV_PP_CAT<doxid-pp_8hpp_1a612dd46abeb39d2f926109f8e1053beb>`(x, y)
	#define :target:`OV_PP_CAT3<doxid-pp_8hpp_1a59dbe4735c4e3719d81480aa1166c3a1>`(x, y, z)
	#define :target:`OV_PP_CAT3_<doxid-pp_8hpp_1afd7403d3b64ebbb74b78831d68a73e1a>`(x, y, z)
	#define :target:`OV_PP_CAT4<doxid-pp_8hpp_1a5960ff66841447206463603d311c29cf>`(x, y, z, w)
	#define :target:`OV_PP_CAT4_<doxid-pp_8hpp_1a635a6aa7f11d7b13692e3acce535802b>`(x, y, z, w)
	#define :target:`OV_PP_CAT_<doxid-pp_8hpp_1afdedb4664f439e8b30760c6b522a37aa>`(x, y)
	#define :target:`OV_PP_EXPAND<doxid-pp_8hpp_1ad806d90e59484abb20dac54459cfc638>`(X)
	#define :target:`OV_PP_IS_ENABLED<doxid-pp_8hpp_1a8b74b93db549f42008484b25a9514a40>`(x)
	#define :target:`OV_PP_IS_ENABLED1<doxid-pp_8hpp_1a7ff2dde6fac67f82d13c270293860dcf>`(val)
	#define :target:`OV_PP_IS_ENABLED2<doxid-pp_8hpp_1a4539f52ad33e777c8b9efe7796605ebb>`(arg1_or_junk)
	#define :target:`OV_PP_NARG<doxid-pp_8hpp_1a49a9b268ccbd2854d82ef8bc964e4fb5>`(...)
	#define :target:`OV_PP_NARG_<doxid-pp_8hpp_1aec5c441a60e6e048f0c42dd35eac9023>`(...)
	#define :target:`OV_PP_NO_ARGS<doxid-pp_8hpp_1acecf61145a9dc684a039662638f136b2>`(NAME)
	#define :target:`OV_PP_OVERLOAD<doxid-pp_8hpp_1a77d37ee60c77ec0a567f8225b93371c0>`(NAME, ...)
	#define :target:`OV_PP_RSEQ_N<doxid-pp_8hpp_1ad504fd5ccfec1e5efe603ac642b087fe>`()
	#define :target:`OV_PP_SECOND_ARG<doxid-pp_8hpp_1ae17c415482bf394d6c5d9f7004bab595>`(...)
	#define :target:`OV_PP_SECOND_ARG_<doxid-pp_8hpp_1a17c7a49f786a32a8273ee44c5aef1c31>`(...)
	#define :target:`OV_PP_SECOND_ARG_GET<doxid-pp_8hpp_1a1052d448ef0c59f61803f3a37fe00a3e>`(ignored, val, ...)
	#define :target:`OV_PP_TOSTRING<doxid-pp_8hpp_1a21670824fa7f134192a53cce80129ad8>`(...)
	#define :target:`OV_PP_TOSTRING_<doxid-pp_8hpp_1a141f8fbf3f3b42a4f844e20d66c2f0cd>`(...)
	#define :target:`OV_PREPROC_PLUGIN_CALL_STATEMENT<doxid-ie__preprocess__data_8hpp_1a4f586e3b71d4f1722797978b7d055caf>`(...)
	#define :target:`OV_SWITCH<doxid-selective__build_8h_1a2742bb50365b3b73b170cf2fceaa884f>`(Module, fn, ctx, val, ...)
	#define :target:`PROJECT_ROOT_DIR<doxid-core_2include_2ngraph_2log_8hpp_1abb433164e0846871fed15fd225e445d4>`
	#define :target:`PROJECT_ROOT_DIR<doxid-common_2util_2include_2openvino_2util_2log_8hpp_1abb433164e0846871fed15fd225e445d4>`

	#define :target:`RETURN_ARG_COUNT<doxid-openvino_2core_2except_8hpp_1a5241dd46d9608d78ac9ac4109d94efd9>`( \
		_1_, \
		_2_, \
		_3_, \
		_4_, \
		_5_, \
		_6, \
		_7, \
		_8, \
		_9, \
		_10, \
		_11, \
		_12, \
		_13, \
		_14, \
		_15, \
		_16, \
		_17, \
		_18, \
		_19, \
		_20, \
		_21, \
		_22, \
		_23, \
		_24, \
		_25, \
		count, \
		... \
		)

	#define :target:`THROW_IE_LPT_EXCEPTION<doxid-ie__lpt__exception_8hpp_1a03459d975cddf78577d2c13e2808357e>`(node)
	#define :target:`THROW_TRANSFORMATION_EXCEPTION<doxid-ie__lpt__exception_8hpp_1ac0b460d6a654c83e284c37d7558352b1>`
	#define :target:`TRANSFORMATIONS_API<doxid-transformations__visibility_8hpp_1a1599ac26d40b94c599e76283ca59f46c>`
	#define :ref:`TYPE_CASE<doxid-openvino_2core_2node_8hpp_1a3fc5fb5b6a59e5bf8afcd4d1d2f8b50e>`(a)
	#define :target:`USE_CVKL<doxid-ie__preprocess__gapi__kernels__impl_8hpp_1a93823db235b47ed3bf36353be25a4328>`
	#define :target:`USE_FACTORY<doxid-blob__factory_8hpp_1aaf0b98c94cba9aada16f65616a332c8d>`(precision)
	#define :target:`_IE_SUPPRESS_DEPRECATED_END_MSVC<doxid-ie__layers_8h_1a7b18869017f6007746cef87d671344be>`
	#define :target:`_IE_SUPPRESS_DEPRECATED_START_MSVC<doxid-ie__layers_8h_1a20087e53215d44082e255ea5944a1ecd>`
	#define :target:`_NGRAPH_RTTI_DEFINITION_COMMON<doxid-ngraph_2node_8hpp_1aca33e8c426ef215e1eb2b716edf468b6>`(CLASS)
	#define :target:`_NGRAPH_RTTI_DEFINITION_NO_PARENT<doxid-ngraph_2node_8hpp_1ac930e14fd79812a2a95879d023622bc3>`(CLASS, TYPE_NAME, _VERSION_INDEX)

	#define :target:`_NGRAPH_RTTI_DEFINITION_WITH_PARENT<doxid-ngraph_2node_8hpp_1ad8c2a5c20daec05bc9bd8a2553b26365>`( \
		CLASS, \
		TYPE_NAME, \
		_VERSION_INDEX, \
		PARENT_CLASS \
		)

	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset7_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset6__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset9__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset9_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset5_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset4__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset4_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset5__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset8_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset8__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset7__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset6_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset3_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset3__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset2__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-ngraph_2opsets_2opset1__tbl_8hpp_1a7841d859ce721fbbf7366a30b542bde3>`
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset1_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_OP_REG<doxid-openvino_2opsets_2opset2_8hpp_1a336d41e89ceba6faa6edddfa03e454f6>`(a, b)
	#define :target:`_OPENVINO_RTTI_DEFINITION_SELECTOR<doxid-rtti_8hpp_1a4353cec99cde3ca385ba319f16827cf4>`(_1, _2, _3, _4, NAME, ...)
	#define :target:`_OPENVINO_RTTI_EXPAND<doxid-rtti_8hpp_1a37bffe67a08b260959c49605096aa1df>`(X)
	#define :target:`_OPENVINO_RTTI_OP_WITH_TYPE<doxid-core_2include_2openvino_2op_2op_8hpp_1a2838c7d9cf8dd411451f77f0666dad07>`(TYPE_NAME)
	#define :target:`_OPENVINO_RTTI_OP_WITH_TYPE_VERSION<doxid-core_2include_2openvino_2op_2op_8hpp_1aabc11a8c934cc1b3d42d8446e598c6cf>`(TYPE_NAME, VERSION_NAME)
	#define :target:`_OPENVINO_RTTI_WITH_TYPE<doxid-rtti_8hpp_1ab1564cffba143fdae4e832d8df8816f7>`(TYPE_NAME)
	#define :target:`_OPENVINO_RTTI_WITH_TYPE_VERSION<doxid-rtti_8hpp_1aa6e0ba5a050546a24240f08fcfa22162>`(TYPE_NAME, VERSION_NAME)

	#define :target:`_OPENVINO_RTTI_WITH_TYPE_VERSIONS_PARENT<doxid-rtti_8hpp_1a5b5e282d60197baae94137eaa983c310>`( \
		TYPE_NAME, \
		VERSION_NAME, \
		PARENT_CLASS, \
		OLD_VERSION \
		)

	#define :target:`_OPENVINO_RTTI_WITH_TYPE_VERSION_PARENT<doxid-rtti_8hpp_1ab5061880fd0ae9106d4eae47fc16a29e>`( \
		TYPE_NAME, \
		VERSION_NAME, \
		PARENT_CLASS \
		)

	#define :target:`createNodeIfRegistered<doxid-factory_8h_1a9a1f2f3a5e41d807c10af701e865b105>`(Module, key, ...)
	#define :target:`cu32<doxid-openvino_2core_2type_2bfloat16_8hpp_1ad658517d80cb8230f60d33ccb622bf97>`(x)
	#define :target:`registerNodeIfRequired<doxid-factory_8h_1aff7bf11d30c949ea501d33c39628ce07>`(Module, Name, key, Impl)
	#define :target:`strncasecmp<doxid-debug_8h_1aba00036f71bb67f8600b239a39cf5ec9>`

.. _details-global:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Macros
------

.. _doxid-ie__plugin__config_8hpp_1a7c9db10b002aa799ba6d198c61c5c743:
.. index:: pair: define; AUTO_CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define AUTO_CONFIG_KEY(name)

A macro which provides an AUTO-mangled name for configuration key with name ``name``

.. _doxid-rtti_8hpp_1a95c39aa70e3b5ce8055a31a5df9c4875:
.. index:: pair: define; BWDCMP_RTTI_DECLARATION

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define BWDCMP_RTTI_DECLARATION

Note: Please don't use this macros for new operations.

.. _doxid-cldnn__config_8hpp_1ad2e237cf3c04453361a0a6f743d0a719:
.. index:: pair: define; CLDNN_CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define CLDNN_CONFIG_KEY(name)

shortcut for defining configuration keys

.. _doxid-ie__plugin__config_8hpp_1aad09cfba062e8ec9fb7ab9383f656ec7:
.. index:: pair: define; CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define CONFIG_KEY(name)

shortcut for defining configuration keys

.. _doxid-ie__plugin__config_8hpp_1a2b1801501dc6436ffa1a9ed9c6333b40:
.. index:: pair: define; CONFIG_VALUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define CONFIG_VALUE(name)

shortcut for defining configuration values

.. _doxid-gpu__params_8hpp_1a7c86c40f2e7948bb6c5de3adc8be196c:
.. index:: pair: define; DECLARE_GPU_PARAM_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define DECLARE_GPU_PARAM_KEY(name, ...)

Shortcut for defining object parameter keys.

.. _doxid-gpu__params_8hpp_1a060c89ece9f8f5a1182dd03fdf57d5ea:
.. index:: pair: define; DECLARE_GPU_PARAM_VALUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define DECLARE_GPU_PARAM_VALUE(name)

Shortcut for defining possible values for object parameter keys.

.. _doxid-ie__layers_8h_1ad266549c8747e8451c058de008f2331e:
.. index:: pair: define; DEFINE_PROP

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define DEFINE_PROP(prop_name)

convinenent way to declare property with backward compatibility to 2D members

.. _doxid-ie__plugin__config_8hpp_1adb48efa632ae9bacfa86b8a3a0d9541e:
.. index:: pair: define; EXEC_NETWORK_METRIC_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define EXEC_NETWORK_METRIC_KEY(name)

shortcut for defining common Inference Engine ExecutableNetwork metrics

.. _doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1addbb9b81cba65edbb9156def7b9dcdfe:
.. index:: pair: define; FRONT_END_CHECK_IMPLEMENTED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FRONT_END_CHECK_IMPLEMENTED(COND, NAME)

Assert macro.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- COND

		- Condition. If 'false', throws 'NotImplementedFailure'

	*
		- NAME

		- Name of the function that is not implemented

	*
		- :ref:`ov::frontend::NotImplementedFailure <doxid-classov_1_1frontend_1_1_not_implemented_failure>`

		-

.. _doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1ae8c595f7a105bb22f095247bcb78bba4:
.. index:: pair: define; FRONT_END_GENERAL_CHECK

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FRONT_END_GENERAL_CHECK(...)

Macro to check whether a boolean condition holds.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cond

		- Condition to check

	*
		- ...

		- Additional error message info to be added to the error message via the ``<<`` stream-insertion operator. Note that the expressions here will be evaluated lazily, i.e., only if the ``cond`` evalutes to ``false``.

	*
		- :ref:`ov::frontend::GeneralFailure <doxid-classov_1_1frontend_1_1_general_failure>`

		- if ``cond`` is false.

.. _doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1aee169f84aff92500e8aba1fe3f48e7bf:
.. index:: pair: define; FRONT_END_INITIALIZATION_CHECK

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FRONT_END_INITIALIZATION_CHECK(...)

Macro to check whether a boolean condition holds.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cond

		- Condition to check

	*
		- ...

		- Additional error message info to be added to the error message via the ``<<`` stream-insertion operator. Note that the expressions here will be evaluated lazily, i.e., only if the ``cond`` evalutes to ``false``.

	*
		- :ref:`ov::frontend::InitializationFailure <doxid-classov_1_1frontend_1_1_initialization_failure>`

		- if ``cond`` is false.

.. _doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1a5e008e66e26d93062e3fa10835dfb8bc:
.. index:: pair: define; FRONT_END_NOT_IMPLEMENTED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FRONT_END_NOT_IMPLEMENTED(NAME)

Assert macro.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- NAME

		- Name of the function that is not implemented

	*
		- :ref:`ov::frontend::NotImplementedFailure <doxid-classov_1_1frontend_1_1_not_implemented_failure>`

		-

.. _doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1a80d6bce097f283d05d39913b61900c51:
.. index:: pair: define; FRONT_END_OP_CONVERSION_CHECK

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FRONT_END_OP_CONVERSION_CHECK(...)

Macro to check whether a boolean condition holds.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cond

		- Condition to check

	*
		- ...

		- Additional error message info to be added to the error message via the ``<<`` stream-insertion operator. Note that the expressions here will be evaluated lazily, i.e., only if the ``cond`` evalutes to ``false``.

	*
		- :ref:`ov::frontend::OpConversionFailure <doxid-classov_1_1frontend_1_1_op_conversion_failure>`

		- if ``cond`` is false.

.. _doxid-frontends_2common_2include_2openvino_2frontend_2exception_8hpp_1a58b0ba5a2a92e3cdb97aa0bdf68fcd5b:
.. index:: pair: define; FRONT_END_THROW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FRONT_END_THROW(MSG)

Assert macro.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- MSG

		- Error message

	*
		- :ref:`ov::frontend::GeneralFailure <doxid-classov_1_1frontend_1_1_general_failure>`

		-

.. _doxid-gna__config_8hpp_1a8124b15c4055e25f8c5792f2afe1e822:
.. index:: pair: define; GNA_CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define GNA_CONFIG_KEY(name)

Shortcut for defining configuration keys.

.. _doxid-gna__config_8hpp_1a208a60b02fdd02d379486a1625bf5ebc:
.. index:: pair: define; GNA_CONFIG_VALUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define GNA_CONFIG_VALUE(name)

Shortcut for defining configuration values.

.. _doxid-gpu__config_8hpp_1a13885ca77f3ccedfe592638155fea12f:
.. index:: pair: define; GPU_CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define GPU_CONFIG_KEY(name)

shortcut for defining configuration keys

.. _doxid-gpu__config_8hpp_1a466af595ab1b49582c27d8f6fff87b16:
.. index:: pair: define; GPU_METRIC_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define GPU_METRIC_KEY(name)

shortcut for defining GPU plugin metrics

.. _doxid-gpu__params_8hpp_1a7aedafe279f57c6fca380e3fe8538993:
.. index:: pair: define; GPU_PARAM_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define GPU_PARAM_KEY(name)

Shortcut for defining configuration keys.

.. _doxid-gpu__params_8hpp_1ae3caba30e291cdbfc5b2959b7289699b:
.. index:: pair: define; GPU_PARAM_VALUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define GPU_PARAM_VALUE(name)

Shortcut for defining configuration values.

.. _doxid-hetero__plugin__config_8hpp_1aa455ce33b7e7a245be639015625a9768:
.. index:: pair: define; HETERO_CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define HETERO_CONFIG_KEY(name)

Shortcut for defining HETERO configuration keys.

.. _doxid-ie__common_8h_1af7eb522bba9d110ae52c00dc1ef2f28a:
.. index:: pair: define; IE_ASSERT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_ASSERT(EXPRESSION)

Uses assert() function if NDEBUG is not defined, :ref:`InferenceEngine <doxid-namespace_inference_engine>` exception otherwise.

.. _doxid-ie__iextension_8h_1ad45c2c4e5155992e79925d0e2ba5138b:
.. index:: pair: define; IE_CREATE_EXTENSION

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_CREATE_EXTENSION

Defines a name of a function creating extension instance.

.. _doxid-ie__iextension_8h_1a9138b9e722336fddd0f92bad2a55d809:
.. index:: pair: define; IE_DEFINE_EXTENSION_CREATE_FUNCTION

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_DEFINE_EXTENSION_CREATE_FUNCTION(ExtensionType)

Generates extension creation function.

.. _doxid-ie__common_8h_1a2cecd150192b914ca06109942ce35c17:
.. index:: pair: define; IE_EXCEPTION_SWITCH

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_EXCEPTION_SWITCH(STATUS, TYPE_ALIAS, ...)

Generate Switch statement over error codes adn maps them to coresponding exceptions type.

.. _doxid-ie__common_8h_1a643ef2aa5e1c6b7523e55cc4396e3e02:
.. index:: pair: define; IE_THROW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_THROW(...)

A macro used to throw specified exception with a description.

.. _doxid-ie__version_8hpp_1a0a2d5226e0373446c5d8d034bbeb2e75:
.. index:: pair: define; IE_VERSION_MAJOR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_VERSION_MAJOR

Defines Inference Engine major version.

.. _doxid-ie__version_8hpp_1adfa9ccfc2f67d4d66890433e29dc7e8e:
.. index:: pair: define; IE_VERSION_MINOR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_VERSION_MINOR

Defines Inference Engine minor version.

.. _doxid-ie__version_8hpp_1a9e7a9f9e8c6b963d51bab07e89b15206:
.. index:: pair: define; IE_VERSION_PATCH

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_VERSION_PATCH

Defines Inference Engine patch version.

.. _doxid-ie__plugin__config_8hpp_1a69d0efa20c5b2bec020a706279f0c7be:
.. index:: pair: define; METRIC_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define METRIC_KEY(name)

shortcut for defining common Inference Engine metrics

.. _doxid-ie__plugin__config_8hpp_1ad6dd157c1a4d27888bfdcdf1b64cfdb2:
.. index:: pair: define; METRIC_VALUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define METRIC_VALUE(name)

shortcut for defining metric values

.. _doxid-multi__device__config_8hpp_1aa887cd604b772a3a51ba73f9652ae6c4:
.. index:: pair: define; MULTI_CONFIG_KEY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define MULTI_CONFIG_KEY(name)

A macro which provides a MULTI-mangled name for configuration key with name ``name``

.. _doxid-ngraph_2node_8hpp_1a479e20cfdaf3d59d557207ea9033f4a0:
.. index:: pair: define; NGRAPH_RTTI_DECLARATION

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define NGRAPH_RTTI_DECLARATION

Helper macro that puts necessary declarations of RTTI block inside a class definition. Should be used in the scope of class that requires type identification besides one provided by C++ RTTI. Recommended to be used for all classes that are inherited from class :ref:`ov::Node <doxid-classov_1_1_node>` to enable pattern matching for them. Accepts necessary type identification details like type of the operation, version and optional parent class.

Applying this macro within a class definition provides declaration of type_info static constant for backward compatibility with old RTTI definition for Node, static function get_type_info_static which returns a reference to an object that is equal to type_info but not necessary to the same object, and get_type_info virtual function that overrides Node::get_type_info and returns a reference to the same object that get_type_info_static gives.

Use this macro as a public part of the class definition:

.. code-block:: cpp

	class MyOp : public Node
	{
	    public:
	        // Don't use Node as a parent for type_info, it doesn't have any value and
	        prohibited
	        NGRAPH_RTTI_DECLARATION;
	
	        ...
	};
	
	class MyInheritedOp : public MyOp
	{
	    public:
	        NGRAPH_RTTI_DECLARATION;
	
	        ...
	};

To complete type identification for a class, use NGRAPH_RTTI_DEFINITION.

.. _doxid-openvino_2core_2except_8hpp_1a7ff78e5accf3159b30b4b32bbb72d272:
.. index:: pair: define; OPENVINO_ASSERT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_ASSERT(...)

Macro to check whether a boolean condition holds.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cond

		- Condition to check

	*
		- ...

		- Additional error message info to be added to the error message via the ``<<`` stream-insertion operator. Note that the expressions here will be evaluated lazily, i.e., only if the ``cond`` evalutes to ``false``.

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if ``cond`` is false.

.. _doxid-core_2include_2openvino_2core_2extension_8hpp_1acdadcfa0eff763d8b4dadb8a9cb6f6e6:
.. index:: pair: define; OPENVINO_CREATE_EXTENSIONS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_CREATE_EXTENSIONS(extensions)

Macro generates the entry point for the library.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vector

		- of extensions

.. _doxid-rtti_8hpp_1a00d4d2c156da8f59cbc4e671b0e2ff33:
.. index:: pair: define; OPENVINO_RTTI

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_RTTI(...)

Helper macro that puts necessary declarations of RTTI block inside a class definition. Should be used in the scope of class that requires type identification besides one provided by C++ RTTI. Recommended to be used for all classes that are inherited from class :ref:`ov::Node <doxid-classov_1_1_node>` to enable pattern matching for them. Accepts necessary type identification details like type of the operation, version and optional parent class.

Applying this macro within a class definition provides declaration of type_info static constant for backward compatibility with old RTTI definition for Node, static function get_type_info_static which returns a reference to an object that is equal to type_info but not necessary to the same object, and get_type_info virtual function that overrides Node::get_type_info and returns a reference to the same object that get_type_info_static gives.

Use this macro as a public part of the class definition:

.. code-block:: cpp

	class MyClass
	{
	    public:
	        OPENVINO_RTTI("MyClass", "my_version");
	
	        ...
	};
	
	class MyClass2: public MyClass
	{
	    public:
	        OPENVINO_RTTI("MyClass2", "my_version2", MyClass);
	
	        ...
	};

:ref:`OPENVINO_RTTI(name) <doxid-rtti_8hpp_1a00d4d2c156da8f59cbc4e671b0e2ff33>` :ref:`OPENVINO_RTTI(name, version_id) <doxid-rtti_8hpp_1a00d4d2c156da8f59cbc4e671b0e2ff33>` :ref:`OPENVINO_RTTI(name, version_id, parent) <doxid-rtti_8hpp_1a00d4d2c156da8f59cbc4e671b0e2ff33>` :ref:`OPENVINO_RTTI(name, version_id, parent, old_version) <doxid-rtti_8hpp_1a00d4d2c156da8f59cbc4e671b0e2ff33>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TYPE_NAME

		- a string literal of type const char\* that names your class in type identification namespace; It is your choice how to name it, but it should be unique among all OPENVINO_RTTI_DECLARATION-enabled classes that can be used in conjunction with each other in one transformation flow.

	*
		- VERSION_NAME

		- is an name of operation version to distinguish different versions of operations that shares the same TYPE_NAME

	*
		- PARENT_CLASS

		- is an optional direct or indirect parent class for this class; define it only in case if there is a need to capture any operation from some group of operations that all derived from some common base class. Don't use Node as a parent, it is a base class for all operations and doesn't provide ability to define some perfect subset of operations. PARENT_CLASS should define RTTI with OPENVINO_RTTI_{DECLARATION/DEFINITION} macros.

	*
		- _VERSION_INDEX

		- is an unsigned integer index to distinguish different versions of operations that shares the same TYPE_NAME (for backward compatibility)

.. _doxid-openvino_2core_2except_8hpp_1af19405fcee2589306ccc9288fe253b62:
.. index:: pair: define; OPENVINO_UNREACHABLE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_UNREACHABLE(...)

Macro to signal a code path that is unreachable in a successful execution. It's implemented with OPENVINO_ASSERT macro.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ...

		- Additional error message that should describe why that execution path is unreachable.

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if the macro is executed.

.. _doxid-openvino_2core_2version_8hpp_1a8cf5c3a5fcc3032007ac29e160f2b8b0:
.. index:: pair: define; OPENVINO_VERSION_MAJOR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_VERSION_MAJOR

Defines OpenVINO major version.

.. _doxid-openvino_2core_2version_8hpp_1a9886d64c4de9b93730bc318cf8437b18:
.. index:: pair: define; OPENVINO_VERSION_MINOR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_VERSION_MINOR

Defines OpenVINO minor version.

.. _doxid-openvino_2core_2version_8hpp_1ad0ff746021e0e7f76ddb964be244f29e:
.. index:: pair: define; OPENVINO_VERSION_PATCH

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OPENVINO_VERSION_PATCH

Defines OpenVINO patch version.

.. _doxid-openvino_2core_2node_8hpp_1a3fc5fb5b6a59e5bf8afcd4d1d2f8b50e:
.. index:: pair: define; TYPE_CASE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define TYPE_CASE(a)

Used in evaluator switch statement so that the case type and evaluate call are guaranteed to have the types match.

Use this in an evaluate_\*() function like this switch (arg0->get_element_type()) {:ref:`TYPE_CASE(i8) <doxid-openvino_2core_2node_8hpp_1a3fc5fb5b6a59e5bf8afcd4d1d2f8b50e>` (arg0, arg1, out, broadcast_spec); break; :ref:`TYPE_CASE(i16) <doxid-openvino_2core_2node_8hpp_1a3fc5fb5b6a59e5bf8afcd4d1d2f8b50e>` (arg0, arg1, out, broadcast_spec); break; ... }

Each TYPE_CASE statement expands like this: case element::Type_t::a: rc = evaluate<element::Type_t::a>(arg0, arg1, out, broadcast_spec)

Don't forget to put a break after each statement or it will fall through and generate a runtime error.

