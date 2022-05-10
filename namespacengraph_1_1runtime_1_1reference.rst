.. index:: pair: namespace; ngraph::runtime::reference
.. _doxid-namespacengraph_1_1runtime_1_1reference:

namespace ngraph::runtime::reference
====================================

.. toctree::
	:hidden:

	adaptive_pool <namespacengraph_1_1runtime_1_1reference_1_1adaptive_pool.rst>
	detail <namespacengraph_1_1runtime_1_1reference_1_1detail.rst>
	details <namespacengraph_1_1runtime_1_1reference_1_1details.rst>
	fake_quantize_details <namespacengraph_1_1runtime_1_1reference_1_1fake_quantize_details.rst>
	fft_common <namespacengraph_1_1runtime_1_1reference_1_1fft_common.rst>
	internal <namespacengraph_1_1runtime_1_1reference_1_1internal.rst>
	kernel <namespacengraph_1_1runtime_1_1reference_1_1kernel.rst>
	nms_common <namespacengraph_1_1runtime_1_1reference_1_1nms_common.rst>
	CellType <enumngraph_1_1runtime_1_1reference_1_1CellType.rst>
	FFTKind <enumngraph_1_1runtime_1_1reference_1_1FFTKind.rst>
	PSROIPoolingMode <enumngraph_1_1runtime_1_1reference_1_1PSROIPoolingMode.rst>
	CellArgs <structngraph_1_1runtime_1_1reference_1_1CellArgs.rst>
	convert_types <structngraph_1_1runtime_1_1reference_1_1convert_types.rst>
	widen <structngraph_1_1runtime_1_1reference_1_1widen.rst>
	GetNearestPixel <classngraph_1_1runtime_1_1reference_1_1GetNearestPixel.rst>
	GetOriginalCoordinate <classngraph_1_1runtime_1_1reference_1_1GetOriginalCoordinate.rst>
	InterpolateEval <classngraph_1_1runtime_1_1reference_1_1InterpolateEval.rst>
	InterpolateEvalHelper <classngraph_1_1runtime_1_1reference_1_1InterpolateEvalHelper.rst>
	Span <classngraph_1_1runtime_1_1reference_1_1Span.rst>
	referenceDetectionOutput <classngraph_1_1runtime_1_1reference_1_1referenceDetectionOutput.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace reference {

	// namespaces

	namespace :ref:`ngraph::runtime::reference::adaptive_pool<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool>`;
	namespace :ref:`ngraph::runtime::reference::detail<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail>`;
	namespace :ref:`ngraph::runtime::reference::details<doxid-namespacengraph_1_1runtime_1_1reference_1_1details>`;
	namespace :ref:`ngraph::runtime::reference::fake_quantize_details<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details>`;
	namespace :ref:`ngraph::runtime::reference::fft_common<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common>`;
	namespace :ref:`ngraph::runtime::reference::internal<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal>`;
	namespace :ref:`ngraph::runtime::reference::kernel<doxid-namespacengraph_1_1runtime_1_1reference_1_1kernel>`;
	namespace :ref:`ngraph::runtime::reference::nms_common<doxid-namespacengraph_1_1runtime_1_1reference_1_1nms__common>`;

	// typedefs

	typedef :ref:`ngraph::op::v4::Interpolate::NearestMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>` :target:`Nearest_mode<doxid-namespacengraph_1_1runtime_1_1reference_1ab4bffd1c61ab255095f2b61fbd9e5999>`;
	typedef :ref:`ngraph::op::v4::Interpolate::CoordinateTransformMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>` :target:`Transform_mode<doxid-namespacengraph_1_1runtime_1_1reference_1a97d69d4e87b89eeb9de73fb996337d61>`;
	typedef :ref:`ngraph::op::v4::Interpolate::InterpolateMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1a567d8870044804dc59d6d6e3df290da7>` :target:`InterpolateMode<doxid-namespacengraph_1_1runtime_1_1reference_1ad62e9140cbb1b44d6ffabc71c6f5fb31>`;
	typedef :ref:`op::v3::ROIAlign::PoolingMode<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align_1a7ef654649e9fe953a81a3cf7a30c85d7>` :target:`ROIPoolingMode<doxid-namespacengraph_1_1runtime_1_1reference_1a406e18f7f3aeb8dc54fb72035435a150>`;
	typedef :ref:`op::v9::ROIAlign::AlignedMode<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1a647f0c34a0cbfe186bb2570dcbdb7d29>` :target:`AlignedMode<doxid-namespacengraph_1_1runtime_1_1reference_1a2442cbdf57e5370f53f886d0b3300033>`;
	typedef std::function<void(const std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>&:ref:`function<doxid-namespacengraph_1_1runtime_1_1reference_1a4bbb4f04db61c605971a3eb4c1553b6e>`, const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`&inputs, :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`&outputs)> :target:`custom_evaluate_function<doxid-namespacengraph_1_1runtime_1_1reference_1ab5bca01cc5197bf9d2499b94a7a82bf9>`;

	// enums

	enum
	{
	    :target:`idxLocation<doxid-namespacengraph_1_1runtime_1_1reference_1a5e405e49a64c08cdbe3cf1419f541067a1c33305277cbe9d6552397164d68b702>`,
	    :target:`idxConfidence<doxid-namespacengraph_1_1runtime_1_1reference_1a5e405e49a64c08cdbe3cf1419f541067ad3829cad54f447af80065406fcbbb493>`,
	    :target:`idxPriors<doxid-namespacengraph_1_1runtime_1_1reference_1a5e405e49a64c08cdbe3cf1419f541067a2d045fd74198c8600a5dcaaba39634b1>`,
	    :target:`idxArmConfidence<doxid-namespacengraph_1_1runtime_1_1reference_1a5e405e49a64c08cdbe3cf1419f541067a43d87379ee0fabe4316c7c33f5cc0661>`,
	    :target:`idxArmLocation<doxid-namespacengraph_1_1runtime_1_1reference_1a5e405e49a64c08cdbe3cf1419f541067ac9ae1cc66f9491d17f03a728dbca187a>`,
	    :target:`numInputs<doxid-namespacengraph_1_1runtime_1_1reference_1a5e405e49a64c08cdbe3cf1419f541067afd8d0802f3109106a70cf0f8f18cb655>`,
	};

	enum :ref:`CellType<doxid-namespacengraph_1_1runtime_1_1reference_1af047ab7ef07c74841d7382e3798c9f96>`;
	enum :ref:`FFTKind<doxid-namespacengraph_1_1runtime_1_1reference_1afe80597983953aef3c4106099407bd20>`;
	enum :ref:`PSROIPoolingMode<doxid-namespacengraph_1_1runtime_1_1reference_1a973ee8e4d4d46aa6adfc084c06d5cb4b>`;

	// structs

	struct :ref:`CellArgs<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args>`;
	struct :ref:`convert_types<doxid-structngraph_1_1runtime_1_1reference_1_1convert__types>`;
	template <>
	struct :ref:`widen<double><doxid-structngraph_1_1runtime_1_1reference_1_1widen_3_01double_01_4>`;
	template <typename T>
	struct :ref:`widen<doxid-structngraph_1_1runtime_1_1reference_1_1widen>`;
	template <>
	struct :ref:`widen<float><doxid-structngraph_1_1runtime_1_1reference_1_1widen_3_01float_01_4>`;

	// classes

	class :ref:`GetNearestPixel<doxid-classngraph_1_1runtime_1_1reference_1_1_get_nearest_pixel>`;
	class :ref:`GetOriginalCoordinate<doxid-classngraph_1_1runtime_1_1reference_1_1_get_original_coordinate>`;
	template <typename T>
	class :ref:`InterpolateEval<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval>`;
	class :ref:`InterpolateEvalHelper<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper>`;
	template <typename Element>
	class :ref:`Span<doxid-classngraph_1_1runtime_1_1reference_1_1_span>`;
	template <typename dataType>
	class :ref:`referenceDetectionOutput<doxid-classngraph_1_1runtime_1_1reference_1_1reference_detection_output>`;

	// global variables

	const FILTER \* :target:`f<doxid-namespacengraph_1_1runtime_1_1reference_1a4582949bb0b6082a5159f90c43a71ca9>`;
	const FILTER OUTPUT \* :target:`out<doxid-namespacengraph_1_1runtime_1_1reference_1ac9d07fc6d49867bb411a4f4132777aae>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>`& :target:`in_shape<doxid-namespacengraph_1_1runtime_1_1reference_1a9ca739ccf7da267b87ff139b4ad05a17>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>`& :target:`filter_shape<doxid-namespacengraph_1_1runtime_1_1reference_1a6f612ade93d12733e1f3700872f2a31e>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>`& :target:`out_shape<doxid-namespacengraph_1_1runtime_1_1reference_1adf1cfde880ec451f975ac61a13e95485>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Strides<doxid-classov_1_1_strides>`& :target:`strides<doxid-namespacengraph_1_1runtime_1_1reference_1aeec60915d8b6c08106e358bb73f0e595>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Strides<doxid-classov_1_1_strides>` const :ref:`Strides<doxid-classov_1_1_strides>`& :target:`dilation<doxid-namespacengraph_1_1runtime_1_1reference_1a783ee1d9a10dce6061214485d9be9037>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Strides<doxid-classov_1_1_strides>` const :ref:`Strides<doxid-classov_1_1_strides>` const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& :target:`pads_begin<doxid-namespacengraph_1_1runtime_1_1reference_1aac837a6a73197557b09bd5ca4e178d44>`;
	const FILTER OUTPUT const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Shape<doxid-classov_1_1_shape>` const :ref:`Strides<doxid-classov_1_1_strides>` const :ref:`Strides<doxid-classov_1_1_strides>` const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>` const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& :target:`pads_end<doxid-namespacengraph_1_1runtime_1_1reference_1a762c0291e89375001336c0f5ea8c602c>` {     const :ref:`ngraph::CoordinateDiff<doxid-classov_1_1_coordinate_diff>` :ref:`output_padding<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1a14891dbf0955c3b6c2328c3dd7011629>`(in_shape.size() - 2, 0);
	const uint32_t :target:`crush_resistance_const_lower_value<doxid-namespacengraph_1_1runtime_1_1reference_1a1eba2ebb7bd3855afde201bfaf1fd483>` = 0x9E3779B9;
	const uint32_t :target:`crush_resistance_const_upper_value<doxid-namespacengraph_1_1runtime_1_1reference_1a84e59d57e9dd8c15a71833188d48a65f>` = 0xBB67AE85;
	const uint64_t :target:`statistic_maximizing_multiplier_n<doxid-namespacengraph_1_1runtime_1_1reference_1a2e800cabddd8c4bb4b80f6d83bffc524>` = 0xD2511F53;
	const uint64_t :target:`statistic_maximizing_multiplier_counter<doxid-namespacengraph_1_1runtime_1_1reference_1a4d161fdc8fcab2b10f9eed4fe36d0f15>` = 0xCD9E8D57;
	const size_t :target:`rounds_number<doxid-namespacengraph_1_1runtime_1_1reference_1a9eee2811fdb35434f03cb851960ec255>` = 10;
	const uint64_t :target:`skip_const<doxid-namespacengraph_1_1runtime_1_1reference_1ad46ba08c7f551fd282a0b4c4d33f0fe4>` = 256;

	// global functions

	template <
		typename T,
		typename std::enable_if<std::is_unsigned<T>::value, bool>::type = true
		>
	void :target:`abs<doxid-namespacengraph_1_1runtime_1_1reference_1af17e259120922e6ffb66ac8961a74256>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`acos<doxid-namespacengraph_1_1runtime_1_1reference_1a9810a2f0cff728999c1aca8d45a02b2b>`(const T \* arg, T \* out, size_t count);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`acosh<doxid-namespacengraph_1_1runtime_1_1reference_1ac358e0fc91e9145259095212c608fe38>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`adaptive_avg_pool<doxid-namespacengraph_1_1runtime_1_1reference_1acffdd4e750af03815513e1c5278d45d4>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape
		);

	template <typename T, typename IT>
	void :target:`adaptive_max_pool_1d<doxid-namespacengraph_1_1runtime_1_1reference_1abfeabb0836eb409180767556975ca048>`(
		const T \* arg,
		T \* out,
		IT \* indices,
		size_t h_in,
		size_t h_out
		);

	template <typename T, typename IT>
	void :target:`adaptive_max_pool_2d<doxid-namespacengraph_1_1runtime_1_1reference_1aad7b56b39f3ec723f158574110d8384a>`(
		const T \* arg,
		T \* out,
		IT \* indices,
		size_t h_in,
		size_t h_out,
		size_t w_in,
		size_t w_out
		);

	template <typename T, typename IT>
	void :target:`adaptive_max_pool_3d<doxid-namespacengraph_1_1runtime_1_1reference_1a77845d19b9ffbec8f565058ab6b60d97>`(
		const T \* arg,
		T \* out,
		IT \* indices,
		size_t d_in,
		size_t d_out,
		size_t h_in,
		size_t h_out,
		size_t w_in,
		size_t w_out
		);

	template <typename T, typename IT>
	void :target:`adaptive_max_pool<doxid-namespacengraph_1_1runtime_1_1reference_1a4a3bb49eea91132a9f8f1c63b5c85041>`(
		const T \* arg,
		T \* out,
		IT \* selected_indices,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape
		);

	template <typename T>
	void :target:`add<doxid-namespacengraph_1_1runtime_1_1reference_1a12956a756feab4106f4f12a6a372db41>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`add<doxid-namespacengraph_1_1runtime_1_1reference_1a83b76d72f78ceca76ba1a3683e972604>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`logical_and<doxid-namespacengraph_1_1runtime_1_1reference_1adce451e6facd9755747f88a9f92577eb>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`logical_and<doxid-namespacengraph_1_1runtime_1_1reference_1a83132ef08a2eac21cc07dccfbc638919>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`asin<doxid-namespacengraph_1_1runtime_1_1reference_1a1fe80c09983c8bc5cace7c8c425c5116>`(const T \* arg, T \* out, size_t count);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`asinh<doxid-namespacengraph_1_1runtime_1_1reference_1a04179b3685cf99bb0e30b5d4b07ddc3e>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`atan<doxid-namespacengraph_1_1runtime_1_1reference_1a26928b5ccc0b0e9418e7eaad39df5a39>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename X, typename Y, typename Z>
	void :target:`atan2<doxid-namespacengraph_1_1runtime_1_1reference_1a0fe523fcc10ffde40ad189c4c0acfcbb>`(
		const X \* py,
		const Y \* px,
		Z \* pout,
		size_t count
		);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`atanh<doxid-namespacengraph_1_1runtime_1_1reference_1a06841b98bc20e92993d3e44510818633>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T, typename U, typename Functor>
	void :ref:`autobroadcast_binop<doxid-namespacengraph_1_1runtime_1_1reference_1abf5e60d695b5435bb753f9ad8f22c381>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec,
		Functor elementwise_functor
		);

	template <typename T, typename U, typename Functor>
	void :ref:`autobroadcast_select<doxid-namespacengraph_1_1runtime_1_1reference_1a9e418259657aad2d9b6f8396178ca576>`(
		const U \* arg0,
		const T \* arg1,
		const T \* arg2,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg2_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec,
		Functor elementwise_functor
		);

	template <typename T>
	void :target:`avg_pool_backprop<doxid-namespacengraph_1_1runtime_1_1reference_1ac8fef8536fc82a61c499b0b561e49ad4>`(
		const T \* delta,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& delta_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& window_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_movement_strides,
		const :ref:`Shape<doxid-classov_1_1_shape>`& padding_below,
		const :ref:`Shape<doxid-classov_1_1_shape>`& padding_above,
		bool include_padding_in_avg_computation
		);

	template <typename T>
	void :target:`avg_pool<doxid-namespacengraph_1_1runtime_1_1reference_1a6adbad0e384c33bf743434da33e4a0bb>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& window_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_movement_strides,
		const :ref:`Shape<doxid-classov_1_1_shape>`& padding_below,
		const :ref:`Shape<doxid-classov_1_1_shape>`& padding_above,
		bool include_padding_in_avg_computation
		);

	template <typename T>
	static T :target:`norm<doxid-namespacengraph_1_1runtime_1_1reference_1a245cd52a8980cf5851b581a332965999>`(T val, T mean, T var, T eps);

	template <typename T>
	void :target:`batch_norm_inference<doxid-namespacengraph_1_1runtime_1_1reference_1ac0a25694c5a9439a48bee5fc1cc8e507>`(
		float eps,
		const T \* in,
		const T \* gamma,
		const T \* beta,
		const T \* mean,
		const T \* variance,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape
		);

	template <typename T_IN, typename T_F>
	void :target:`binary_convolution<doxid-namespacengraph_1_1runtime_1_1reference_1ab76ef320e6ec43958fb0cf9e3a104107>`(
		const T_IN \* in,
		const T_F \* f,
		T_IN \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const float pad_value
		);

	void :target:`broadcast<doxid-namespacengraph_1_1runtime_1_1reference_1a394e1bb9bf3dc1264efa531e91d81470>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& broadcast_axes,
		size_t elem_size
		);

	template <typename T, typename B, typename P>
	void :target:`bucketize<doxid-namespacengraph_1_1runtime_1_1reference_1ab3d8501de75e34542c8c2c99bf1715e8>`(
		const T \* data,
		const B \* buckets,
		P \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& buckets_shape,
		bool with_right_bound
		);

	template <typename T>
	void :target:`ceiling<doxid-namespacengraph_1_1runtime_1_1reference_1aca711fd6db3cf61327049f17713251c1>`(const T \* arg, T \* out, size_t count);

	template <typename T>
	void :target:`clamp<doxid-namespacengraph_1_1runtime_1_1reference_1a31ab0f627c4457fc7f527087cb5dd35f>`(
		const T \* arg,
		T \* out,
		T min,
		T max,
		size_t count
		);

	void :target:`concat<doxid-namespacengraph_1_1runtime_1_1reference_1a697183f9ae579acade2cb21c5ebad1ca>`(
		const std::vector<const char \*>& args,
		char \* out,
		const std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>& in_shapes,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		int64_t concatenation_axis,
		size_t elem_size
		);

	template <typename T>
	void :target:`constant<doxid-namespacengraph_1_1runtime_1_1reference_1a987f73089cb01d178940b8fc314cebd7>`(const T \* arg0, T \* out, size_t count);

	template <typename TI, typename TO>
	std::enable_if<!std::is_same<TO, char>::value>::type :target:`convert<doxid-namespacengraph_1_1runtime_1_1reference_1a47c51966524a20fa5df43fba5e61f419>`(
		const TI \* arg,
		TO \* out,
		size_t count
		);

	void :target:`convert< uint8_t, float16 ><doxid-namespacengraph_1_1runtime_1_1reference_1a3523c1c7653493a0685d08049d6db07d>`(const uint8_t \* arg, :ref:`float16<doxid-classov_1_1float16>` \* out, size_t count);
	void :target:`convert< float16, float ><doxid-namespacengraph_1_1runtime_1_1reference_1a1aa9b963b02a35343b0edca301a31424>`(const :ref:`float16<doxid-classov_1_1float16>` \* arg, float \* out, size_t count);
	void :target:`convert< float, int8_t ><doxid-namespacengraph_1_1runtime_1_1reference_1a5f177bf69bad60b465022541ba385d89>`(const float \* arg, int8_t \* out, size_t count);
	void :target:`convert< float16, int8_t ><doxid-namespacengraph_1_1runtime_1_1reference_1aa6104238db572cb505c289886f750c4f>`(const :ref:`float16<doxid-classov_1_1float16>` \* arg, int8_t \* out, size_t count);

	template <typename TI, typename TO>
	std::enable_if<std::is_same<TO, char>::value>::type :target:`convert<doxid-namespacengraph_1_1runtime_1_1reference_1a16d703264fd46de639b4622f3077550e>`(
		const TI \* arg,
		TO \* out,
		size_t count
		);

	template <typename T>
	std::tuple<T, T, T> :target:`yuv_pixel_to_rgb<doxid-namespacengraph_1_1runtime_1_1reference_1a831a637eca17ebf1389af8b52915b108>`(
		float y_val,
		float u_val,
		float v_val
		);

	template <typename T>
	void :target:`color_convert_nv12<doxid-namespacengraph_1_1runtime_1_1reference_1a7e1063f308607c464ee8dcf63bc6d78d>`(
		const T \* arg_y,
		const T \* arg_uv,
		T \* out_ptr,
		size_t batch_size,
		size_t image_h,
		size_t image_w,
		size_t stride_y,
		size_t stride_uv,
		:ref:`ov::op::util::ConvertColorNV12Base::ColorConversion<doxid-classov_1_1op_1_1util_1_1_convert_color_n_v12_base_1afbdb3631faab232fb42d01ff83c5573b>` color_format
		);

	template <typename T>
	void :target:`color_convert_i420<doxid-namespacengraph_1_1runtime_1_1reference_1a8ce5e6069afb68d851c752fc7b7090aa>`(
		const T \* arg_y,
		const T \* arg_u,
		const T \* arg_v,
		T \* out_ptr,
		size_t batch_size,
		size_t image_h,
		size_t image_w,
		size_t stride_y,
		size_t stride_uv,
		:ref:`ov::op::util::ConvertColorI420Base::ColorConversion<doxid-classov_1_1op_1_1util_1_1_convert_color_i420_base_1a203405069101c4fe7f82e5f0d326788f>` color_format
		);

	template <ov::element::Type_t ET>
	bool :target:`color_convert_nv12<doxid-namespacengraph_1_1runtime_1_1reference_1a74af436bd54795a1ef939836188c5252>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& op,
		const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& outputs,
		const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& inputs,
		:ref:`ov::op::util::ConvertColorNV12Base::ColorConversion<doxid-classov_1_1op_1_1util_1_1_convert_color_n_v12_base_1afbdb3631faab232fb42d01ff83c5573b>` type
		);

	template <ov::element::Type_t ET>
	bool :target:`color_convert_i420<doxid-namespacengraph_1_1runtime_1_1reference_1a2100eed16421cf65a92072fbd4f2ba5b>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& op,
		const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& outputs,
		const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& inputs,
		:ref:`ov::op::util::ConvertColorI420Base::ColorConversion<doxid-classov_1_1op_1_1util_1_1_convert_color_i420_base_1a203405069101c4fe7f82e5f0d326788f>` type
		);

	template <typename T>
	void :target:`convolution<doxid-namespacengraph_1_1runtime_1_1reference_1a285ae18e24d1c3c3dc9186367f529319>`(
		const T \* in,
		const T \* f,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	template <typename T>
	void :target:`convolution_backprop_in<doxid-namespacengraph_1_1runtime_1_1reference_1a80634fff9d4a75ae9e4cb3db63081137>`(
		const T \* delta_in,
		const T \* filter,
		T \* delta_out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filter_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& in_dilation,
		const :ref:`Strides<doxid-classov_1_1_strides>`& filter_dilation,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& forward_in_pad_bellow,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& forward_in_pad_above,
		const :ref:`Strides<doxid-classov_1_1_strides>`& stride,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& output_padding
		);

	template <typename T>
	void :target:`copy<doxid-namespacengraph_1_1runtime_1_1reference_1ae9e111c1aee5932340d30ef5bcb9886c>`(const T \* arg, T \* out, size_t count);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`cos<doxid-namespacengraph_1_1runtime_1_1reference_1a10a27da6cfe17b88bc42d507744e44db>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`cosh<doxid-namespacengraph_1_1runtime_1_1reference_1a88d67354daeb6f5065d420d6793f7669>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`ctc_greedy_decoder<doxid-namespacengraph_1_1runtime_1_1reference_1a10328be39fc08bd46a054921ac23df9c>`(
		const T \* data,
		const T \* sequence_masks,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& sequence_masks_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const bool ctc_merge_repeated
		);

	template <typename TF, typename TI, typename TCI, typename TSL>
	void :target:`ctc_greedy_decoder_seq_len<doxid-namespacengraph_1_1runtime_1_1reference_1a91c522919ea54ea5f1e04327990f8a4d>`(
		const TF \* data,
		const TI \* sequence_length,
		const TI \* blank_index,
		TCI \* out1,
		TSL \* out2,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const bool ctc_merge_repeated
		);

	template <typename T, typename U>
	void :target:`CTCLoss<doxid-namespacengraph_1_1runtime_1_1reference_1a08182db7eb83464e7597df9bdba60731>`(
		const T \* logits,
		const :ref:`Shape<doxid-classov_1_1_shape>`& logitsShape,
		const U \* logitsLength,
		const U \* labels,
		const U \* labelsLength,
		const U \* blankIndexP,
		const bool preprocessCollapseRepeated,
		const bool ctcMergeRepeated,
		const bool unique,
		T \* output
		);

	template <typename T, typename P>
	void :target:`cumsum<doxid-namespacengraph_1_1runtime_1_1reference_1a996b5e62a1254eea725814727328e3ad>`(
		const T \* arg,
		const P \* axis_tensor,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& tensor_shape,
		const bool exclusive,
		const bool reverse
		);

	template <typename T>
	void :target:`deformable_convolution<doxid-namespacengraph_1_1runtime_1_1reference_1aaa07170c725d8735accb9ff2f9e35859>`(
		const T \* in,
		const T \* offsets,
		const T \* filters,
		const T \* mask,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& o_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& m_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilation,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const int64_t groups,
		const int64_t deformable_groups,
		const bool bilinear_interpolation_pad
		);

	template <typename T>
	void :target:`deformable_convolution<doxid-namespacengraph_1_1runtime_1_1reference_1a2dfcae51dc4b001f24d7a8918416829c>`(
		const T \* in,
		const T \* offsets,
		const T \* filters,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& o_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilation,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const int64_t groups,
		const int64_t deformable_groups,
		const bool bilinear_interpolation_pad = false
		);

	template <typename T>
	void :target:`deformable_psroi_pooling<doxid-namespacengraph_1_1runtime_1_1reference_1a141fd7a13e4f69b95d717ef33f52c5c6>`(
		const T \* data_input,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_input_shape,
		const T \* rois_input,
		const :ref:`Shape<doxid-classov_1_1_shape>`& rois_input_shape,
		const T \* offsets_input,
		const :ref:`Shape<doxid-classov_1_1_shape>`& offsets_input_shape,
		T \* output,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const std::string& mode_str,
		const float spatial_scale,
		const int64_t spatial_bins_x,
		const int64_t spatial_bins_y,
		const float trans_std,
		const int64_t part_size
		);

	void :target:`depth_to_space<doxid-namespacengraph_1_1runtime_1_1reference_1a094267379a32181a2a239d79828e187d>`(
		const char \*const in,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		char \*const out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const size_t block_size,
		const :ref:`op::DepthToSpace::DepthToSpaceMode<doxid-classov_1_1op_1_1v0_1_1_depth_to_space_1adf46d7cb205c4a8b94bafa9d4c34c303>` mode,
		const size_t elem_size
		);

	template <typename T>
	std::enable_if<std::is_integral<T>::value>::type :target:`divide<doxid-namespacengraph_1_1runtime_1_1reference_1abbf500e2f95da145f18163900745b28c>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count,
		bool pythondiv
		);

	template <typename T>
	std::enable_if<std::is_integral<T>::value>::type :target:`divide<doxid-namespacengraph_1_1runtime_1_1reference_1a9f32610e6eaba4dc9e9fa90b958db332>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec,
		bool pythondiv
		);

	template <typename T>
	std::enable_if<std::is_floating_point<T>::value||std::is_same<T, :ref:`bfloat16<doxid-classov_1_1bfloat16>`>::value||std::is_same<T, :ref:`float16<doxid-classov_1_1float16>`>::value>::type :target:`divide<doxid-namespacengraph_1_1runtime_1_1reference_1aeee89956b89b166001ab4584bf430a8c>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count,
		bool pythondiv
		);

	template <typename T>
	std::enable_if<std::is_floating_point<T>::value||std::is_same<T, :ref:`bfloat16<doxid-classov_1_1bfloat16>`>::value||std::is_same<T, :ref:`float16<doxid-classov_1_1float16>`>::value>::type :target:`divide<doxid-namespacengraph_1_1runtime_1_1reference_1afefc2a24913bf05f446ab73396662246>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec,
		bool pythondiv
		);

	void :target:`einsum<doxid-namespacengraph_1_1runtime_1_1reference_1a1c3591e83db2049920c6a6537cad5de9>`(
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& outputs,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& inputs,
		const std::string& equation
		);

	template <typename T>
	void :target:`elu<doxid-namespacengraph_1_1runtime_1_1reference_1a6662f3fef1b3d0c40756f16d7fe54f3e>`(
		const T \* arg,
		T \* out,
		size_t count,
		double alpha
		);

	template <typename T, typename U>
	void :target:`embeddingBagOffsetsSum<doxid-namespacengraph_1_1runtime_1_1reference_1a5d116a1b38aba1098d083368c570979b>`(
		const T \* emb_table,
		const U \* indices,
		const U \* offsets,
		const U \* default_index,
		const T \* weights,
		T \* out,
		const size_t indices_count,
		const :ref:`Shape<doxid-classov_1_1_shape>`& outShape
		);

	template <typename T, typename U>
	void :target:`embeddingBagPackedSum<doxid-namespacengraph_1_1runtime_1_1reference_1adedf5dea93a95b13728a2c5ac39d7e57>`(
		const T \* emb_table,
		const U \* indices,
		const T \* weights,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indicesShape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& outShape
		);

	template <typename T, typename U>
	void :target:`embeddingSegmentsSum<doxid-namespacengraph_1_1runtime_1_1reference_1ab25de243414a25bd0f3eb8d019383b08>`(
		const T \* embTable,
		const U \* indices,
		const U \* segmentIds,
		const U \* defaultIndex,
		const T \* weights,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& embTableShape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indicesShape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& outShape
		);

	template <typename T>
	void :target:`equal<doxid-namespacengraph_1_1runtime_1_1reference_1aa1f787df30e32ca1f09be4e35e2ecdc6>`(
		const T \* arg0,
		const T \* arg1,
		char \* out,
		size_t count
		);

	template <typename T, typename U>
	void :target:`equal<doxid-namespacengraph_1_1runtime_1_1reference_1abb0b8406297dafddd08106705460c2a9>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`erf<doxid-namespacengraph_1_1runtime_1_1reference_1a7378a9569067e94325bb72761998de3e>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`exp<doxid-namespacengraph_1_1runtime_1_1reference_1afa908f53fa8f5cd5dd5617e37fe7da6e>`(const T \* arg, T \* out, size_t count);

	void :target:`experimental_detectron_detection_output<doxid-namespacengraph_1_1runtime_1_1reference_1aa468036d4ed79c1b32495d967b51863f>`(
		const float \* input_rois,
		const float \* input_deltas,
		const float \* input_scores,
		const float \* input_im_info,
		const :ref:`op::v6::ExperimentalDetectronDetectionOutput::Attributes<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes>`& attrs,
		float \* output_boxes,
		float \* output_scores,
		int32_t \* output_classes
		);

	void :target:`experimental_detectron_detection_output_postprocessing<doxid-namespacengraph_1_1runtime_1_1reference_1a58897fe82920af0db9a42d6df860ca96>`(
		void \* pboxes,
		void \* pclasses,
		void \* pscores,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` output_type,
		const std::vector<float>& output_boxes,
		const std::vector<int32_t>& output_classes,
		const std::vector<float>& output_scores,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_boxes_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_classes_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_scores_shape
		);

	template <typename T>
	void :target:`experimental_detectron_prior_grid_generator<doxid-namespacengraph_1_1runtime_1_1reference_1a870545432907042136adb5a60afe8a6f>`(
		const T \* priors,
		const :ref:`Shape<doxid-classov_1_1_shape>`& priors_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& feature_map_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& im_data_shape,
		T \* output_rois,
		int64_t grid_h,
		int64_t grid_w,
		float stride_h,
		float stride_w
		);

	void :target:`experimental_detectron_proposals_single_image<doxid-namespacengraph_1_1runtime_1_1reference_1a31498cbea8c25d42721b1fc7d89493ce>`(
		const float \* im_info,
		const float \* anchors,
		const float \* deltas,
		const float \* scores,
		const :ref:`op::v6::ExperimentalDetectronGenerateProposalsSingleImage::Attributes<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_generate_proposals_single_image_1_1_attributes>`& attrs,
		const :ref:`Shape<doxid-classov_1_1_shape>`& im_info_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& anchors_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& deltas_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& scores_shape,
		float \* output_rois,
		float \* output_scores
		);

	void :target:`experimental_detectron_proposals_single_image_postprocessing<doxid-namespacengraph_1_1runtime_1_1reference_1af7e092a314363b3637b55cfe8b2d09da>`(
		void \* prois,
		void \* pscores,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` output_type,
		const std::vector<float>& output_rois,
		const std::vector<float>& output_scores,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_rois_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_scores_shape
		);

	void :target:`experimental_detectron_roi_feature_extractor<doxid-namespacengraph_1_1runtime_1_1reference_1ad903d51d02e6fc7f67dfc911448cb448>`(
		const std::vector<std::vector<float>>& inputs,
		const std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>& input_shapes,
		const :ref:`op::v6::ExperimentalDetectronROIFeatureExtractor::Attributes<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_r_o_i_feature_extractor_1_1_attributes>`& attrs,
		float \* output_rois_features,
		float \* output_rois
		);

	void :target:`experimental_detectron_roi_feature_extractor_postprocessing<doxid-namespacengraph_1_1runtime_1_1reference_1af1d5c28a961c566a47cc3046ad87ee0a>`(
		void \* prois_features,
		void \* prois,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` output_type,
		const std::vector<float>& output_roi_features,
		const std::vector<float>& output_rois,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_roi_features_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_rois_shape
		);

	template <typename T>
	void :target:`experimental_detectron_topk_rois<doxid-namespacengraph_1_1runtime_1_1reference_1abcd67ded9f44faf9bf9366a84e813d37>`(
		const T \* input_rois,
		const T \* input_probs,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_rois_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_probs_shape,
		size_t max_rois,
		T \* output_rois
		);

	template <typename T>
	void :target:`extract_image_patches<doxid-namespacengraph_1_1runtime_1_1reference_1ae186c3d922b4d4dec4d3d940338a8d1a>`(
		const std::shared_ptr<:ref:`op::ExtractImagePatches<doxid-classov_1_1op_1_1v3_1_1_extract_image_patches>`> extImgPatches,
		const T \* input,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& inShape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& outShape
		);

	template <typename T>
	void :target:`fake_quantize<doxid-namespacengraph_1_1runtime_1_1reference_1a39643d239af64a9b765a58e165d5d864>`(
		const T \*const arg,
		const T \*const in_low,
		const T \*const in_high,
		const T \*const out_low,
		const T \*const out_high,
		T \*const out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_low_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_high_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_low_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_high_shape,
		size_t levels,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast
		);

	void :target:`fft<doxid-namespacengraph_1_1runtime_1_1reference_1ad7ea5bcb1304f4cc5bf080b7ff692cb4>`(
		const float \* input_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
		const int64_t \* axes_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& axes_data_shape,
		float \* fft_result,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		:ref:`FFTKind<doxid-namespacengraph_1_1runtime_1_1reference_1afe80597983953aef3c4106099407bd20>` fft_kind
		);

	void :target:`fft_postprocessing<doxid-namespacengraph_1_1runtime_1_1reference_1a169d56f3827fd31fbd9435781b418f81>`(
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& outputs,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` output_type,
		const std::vector<float>& fft_result
		);

	std::vector<int64_t> :target:`canonicalize_axes<doxid-namespacengraph_1_1runtime_1_1reference_1a62ff619e856a7d07ddb2879e4a844d33>`(
		const int64_t \* axes_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& axes_data_shape,
		int64_t complex_data_rank
		);

	template <typename T>
	void :target:`floor<doxid-namespacengraph_1_1runtime_1_1reference_1a8e3635833ce953454fb37544c30dfcd1>`(const T \* arg, T \* out, size_t count);

	template <typename T>
	void :target:`floor_mod<doxid-namespacengraph_1_1runtime_1_1reference_1a3cd1a546fd1b18be9493aa43bc349b19>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	void :target:`function<doxid-namespacengraph_1_1runtime_1_1reference_1a4bbb4f04db61c605971a3eb4c1553b6e>`(
		const std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& function,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& inputs,
		:ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& outputs
		);

	template <typename T, typename U>
	void :target:`gather<doxid-namespacengraph_1_1runtime_1_1reference_1a4e3b7e6f24c9b436fe8ab08be1521d06>`(
		const T \*const data,
		const U \*const indices,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		size_t axis,
		size_t batch_dims = 0
		);

	template <typename T, typename U>
	void :target:`gather_elements<doxid-namespacengraph_1_1runtime_1_1reference_1a1f1284529d9a65b8607693fe3147b8f3>`(
		const T \* data,
		const U \* indices,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		int64_t axis
		);

	template <typename T, typename U>
	void :ref:`gather_nd<doxid-namespacengraph_1_1runtime_1_1reference_1ae82f73a16cf2f13da1d9c246a95ddb6e>`(
		const T \*const params,
		const U \*const indices,
		T \*const out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& params_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const int batch_dims = 0
		);

	void :target:`gather_tree<doxid-namespacengraph_1_1runtime_1_1reference_1ae3d147ff67d673e9074bb0aa698be1c2>`(
		const char \* step_ids,
		const char \* parent_ids,
		const char \* max_seq_len,
		const char \* end_token,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& step_ids_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& parent_ids_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& max_seq_len_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& end_token_shape,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type
		);

	template <typename T>
	void :target:`gelu<doxid-namespacengraph_1_1runtime_1_1reference_1ad77702e7cf97aa16b1cfc2e6d1791aeb>`(
		const T \* arg,
		T \* out,
		op::GeluApproximationMode mode,
		size_t count
		);

	template <typename T>
	void :target:`greater<doxid-namespacengraph_1_1runtime_1_1reference_1a57392ae82f5b22607d69470afd59139a>`(
		const T \* arg0,
		const T \* arg1,
		char \* out,
		size_t count
		);

	template <typename T, typename U>
	void :target:`greater<doxid-namespacengraph_1_1runtime_1_1reference_1a61a779299ef2ae4e418079a93fe8ed81>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`greater_eq<doxid-namespacengraph_1_1runtime_1_1reference_1a6a3ba9ed3828cb959b86c2efcabc140b>`(
		const T \* arg0,
		const T \* arg1,
		char \* out,
		size_t count
		);

	template <typename T, typename U>
	void :target:`greater_eq<doxid-namespacengraph_1_1runtime_1_1reference_1af39194f2119e97c3263f400e719cdb5f>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`grn<doxid-namespacengraph_1_1runtime_1_1reference_1a159c34e8004bfe15a9b2f849c7cbc1a0>`(
		const T \* data,
		T \* out,
		float bias,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape
		);

	void :target:`validate_group_convolution_parameters<doxid-namespacengraph_1_1runtime_1_1reference_1aa3e9197727c6871d4725d1c6dffbeec4>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	template <
		typename INPUT,
		typename FILTER,
		typename OUTPUT,
		typename ACCU = typename widen<OUTPUT>::type
		>
	void :target:`group_convolution<doxid-namespacengraph_1_1runtime_1_1reference_1aa340bc553561bff602330b921cb8a441>`(
		const INPUT \* in,
		const FILTER \* f,
		OUTPUT \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filter_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilation,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	void :target:`infer_backward_conv_output_shape<doxid-namespacengraph_1_1runtime_1_1reference_1a45b036b5f205aa21c075c12e99a279e5>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_spatial_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_spatial_shape,
		:ref:`Shape<doxid-classov_1_1_shape>`& out_spatial_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	void :target:`validate_convolution_backprop_data_parameters<doxid-namespacengraph_1_1runtime_1_1reference_1a008bfb9b23544934108444c835469309>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	void :target:`validate_group_convolution_backprop_data_parameters<doxid-namespacengraph_1_1runtime_1_1reference_1a0950b73d2de5627fbcc854b5a0050bf0>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& f_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	template <typename T>
	void :target:`group_convolution_backprop_data<doxid-namespacengraph_1_1runtime_1_1reference_1a3467daccce5992cd513974f945064f5b>`(
		const T \* in,
		const T \* f,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filter_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilation,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& output_padding
		);

	template <
		typename OUTPUT,
		typename FILTER,
		typename INPUT,
		typename ACCUMULATION = typename widen<INPUT>::type
		>
	:target:`NGRAPH_DEPRECATED<doxid-namespacengraph_1_1runtime_1_1reference_1afcbc55207e8e2b56784a087d0a068798>`(
		"group_convolution_backprop_data :ref:`function<doxid-namespacengraph_1_1runtime_1_1reference_1a4bbb4f04db61c605971a3eb4c1553b6e>` without output_paddings is deprecated,
		" "use the one with output_padding."
		) const;

	:target:`group_convolution_backprop_data<doxid-namespacengraph_1_1runtime_1_1reference_1a5b067f353cc802c445b42d6419aff2dc>`(
		in,
		:ref:`f<doxid-namespacengraph_1_1runtime_1_1reference_1a4582949bb0b6082a5159f90c43a71ca9>`,
		:ref:`out<doxid-namespacengraph_1_1runtime_1_1reference_1ac9d07fc6d49867bb411a4f4132777aae>`,
		:ref:`in_shape<doxid-namespacengraph_1_1runtime_1_1reference_1a9ca739ccf7da267b87ff139b4ad05a17>`,
		:ref:`filter_shape<doxid-namespacengraph_1_1runtime_1_1reference_1a6f612ade93d12733e1f3700872f2a31e>`,
		:ref:`out_shape<doxid-namespacengraph_1_1runtime_1_1reference_1adf1cfde880ec451f975ac61a13e95485>`,
		:ref:`strides<doxid-namespacengraph_1_1runtime_1_1reference_1aeec60915d8b6c08106e358bb73f0e595>`,
		:ref:`dilation<doxid-namespacengraph_1_1runtime_1_1reference_1a783ee1d9a10dce6061214485d9be9037>`,
		:ref:`pads_begin<doxid-namespacengraph_1_1runtime_1_1reference_1aac837a6a73197557b09bd5ca4e178d44>`,
		:ref:`pads_end<doxid-namespacengraph_1_1runtime_1_1reference_1a762c0291e89375001336c0f5ea8c602c>`,
		:ref:`output_padding<doxid-core_2reference_2include_2ngraph_2runtime_2reference_2convolution_8hpp_1a14891dbf0955c3b6c2328c3dd7011629>`
		);

	template <typename T>
	void :target:`gru_cell<doxid-namespacengraph_1_1runtime_1_1reference_1a923cebe7aad87ffa5a6e47fe63fa5129>`(
		const T \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const T \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const T \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const T \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const T \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		T \* dst_data,
		const std::string& activation_f,
		const std::string& activation_g,
		float clip,
		bool linear_before_reset
		);

	template <typename T>
	void :target:`hard_sigmoid<doxid-namespacengraph_1_1runtime_1_1reference_1afa846a8fb51bc6a7e14d6741423262c2>`(
		const T \* arg,
		const T alpha,
		const T beta,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`hsigmoid<doxid-namespacengraph_1_1runtime_1_1reference_1a31c35f86052e25fd05080a17637d358d>`(const T \* arg, T \* out, size_t count);

	template <typename T>
	void :target:`hswish<doxid-namespacengraph_1_1runtime_1_1reference_1a4424d35bee30ad56b652cd622f515f73>`(const T \* arg, T \* out, size_t count);

	void :target:`if_reference<doxid-namespacengraph_1_1runtime_1_1reference_1a7da6efd9a2a6cc69a162794d582512f7>`(
		const std::vector<std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>>& body,
		const std::vector<:ref:`op::util::MultiSubgraphOutputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1aac4ca5b6b097bff1f0ee58648ab3f0e5>`>& out_descs,
		const std::vector<:ref:`op::util::MultiSubgraphInputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a3d048c2d9f6ca65f578ac3029a0a330e>`>& input_descs,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& out,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& args
		);

	static void :target:`pad_input_data<doxid-namespacengraph_1_1runtime_1_1reference_1a03e4271421b9e2a92e0c27e33b645358>`(
		const uint8_t \* data_ptr,
		uint8_t \* padded_data_ptr,
		size_t type_size,
		const :ref:`ov::Shape<doxid-classov_1_1_shape>`& input_shape,
		const :ref:`ov::Shape<doxid-classov_1_1_shape>`& padded_input_shape,
		const std::vector<size_t>& pads_begin
		);

	static :ref:`PartialShape<doxid-classov_1_1_partial_shape>` :target:`get_padded_input_shape<doxid-namespacengraph_1_1runtime_1_1reference_1ad0c556b3dceab0a8410138915aaeed79>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		const :ref:`op::v0::Interpolate::Attributes<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes>`& attrs
		);

	static std::vector<float> :target:`get_scales<doxid-namespacengraph_1_1runtime_1_1reference_1a160dc2090814ee9de3c59588a4755e21>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_data_partial_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`op::v0::Interpolate::Attributes<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes>`& attrs
		);

	static :ref:`op::v4::Interpolate::InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs>` :target:`transform_v0_to_v4<doxid-namespacengraph_1_1runtime_1_1reference_1a67cce1a3af31905205b95840c11c4762>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_partial_shape,
		const :ref:`op::v0::Interpolate::Attributes<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes>`& attrs_v0
		);

	template <typename T>
	void :target:`interpolate<doxid-namespacengraph_1_1runtime_1_1reference_1a3a4fa97a675582b5eef566c0edb5f08f>`(
		const T \* input_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
		const std::vector<float>& scales,
		const std::vector<int64_t>& axes,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`op::v4::Interpolate::InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs>`& attrs
		);

	template <typename T>
	void :target:`interpolate<doxid-namespacengraph_1_1runtime_1_1reference_1a2916d8e8ea722fe65c5992e4561dbaf0>`(
		T \* input_data,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_data_shape,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`op::v0::Interpolate::Attributes<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes>`& attrs
		);

	template <typename T>
	void :target:`less<doxid-namespacengraph_1_1runtime_1_1reference_1a5ccaffa59016865a1c2eeaea132eed3a>`(
		const T \* arg0,
		const T \* arg1,
		char \* out,
		size_t count
		);

	template <typename T, typename U>
	void :target:`less<doxid-namespacengraph_1_1runtime_1_1reference_1a34ba10c0b73f53b0d8e277575577a2b3>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`less_eq<doxid-namespacengraph_1_1runtime_1_1reference_1a8dd821ec86338973a2987574eea90f1d>`(
		const T \* arg0,
		const T \* arg1,
		char \* out,
		size_t count
		);

	template <typename T, typename U>
	void :target:`less_eq<doxid-namespacengraph_1_1runtime_1_1reference_1a48ebd36368e5255f9e65ac7af612e576>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`log<doxid-namespacengraph_1_1runtime_1_1reference_1aa6c97bab9e6ec996a491e2f07bba3d23>`(const T \* arg, T \* out, size_t count);

	template <typename T>
	void :target:`log_softmax<doxid-namespacengraph_1_1runtime_1_1reference_1a1062fada6301ec175b6504d6eb7657ec>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& axes
		);

	static void :target:`reduce_logical_and<doxid-namespacengraph_1_1runtime_1_1reference_1ae0c4c62ff433e036ef87986e7dfb20e9>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	static void :target:`reduce_logical_or<doxid-namespacengraph_1_1runtime_1_1reference_1afe9294f5f19f381a5d58d0deeba59145>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	void :target:`loop<doxid-namespacengraph_1_1runtime_1_1reference_1a3986332122a83dd995b32974a298c41d>`(
		const std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& body,
		const :ref:`op::util::OutputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a3235964d87a00ce23118b395dc3a7e31>`& out_descs,
		const :ref:`op::util::InputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a6f702135e7f8b7a71b2d071ac52f5c0c>`& input_descs,
		const opset5::Loop::SpecialBodyPorts& special_ports,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& out,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& args
		);

	static size_t :target:`point_to_flat_idx<doxid-namespacengraph_1_1runtime_1_1reference_1a1820782a6866515194dab5c039d2c77e>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const std::vector<size_t>& point
		);

	static std::vector<size_t> :target:`slice_indices<doxid-namespacengraph_1_1runtime_1_1reference_1a664de06de7be631e5d056c0c0fb81a0c>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& full_shape,
		const std::vector<size_t>& begin,
		const :ref:`Shape<doxid-classov_1_1_shape>`& slice_shape
		);

	template <typename T>
	static T :target:`sum_region_across_axes<doxid-namespacengraph_1_1runtime_1_1reference_1ae483d9465f67ad3158f2348838233697>`(
		const T \* arg,
		const std::vector<size_t>& indices
		);

	template <typename T>
	void :target:`lrn<doxid-namespacengraph_1_1runtime_1_1reference_1a3592d9546d826dc219d747d2b5c4d160>`(
		const T \* arg,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& axes,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		double dalpha,
		double dbeta,
		double dbias,
		size_t size
		);

	template <typename T>
	void :target:`lstm_cell<doxid-namespacengraph_1_1runtime_1_1reference_1a40912cf09f96febfb39967b013dfff6c>`(
		const T \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const T \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const T \* C,
		const :ref:`Shape<doxid-classov_1_1_shape>`& C_shape,
		const T \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const T \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const T \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		T \* out_Ht,
		T \* out_Ct,
		const std::string& activation_f,
		const std::string& activation_g,
		const std::string& activation_h,
		float clip
		);

	template <typename T>
	void :target:`lstm_cell_v1<doxid-namespacengraph_1_1runtime_1_1reference_1a656f990e030c5a9a2ae19d26aad6c07d>`(
		const T \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const T \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const T \* C,
		const :ref:`Shape<doxid-classov_1_1_shape>`& C_shape,
		const T \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const T \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const T \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		const T \* P,
		const :ref:`Shape<doxid-classov_1_1_shape>`& P_shape,
		T \* out_Ht,
		T \* out_Ct,
		const std::string& activation_f,
		const std::string& activation_g,
		const std::string& activation_h,
		float clip,
		const :ref:`ov::op::LSTMWeightsFormat<doxid-namespaceov_1_1op_1a6efe5db5f325a937a6662cd2b66e1437>` weight_format,
		bool input_forget
		);

	template <typename T>
	void :ref:`matmul<doxid-namespacengraph_1_1runtime_1_1reference_1a5cc77214b0225a1310443bebed605745>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		bool transpose_arg0,
		bool transpose_arg1
		);

	void :target:`matrix_nms<doxid-namespacengraph_1_1runtime_1_1reference_1a537bd52ddf3eaf270bdd7216b6312823>`(
		const float \* boxes_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& boxes_data_shape,
		const float \* scores_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& scores_data_shape,
		const :ref:`op::v8::MatrixNms::Attributes<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes>`& attrs,
		float \* selected_outputs,
		const :ref:`Shape<doxid-classov_1_1_shape>`& selected_outputs_shape,
		int64_t \* selected_indices,
		const :ref:`Shape<doxid-classov_1_1_shape>`& selected_indices_shape,
		int64_t \* valid_outputs
		);

	template <typename T>
	void :target:`max<doxid-namespacengraph_1_1runtime_1_1reference_1a92cfabd79e866544fb35d44884e7adfd>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	template <typename T>
	void :target:`max_pool<doxid-namespacengraph_1_1runtime_1_1reference_1a2384002ffb1b180155f58e312bcc429d>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& window_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& window_movement_strides,
		const :ref:`Shape<doxid-classov_1_1_shape>`& padding_below,
		const :ref:`Shape<doxid-classov_1_1_shape>`& padding_above
		);

	template <typename Values_t, typename Indices_t>
	void :target:`max_pool<doxid-namespacengraph_1_1runtime_1_1reference_1a556e2fbc69774844c80fb87848218e10>`(
		const Values_t \* data,
		Values_t \* values,
		Indices_t \* indices,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& kernel,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`Shape<doxid-classov_1_1_shape>`& pads_begin,
		const :ref:`Shape<doxid-classov_1_1_shape>`& pads_end,
		const int64_t axis = 0
		);

	template <typename T>
	void :target:`maximum<doxid-namespacengraph_1_1runtime_1_1reference_1a2c3e6a3b447beeb17efb281542ba3ef2>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`maximum<doxid-namespacengraph_1_1runtime_1_1reference_1aeaf514f53baa7c3b556b73236fd2c957>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`mean<doxid-namespacengraph_1_1runtime_1_1reference_1a052f6098c0d40d15f23664bdc241000a>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	template <typename T>
	void :target:`min<doxid-namespacengraph_1_1runtime_1_1reference_1abc42885cb896b121ab5ac214cbf60935>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	template <typename T>
	void :target:`minimum<doxid-namespacengraph_1_1runtime_1_1reference_1a2bf29f71dbf3918dbf2f66762b5c45df>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`minimum<doxid-namespacengraph_1_1runtime_1_1reference_1a1824c438e6b0f490a8389d9133ed0c58>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`mish<doxid-namespacengraph_1_1runtime_1_1reference_1a9746be5fd62081ad7014125ef92faf83>`(const T \* arg, T \* out, size_t count);

	template <typename T>
	void :target:`mod<doxid-namespacengraph_1_1runtime_1_1reference_1a49c5fce66d220bb55f62984dce847ff4>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape0,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape1,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	void :target:`multiclass_nms<doxid-namespacengraph_1_1runtime_1_1reference_1a2ca9aad4eebdd939f31d20155777349a>`(
		const float \* boxes_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& boxes_data_shape,
		const float \* scores_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& scores_data_shape,
		const :ref:`op::v8::MulticlassNms::Attributes<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes>`& attrs,
		float \* selected_outputs,
		const :ref:`Shape<doxid-classov_1_1_shape>`& selected_outputs_shape,
		int64_t \* selected_indices,
		const :ref:`Shape<doxid-classov_1_1_shape>`& selected_indices_shape,
		int64_t \* valid_outputs
		);

	template <typename T>
	void :target:`multiply<doxid-namespacengraph_1_1runtime_1_1reference_1a00292cb933b4e80075ebb7c6fcd77719>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`multiply<doxid-namespacengraph_1_1runtime_1_1reference_1a44be11757e17c2bd0c895d577e5664d2>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`mvn<doxid-namespacengraph_1_1runtime_1_1reference_1a91beda4c6af95c159de1536490593fd4>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const bool normalize_variance,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes,
		const double eps
		);

	template <typename T>
	void :target:`mvn_6<doxid-namespacengraph_1_1runtime_1_1reference_1aac9819fb1f1d8462f8f8367570f37bb9>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		:ref:`AxisSet<doxid-classov_1_1_axis_set>` reduction_axes,
		bool normalize_variance,
		double eps,
		op::MVNEpsMode eps_mode
		);

	template <typename T>
	void :target:`negate<doxid-namespacengraph_1_1runtime_1_1reference_1a5281544c3e88bbc5c8949e7e9e29f703>`(const T \* arg, T \* out, size_t count);

	void :target:`non_max_suppression<doxid-namespacengraph_1_1runtime_1_1reference_1aacac8c4f6ef7e2d0dfac27f6e924651e>`(
		const float \* boxes_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& boxes_data_shape,
		const float \* scores_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& scores_data_shape,
		int64_t max_output_boxes_per_class,
		float iou_threshold,
		float score_threshold,
		float soft_nms_sigma,
		int64_t \* selected_indices,
		const :ref:`Shape<doxid-classov_1_1_shape>`& selected_indices_shape,
		float \* selected_scores,
		const :ref:`Shape<doxid-classov_1_1_shape>`& selected_scores_shape,
		int64_t \* valid_outputs,
		const bool sort_result_descending
		);

	void :target:`nms5_postprocessing<doxid-namespacengraph_1_1runtime_1_1reference_1a9db9fb0fd7d30a9fd5de79b1e9e88ac1>`(
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& outputs,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` output_type,
		const std::vector<int64_t>& selected_indices,
		const std::vector<float>& selected_scores,
		int64_t valid_outputs,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` selected_scores_type
		);

	template <typename T>
	size_t :ref:`non_zero_get_count<doxid-namespacengraph_1_1runtime_1_1reference_1a0538c05c674d21392cb54dccc5210b31>`(
		const T \* arg,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape
		);

	template <typename T, typename U>
	void :ref:`non_zero<doxid-namespacengraph_1_1runtime_1_1reference_1a9d9749498c328d9503fa0be68768268a>`(
		const T \* arg,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape
		);

	template <typename T>
	void :target:`normalize_l2<doxid-namespacengraph_1_1runtime_1_1reference_1ae27dd27d2a3607a124809cdb96ca21d8>`(
		const T \* data,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes,
		float eps,
		op::EpsMode eps_mode
		);

	template <typename T>
	void :target:`logical_not<doxid-namespacengraph_1_1runtime_1_1reference_1a37fcfeed08766bf51913659b64d4c0e7>`(const T \* arg, T \* out, size_t count);

	template <typename T, typename U>
	void :target:`not_equal<doxid-namespacengraph_1_1runtime_1_1reference_1abed20eca1abf17d246410ecb7c6cb4e9>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename INPUT_TYPE>
	void :target:`one_hot<doxid-namespacengraph_1_1runtime_1_1reference_1af6d44422248692caf10ad9ac7ef876a9>`(
		const INPUT_TYPE \* indices,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape,
		char \* out,
		const size_t out_elem_size,
		const size_t depth,
		const int64_t one_hot_axis,
		const char \* on_value,
		const char \* off_value
		);

	template <typename T>
	void :target:`logical_or<doxid-namespacengraph_1_1runtime_1_1reference_1a2379eae47b2d08cdc4180dc8f26c017d>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`logical_or<doxid-namespacengraph_1_1runtime_1_1reference_1ae5289b70e281447a2e0fe73a7a2cc758>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	void :target:`pad<doxid-namespacengraph_1_1runtime_1_1reference_1ae641bb8113fe10ad72673fffc63fcaa4>`(
		const char \* data,
		const char \* pad_value,
		char \* out,
		const size_t elem_size,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& padding_below,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& padding_above,
		const op::PadMode pad_mode
		);

	template <typename T>
	void :target:`power<doxid-namespacengraph_1_1runtime_1_1reference_1a633fc85061e6939c4a44a68bfe439402>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`power<doxid-namespacengraph_1_1runtime_1_1reference_1a3a2931aa61c4c3d726622ca19ced5ed6>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`prelu<doxid-namespacengraph_1_1runtime_1_1reference_1a5a7b11f21d07606494830dfc1e282766>`(
		const T \* arg,
		const T \* slope,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& slope_shape
		);

	static float :target:`clip_great<doxid-namespacengraph_1_1runtime_1_1reference_1a4c865bd3a093faa8fd139160b06e0954>`(float x, float threshold);
	static float :target:`clip_less<doxid-namespacengraph_1_1runtime_1_1reference_1a5803848adaf4c002823e5644fe455789>`(float x, float threshold);

	template <typename T>
	void :target:`prior_box<doxid-namespacengraph_1_1runtime_1_1reference_1ad761261a2f1a73ec6895d9cd2bf97ff2>`(
		const T \* data,
		const T \* img,
		float \* dst_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`op::v8::PriorBox::Attributes<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes>`& attrs
		);

	template <typename T>
	void :target:`prior_box_clustered<doxid-namespacengraph_1_1runtime_1_1reference_1a20e7d89c7249fcb27c171f2d0b47cb53>`(
		const T \* data,
		const T \* img,
		float \* dst_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`op::PriorBoxClusteredAttrs<doxid-namespacengraph_1_1op_1aace968ed86791f8a1fdd72ca869c5ae0>`& attrs
		);

	template <typename T>
	void :target:`product<doxid-namespacengraph_1_1runtime_1_1reference_1adeab9b7f60a3f1f46bf497ef9c038c51>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	template <typename T>
	void :target:`proposal_v0<doxid-namespacengraph_1_1runtime_1_1reference_1a27afd4b4ab52c373a0600290f0e4b115>`(
		const T \* class_probs,
		const T \* bbox_deltas,
		const T \* image_shape,
		T \* output,
		const :ref:`Shape<doxid-classov_1_1_shape>`& class_probs_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& bbox_deltas_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& image_shape_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`op::ProposalAttrs<doxid-namespacengraph_1_1op_1a4358e1e5587270d7e246c6a9c90b1c51>`& attrs
		);

	template <typename T>
	void :target:`proposal_v4<doxid-namespacengraph_1_1runtime_1_1reference_1ab1efe8f8b111909f34101c8c2568b6be>`(
		const T \* class_probs,
		const T \* bbox_deltas,
		const T \* image_shape,
		T \* output,
		T \* out_probs,
		const :ref:`Shape<doxid-classov_1_1_shape>`& class_probs_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& bbox_deltas_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& image_shape_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_probs_shape,
		const :ref:`op::ProposalAttrs<doxid-namespacengraph_1_1op_1a4358e1e5587270d7e246c6a9c90b1c51>`& attrs
		);

	template <typename T>
	void :target:`psroi_pooling<doxid-namespacengraph_1_1runtime_1_1reference_1aa9ee4fe8d95b070f53bf8768c335fd3b>`(
		const T \* input,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		const T \* rois,
		const :ref:`Shape<doxid-classov_1_1_shape>`& rois_shape,
		T \* output,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const std::string& mode_str,
		float spatial_scale,
		int spatial_bins_x,
		int spatial_bins_y
		);

	template <typename REAL, typename QUANT>
	void :target:`quantize<doxid-namespacengraph_1_1runtime_1_1reference_1acadf7b4bd0710de3185cdcaf67ea9c9a>`(
		const REAL \* input,
		const REAL \* scale,
		const QUANT \* zero_point,
		QUANT \* output,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& scale_zero_point_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& axes,
		op::Quantize::RoundMode round_mode
		);

	std::pair<uint64_t, uint64_t> :target:`random_uniform<doxid-namespacengraph_1_1runtime_1_1reference_1af331f36c1408331912ffda9a305e4be5>`(
		const uint64_t \* out_shape,
		const char \* min_val,
		const char \* max_val,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape_shape,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`& elem_type,
		uint64_t seed,
		uint64_t seed2,
		std::pair<uint64_t, uint64_t> prev_state
		);

	template <typename T>
	std::enable_if<std::is_floating_point<T>::value||std::is_same<T, :ref:`bfloat16<doxid-classov_1_1bfloat16>`>::value||std::is_same<T, :ref:`float16<doxid-classov_1_1float16>`>::value>::type :target:`range<doxid-namespacengraph_1_1runtime_1_1reference_1a6e7a7da51225b5333900d059a6f386d3>`(
		const T \* start,
		const T \* step,
		const size_t& num_elem,
		T \* out
		);

	template <typename T>
	std::enable_if<std::is_integral<T>::value>::type :target:`range<doxid-namespacengraph_1_1runtime_1_1reference_1ad4febc283556b72366456bf31e0236ac>`(
		const T \* start,
		const T \* step,
		const size_t& num_elem,
		T \* out
		);

	void :target:`rdft<doxid-namespacengraph_1_1runtime_1_1reference_1aa89b574a8bedb27ee5d81ba5b67615d0>`(
		const std::vector<float>& input_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
		const std::vector<int64_t>& axes_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_fft_shape,
		float \* rdft_result
		);

	template <typename T>
	void :target:`reduce_l1<doxid-namespacengraph_1_1runtime_1_1reference_1a02d3281ad10c9ed9f6874956e3434306>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	template <typename T>
	void :target:`reduce_l2<doxid-namespacengraph_1_1runtime_1_1reference_1a0ccff95b1e425654f3b038f6c5655f0e>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	static int :target:`entry_index<doxid-namespacengraph_1_1runtime_1_1reference_1af00c37a6983e654002ee8784f0999177>`(
		int width,
		int height,
		int coords,
		int classes,
		int outputs,
		int batch,
		int location,
		int entry
		);

	template <typename T>
	static T :target:`sigmoid<doxid-namespacengraph_1_1runtime_1_1reference_1acb9e761b9f5b112d968f24c1cc38db58>`(float x);

	template <typename T>
	static void :target:`softmax_generic<doxid-namespacengraph_1_1runtime_1_1reference_1a788404051a1c10514c3b3b106314079c>`(
		const T \* src_data,
		T \* dst_data,
		int batches,
		int channels,
		int height,
		int width
		);

	template <typename T>
	void :target:`region_yolo<doxid-namespacengraph_1_1runtime_1_1reference_1a21b08088593585bb963b412e8f8df6e5>`(
		const T \* input,
		T \* output,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		const int coords,
		const int classes,
		const int regions,
		const bool do_softmax,
		const std::vector<int64_t>& mask
		);

	template <typename T>
	void :target:`relu<doxid-namespacengraph_1_1runtime_1_1reference_1a6d15632328f9a877f5347965b51f7afd>`(const T \* arg, T \* out, size_t count);

	void :target:`reorg_yolo<doxid-namespacengraph_1_1runtime_1_1reference_1af9822398745401245e7ecc08d366e647>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		int64_t stride,
		const size_t elem_size
		);

	void :target:`reshape<doxid-namespacengraph_1_1runtime_1_1reference_1a562b3868f63d206713b890f5c52493c3>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisVector<doxid-classov_1_1_axis_vector>`& in_axis_order,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		size_t elem_size
		);

	template <typename T>
	void :target:`result<doxid-namespacengraph_1_1runtime_1_1reference_1a9f63c4359f72e8f64b3d6ff4883447f0>`(const T \* arg, T \* out, size_t count);

	void :target:`reverse<doxid-namespacengraph_1_1runtime_1_1reference_1a53ffda07aed6f53ffdc102f1d59676b9>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reversed_axes,
		size_t elem_size
		);

	template <typename T, typename U>
	void :target:`reverse_sequence<doxid-namespacengraph_1_1runtime_1_1reference_1a262bb8652c02658283c4ea62aafc4387>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		size_t batch_axis,
		size_t sequence_axis,
		const U \* sequence_lengths
		);

	template <typename T>
	void :target:`rnn_cell<doxid-namespacengraph_1_1runtime_1_1reference_1a75c3e91b175fe5e0ba075dfcab418f1b>`(
		const T \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const T \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const T \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const T \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const T \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		T \* dst_data,
		const std::string& activation_f,
		float clip
		);

	template <typename T>
	void :target:`roi_align<doxid-namespacengraph_1_1runtime_1_1reference_1ae0f96a0b3fc17161312b5faa651e8bfb>`(
		const T \* feature_maps,
		const T \* rois,
		const int64_t \* batch_indices,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& feature_maps_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& rois_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& batch_indices_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const int pooled_height,
		const int pooled_width,
		const int sampling_ratio,
		const float spatial_scale,
		const :ref:`ROIPoolingMode<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align_1a7ef654649e9fe953a81a3cf7a30c85d7>`& pooling_mode,
		const :ref:`AlignedMode<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1a647f0c34a0cbfe186bb2570dcbdb7d29>`& aligned_mode = :ref:`AlignedMode::ASYMMETRIC<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1a647f0c34a0cbfe186bb2570dcbdb7d29ad4cb95b2d550c20b06f46e10d4c7c7b2>`
		);

	template <typename T>
	void :target:`roi_pooling<doxid-namespacengraph_1_1runtime_1_1reference_1a4b48daa664b743f6973e07757aaaf883>`(
		const T \* feature_maps,
		const T \* rois,
		T \* output,
		const :ref:`Shape<doxid-classov_1_1_shape>`& feature_maps_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& rois_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const float spatial_scale,
		const std::string& pooling_method
		);

	size_t :target:`shift_pos<doxid-namespacengraph_1_1runtime_1_1reference_1ace53e7288f10f9efe20752bce0d6c622>`(
		size_t pos_in_spanned_data,
		size_t dim_shift,
		size_t spanned_shape_size,
		size_t dim_size
		);

	void :target:`roll<doxid-namespacengraph_1_1runtime_1_1reference_1a993a90201af76ef30eab728666faca0d>`(
		const char \* arg,
		const int64_t \* shift,
		const int64_t \* axes,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shift_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& axes_shape,
		size_t elem_size
		);

	template <typename T>
	T :target:`round_to_nearest_even<doxid-namespacengraph_1_1runtime_1_1reference_1a64cfc5348b0bd6b8a0ff2f8551cf0ab6>`(const T arg);

	template <typename T>
	void :target:`round<doxid-namespacengraph_1_1runtime_1_1reference_1a8ea383ca6ce01d26eabe1c27a0e1bd37>`(
		const T \* arg,
		T \* out,
		size_t count,
		const :ref:`op::v5::Round::RoundMode<doxid-classov_1_1op_1_1v5_1_1_round_1a25a2039a1e12e5aa8e612cb5bb82af7e>` mode
		);

	template <typename DataType, typename IndicesType>
	void :target:`scatter_elem_update<doxid-namespacengraph_1_1runtime_1_1reference_1aee6f15859b402077d5099fc94e7f1462>`(
		const DataType \* input_data,
		const IndicesType \* indices,
		const DataType \* updates,
		const int64_t& axis,
		DataType \* out_buf,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape
		);

	template <typename dataType, typename indicesType>
	void :target:`scatterNdUpdate<doxid-namespacengraph_1_1runtime_1_1reference_1ae9d49e95988ab27dc2d8851ca7dcd810>`(
		const dataType \*const inputData,
		const indicesType \*const indices,
		const dataType \*const updates,
		dataType \*const outBuf,
		const :ref:`Shape<doxid-classov_1_1_shape>`& dataShape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indicesShape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& updatesShape
		);

	static const CoordinateTransformBasic :target:`get_target_shape<doxid-namespacengraph_1_1runtime_1_1reference_1ad8a2b184d219ccdd8b357771c2427f09>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& start_corner,
		const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& end_corner
		);

	static void :target:`scatter_update<doxid-namespacengraph_1_1runtime_1_1reference_1a91f238b5ed44972cc267c8ca4e17d002>`(
		const char \* input_data,
		const int64_t \* indices,
		const char \* updates,
		const int64_t axis,
		char \* out_buf,
		const size_t elem_size,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& updates_shape
		);

	template <typename T>
	void :target:`select<doxid-namespacengraph_1_1runtime_1_1reference_1ac4457574fc3a2d28675eef979fbfc8ee>`(
		const char \* arg0,
		const T \* arg1,
		const T \* arg2,
		T \* out,
		size_t arg0_count,
		size_t arg1_count,
		size_t arg2_count,
		size_t out_count
		);

	template <typename T>
	void :target:`select<doxid-namespacengraph_1_1runtime_1_1reference_1abfd23c068026b8b067037724d332d180>`(
		const char \* arg0,
		const T \* arg1,
		const T \* arg2,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg2_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`selu<doxid-namespacengraph_1_1runtime_1_1reference_1aac53f98d477508faea3d6af161204e3a>`(
		const T \* arg,
		const T \* alpha,
		const T \* lambda,
		T \* out,
		size_t size_arg,
		size_t size_alpha,
		size_t size_lambda
		);

	template <typename T, typename U>
	void :target:`cell_pass<doxid-namespacengraph_1_1runtime_1_1reference_1a9b412e86d4cf202aee60b36d27e5c7b1>`(
		:ref:`CellType<doxid-namespacengraph_1_1runtime_1_1reference_1af047ab7ef07c74841d7382e3798c9f96>` type,
		const std::vector<const char \*>& inputs,
		const std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>& shapes,
		const std::vector<char \*>& outputs,
		const :ref:`CellArgs<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args>`& args,
		bool is_reverse
		);

	template <typename T, typename U>
	void :target:`lstm_sequence<doxid-namespacengraph_1_1runtime_1_1reference_1ada0b3609882d709487d5603fba2b0a56>`(
		const char \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const char \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const char \* C,
		const :ref:`Shape<doxid-classov_1_1_shape>`& C_shape,
		const char \* seq_lengths,
		const :ref:`Shape<doxid-classov_1_1_shape>`& seq_lengths_shape,
		const char \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const char \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const char \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		char \* Y,
		char \* Ho,
		char \* Co,
		const std::string& activation_f,
		const std::string& activation_g,
		const std::string& activation_h,
		float clip,
		op::RecurrentSequenceDirection direction
		);

	template <typename T, typename U>
	void :target:`lstm_sequence_v1<doxid-namespacengraph_1_1runtime_1_1reference_1a23e3b2e8b01147f92d1c56cf17a51ac2>`(
		const char \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const char \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const char \* C,
		const :ref:`Shape<doxid-classov_1_1_shape>`& C_shape,
		const char \* seq_lengths,
		const :ref:`Shape<doxid-classov_1_1_shape>`& seq_lengths_shape,
		const char \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const char \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const char \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		const char \* P,
		const :ref:`Shape<doxid-classov_1_1_shape>`& P_shape,
		char \* Y,
		char \* Ho,
		char \* Co,
		const std::string& activation_f,
		const std::string& activation_g,
		const std::string& activation_h,
		float clip,
		const :ref:`ov::op::LSTMWeightsFormat<doxid-namespaceov_1_1op_1a6efe5db5f325a937a6662cd2b66e1437>` weight_format,
		bool input_forget,
		op::RecurrentSequenceDirection direction
		);

	template <typename T, typename U>
	void :target:`gru_sequence<doxid-namespacengraph_1_1runtime_1_1reference_1a02bd7e9a3ced51844d3c4c4c15bb6aa1>`(
		const char \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const char \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const char \* seq_lengths,
		const :ref:`Shape<doxid-classov_1_1_shape>`& seq_lengths_shape,
		const char \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const char \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const char \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		char \* Y,
		char \* Ho,
		const std::string& activation_f,
		const std::string& activation_g,
		const float clip,
		const op::RecurrentSequenceDirection direction,
		const bool linear_before_reset
		);

	template <typename T, typename U>
	void :target:`rnn_sequence<doxid-namespacengraph_1_1runtime_1_1reference_1a887a24a559fd89c9d5bebddc4911e088>`(
		const char \* X,
		const :ref:`Shape<doxid-classov_1_1_shape>`& X_shape,
		const char \* H,
		const :ref:`Shape<doxid-classov_1_1_shape>`& H_shape,
		const char \* seq_lengths,
		const :ref:`Shape<doxid-classov_1_1_shape>`& seq_lengths_shape,
		const char \* W,
		const :ref:`Shape<doxid-classov_1_1_shape>`& W_shape,
		const char \* R,
		const :ref:`Shape<doxid-classov_1_1_shape>`& R_shape,
		const char \* B,
		const :ref:`Shape<doxid-classov_1_1_shape>`& B_shape,
		char \* Y,
		char \* Ho,
		const std::string& activation_f,
		float clip,
		const op::RecurrentSequenceDirection direction
		);

	template <typename T>
	void :target:`shape_of<doxid-namespacengraph_1_1runtime_1_1reference_1abc9c373cb486c59179385206c7fb4540>`(const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape, T \* out);

	void :target:`shuffle_channels<doxid-namespacengraph_1_1runtime_1_1reference_1a57865af803e62af3298216dacd5eddec>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		size_t elem_size,
		const int64_t axis,
		const int64_t group
		);

	template <
		typename T,
		typename std::enable_if<std::is_integral<T>::value, bool>::type = true
		>
	void :target:`sigmoid<doxid-namespacengraph_1_1runtime_1_1reference_1afa8b3f6853e1228300e920f7ddd39586>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`sign<doxid-namespacengraph_1_1runtime_1_1reference_1a4c4990d199f8a4f4123903b21c39ee4b>`(const T \* arg, T \* out, size_t count);

	template <typename T>
	void :target:`sin<doxid-namespacengraph_1_1runtime_1_1reference_1a8efe909a0942ffd807b78c51230cb193>`(const T \* arg, T \* out, size_t count);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`sinh<doxid-namespacengraph_1_1runtime_1_1reference_1a6bdd88a1680932090b8642def3f611d7>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	void :target:`slice<doxid-namespacengraph_1_1runtime_1_1reference_1ac778a8f07fd5641d844ef24566670f52>`(
		const char \* data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		size_t elem_size,
		const std::vector<int64_t>& starts,
		const std::vector<int64_t>& steps,
		const std::vector<int64_t>& axes
		);

	void :target:`slice<doxid-namespacengraph_1_1runtime_1_1reference_1a8823945e56a8640506c0e6394140a14d>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& lower_bounds,
		const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& upper_bounds,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		size_t elem_size
		);

	template <typename T>
	void :target:`softmax<doxid-namespacengraph_1_1runtime_1_1reference_1aae91b564b3c2a2d081ef153cb21d0314>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& axes
		);

	template <typename T>
	void :target:`softplus<doxid-namespacengraph_1_1runtime_1_1reference_1a57ec0c977ab04866081c431c28eb1c72>`(const T \* arg, T \* out, size_t count);

	void :target:`space_to_depth<doxid-namespacengraph_1_1runtime_1_1reference_1abfc1c7665b2406c31daf8aa5e8c027d5>`(
		const char \*const in,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		char \*const out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const size_t block_size,
		const :ref:`op::SpaceToDepth::SpaceToDepthMode<doxid-classov_1_1op_1_1v0_1_1_space_to_depth_1ad6b782e0cfede20e971e2ff658d80957>` mode,
		const size_t elem_size
		);

	void :target:`split<doxid-namespacengraph_1_1runtime_1_1reference_1a5c11f30b804a436e822eedffccf01a2c>`(
		const char \* data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		size_t elem_size,
		int64_t axis,
		size_t num_splits,
		char \*\* out_data
		);

	template <typename T>
	std::enable_if<!std::is_integral<T>::value>::type :target:`sqrt<doxid-namespacengraph_1_1runtime_1_1reference_1a521b22f55daef69723c6e28d8f153f81>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	std::enable_if<std::is_integral<T>::value>::type :target:`sqrt<doxid-namespacengraph_1_1runtime_1_1reference_1a97187846f1c854b825840b78bcedda98>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`squared_difference<doxid-namespacengraph_1_1runtime_1_1reference_1a536ed64c4b56b8d4ba7b7e0ca14884dc>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	void :target:`strided_slice<doxid-namespacengraph_1_1runtime_1_1reference_1aa5b1c0cbb5d1ea2f48d519ed56c63206>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
		const SlicePlan& sp,
		size_t elem_type
		);

	template <typename T>
	void :target:`subtract<doxid-namespacengraph_1_1runtime_1_1reference_1a959e51636697fd1830dacd2a811ab6da>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`subtract<doxid-namespacengraph_1_1runtime_1_1reference_1aca6750728bb8acfc05fcda994e09502b>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	template <typename T>
	void :target:`sum<doxid-namespacengraph_1_1runtime_1_1reference_1a64755dfcf1508858b9908cfa8342c337>`(
		const T \* arg,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes
		);

	template <typename T>
	void :target:`swish<doxid-namespacengraph_1_1runtime_1_1reference_1a8e08b0c47db6d3ef7714d48e0d330c98>`(
		const T \* arg,
		const T \* beta,
		T \* out,
		size_t count
		);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`tan<doxid-namespacengraph_1_1runtime_1_1reference_1aeb75479962466bbf57b726ea60df9574>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	template <
		typename T,
		typename std::enable_if<!std::is_integral<T>::value, bool>::type = true
		>
	void :target:`tanh<doxid-namespacengraph_1_1runtime_1_1reference_1a4dab02901ed1fc0c1130059ad6020b72>`(
		const T \* arg,
		T \* out,
		size_t count
		);

	void :target:`tensor_iterator<doxid-namespacengraph_1_1runtime_1_1reference_1a2ae7a39178b9c4d892f0527c77f42ac3>`(
		uint64_t num_iterations,
		const std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& body,
		const :ref:`op::util::OutputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a3235964d87a00ce23118b395dc3a7e31>`& out_descs,
		const :ref:`op::util::InputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a6f702135e7f8b7a71b2d071ac52f5c0c>`& input_descs,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& out,
		const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& args,
		const :ref:`custom_evaluate_function<doxid-namespacengraph_1_1runtime_1_1reference_1ab5bca01cc5197bf9d2499b94a7a82bf9>`& evaluate = nullptr
		);

	void :target:`tile<doxid-namespacengraph_1_1runtime_1_1reference_1a00a7a3027e07f1e469fc2c1998b8688a>`(
		const char \* arg,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const size_t elem_size,
		const std::vector<int64_t>& repeats
		);

	template <typename T, typename U>
	bool :target:`compare_max<doxid-namespacengraph_1_1runtime_1_1reference_1ae6de8d251987daff14d247080189017d>`(
		const std::tuple<T, U>& a,
		const std::tuple<T, U>& b
		);

	template <typename T, typename U>
	bool :target:`compare_min<doxid-namespacengraph_1_1runtime_1_1reference_1a78ee7e1de8bdee6a34cc806f1ef42f31>`(
		const std::tuple<T, U>& a,
		const std::tuple<T, U>& b
		);

	template <typename T, typename U>
	bool :target:`sort_indices_ascending<doxid-namespacengraph_1_1runtime_1_1reference_1aade565fd0f3f8fe82dc2ae27e537dd79>`(
		const std::tuple<T, U>& a,
		const std::tuple<T, U>& b
		);

	template <typename T, typename U>
	void :target:`topk<doxid-namespacengraph_1_1runtime_1_1reference_1a5b96904945f6ce911a84316f9ccd25fc>`(
		const T \* arg,
		U \* out_indices,
		T \* out_values,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		size_t axis,
		size_t k,
		bool compute_max,
		:ref:`op::v1::TopK::SortType<doxid-namespaceov_1_1op_1adb25710a58c013466ba8b371156e09cb>` sort = :ref:`op::v1::TopK::SortType::NONE<doxid-namespaceov_1_1op_1adb25710a58c013466ba8b371156e09cbab50339a10e1de285ac99d4c3990b8693>`
		);

	void :target:`transpose<doxid-namespacengraph_1_1runtime_1_1reference_1afd1f146ba7b68379c2fc4c0f4ec05fbb>`(
		const char \* data,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& data_shape,
		size_t element_size,
		const int64_t \* axes_order,
		:ref:`Shape<doxid-classov_1_1_shape>` out_shape
		);

	template <
		typename Iterator,
		typename value = typename details::from_iterator<Iterator>::stored_value,
		details::Required<details::IsRandomAccessIt<Iterator>::value> = true
		>
	constexpr auto :target:`span<doxid-namespacengraph_1_1runtime_1_1reference_1ae62c5f8959ddb4e771baa7bfac3c4705>`(
		Iterator first,
		Iterator second
		);

	template <
		typename Container,
		typename = details::void_t<decltype(std::declval<Container>().data()), decltype(std::declval<Container>().size())>
		>
	constexpr auto :target:`span<doxid-namespacengraph_1_1runtime_1_1reference_1a1790726016a6f0e4f74d26b83e2eb60f>`(const Container& c);

	template <
		typename Container,
		typename = details::void_t<decltype(std::declval<Container>().data()), decltype(std::declval<Container>().size())>
		>
	constexpr auto :target:`span<doxid-namespacengraph_1_1runtime_1_1reference_1a5cb9880fabb2ab49c1b1d1b222cab86d>`(Container& c);

	template <typename Element>
	constexpr auto :target:`span<doxid-namespacengraph_1_1runtime_1_1reference_1a4ce4ca597e831cbd231da387ee97ffe9>`(
		const Element \* data,
		std::size_t size
		);

	template <typename Element>
	constexpr auto :target:`span<doxid-namespacengraph_1_1runtime_1_1reference_1a077221fd3bf412bb2c14b3d47f146f2f>`(
		Element \* data,
		std::size_t size
		);

	template <typename T>
	void :target:`logical_xor<doxid-namespacengraph_1_1runtime_1_1reference_1a2c92a7b41326abb881f02d84b33c29c0>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		size_t count
		);

	template <typename T>
	void :target:`logical_xor<doxid-namespacengraph_1_1runtime_1_1reference_1a292d5e88213c8b9bcb2b866ccc742de9>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
		);

	} // namespace reference
.. _details-namespacengraph_1_1runtime_1_1reference:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespacengraph_1_1runtime_1_1reference_1abf5e60d695b5435bb753f9ad8f22c381:
.. index:: pair: function; autobroadcast_binop

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename U, typename Functor>
	void autobroadcast_binop(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec,
		Functor elementwise_functor
		)

Helper function to implement autobroadcasting elementwise binop references.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Element type of the input tensors.

	*
		- U

		- Element type of the output tensor.

	*
		- Functor

		- Type of the functor for the elementwise operation. Must support operator()(T,T), and operator()(T,T) must return a value of type U.

	*
		- arg0

		- Pointer to the buffer for left operand input tensor.

	*
		- arg1

		- Pointer to the buffer for right operand input tensor.

	*
		- out

		- Pointer to the buffer for output tensor. This must be pre-allocated by the caller, and must be large enough to hold a tensor of the correct shape.

	*
		- broadcast_spec

		- Specification of the auto-broadcasting scheme.

	*
		- elementwise_functor

		- Functor implementing the elementwise operation to be applied across the input tensors. Must accept two arguments of type T, and return a value of type U.

.. _doxid-namespacengraph_1_1runtime_1_1reference_1a9e418259657aad2d9b6f8396178ca576:
.. index:: pair: function; autobroadcast_select

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename U, typename Functor>
	void autobroadcast_select(
		const U \* arg0,
		const T \* arg1,
		const T \* arg2,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg2_shape,
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec,
		Functor elementwise_functor
		)

Helper function to implement autobroadcasting elementwise ternaryop references.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- U

		- Element type of the selector tensor.

	*
		- T

		- Element type of the input tensors.

	*
		- Functor

		- Type of the functor for the elementwise operation. Must support operator()(U,T,T), and operator()(U,T,T) must return a value of type T.

	*
		- arg0

		- Pointer to the buffer for selector tensor.

	*
		- arg1

		- Pointer to the buffer for left operand input tensor.

	*
		- arg2

		- Pointer to the buffer for right operand input tensor.

	*
		- out

		- Pointer to the buffer for output tensor. This must be pre-allocated by the caller, and must be large enough to hold a tensor of the correct shape.

	*
		- broadcast_spec

		- Specification of the auto-broadcasting scheme.

	*
		- elementwise_functor

		- Functor implementing the elementwise operation to be applied across the input tensors. Must accept an argument of type U and two of type T, and return a value of type T.

.. _doxid-namespacengraph_1_1runtime_1_1reference_1ae82f73a16cf2f13da1d9c246a95ddb6e:
.. index:: pair: function; gather_nd

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename U>
	void gather_nd(
		const T \*const params,
		const U \*const indices,
		T \*const out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& params_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& indices_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		const int batch_dims = 0
		)

Implementation find maximum length of *slice* of input *params* which might be copied to *out* index by index. +---- +----------- +---- + | batch | indices[:-1] | slice | | shape | shape | shape | +---- +----------- +---- +

.. _doxid-namespacengraph_1_1runtime_1_1reference_1a5cc77214b0225a1310443bebed605745:
.. index:: pair: function; matmul

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void matmul(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		bool transpose_arg0,
		bool transpose_arg1
		)

Reference kernel for matmul computation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type of input and output tensors.

	*
		- arg0

		- Pointer to the buffer for left operand input tensor.

	*
		- arg1

		- Pointer to the buffer for right operand input tensor.

	*
		- out

		- Pointer to the buffer for output tensor. This must be pre-allocated by the caller, and must be large enough to hold a tensor of the correct shape.

	*
		- arg0_shape

		- Shape of arg0.

	*
		- arg1_shape

		- Shape of arg1.

	*
		- out_shape

		- Shape of out.

	*
		- transpose_arg0

		- Flag to indicate if transpose on arg0.

	*
		- transpose_arg1

		- Flag to indicate if transpose on arg1.

.. _doxid-namespacengraph_1_1runtime_1_1reference_1a0538c05c674d21392cb54dccc5210b31:
.. index:: pair: function; non_zero_get_count

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	size_t non_zero_get_count(
		const T \* arg,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape
		)

Return number of non-zero entries in the input argument.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- arg

		- Input tensor

	*
		- arg_shape

		- Input tensor shape Output number of non-zero entries in arg

.. _doxid-namespacengraph_1_1runtime_1_1reference_1a9d9749498c328d9503fa0be68768268a:
.. index:: pair: function; non_zero

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename U>
	void non_zero(
		const T \* arg,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape
		)

Return indices of non-zero entries in input argument.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- arg

		- Input tensor

	*
		- arg_shape

		- Input tensor shape

	*
		- out

		- Output containing indices of non-zero entries in arg

