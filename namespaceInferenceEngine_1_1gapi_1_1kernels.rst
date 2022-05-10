.. index:: pair: namespace; InferenceEngine::gapi::kernels
.. _doxid-namespace_inference_engine_1_1gapi_1_1kernels:

namespace InferenceEngine::gapi::kernels
========================================

.. toctree::
	:hidden:

	areaDownscale32f <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1areaDownscale32f.rst>
	areaDownscale8u <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1areaDownscale8u.rst>
	areaUpscale <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1areaUpscale.rst>
	areaUpscale32f <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1areaUpscale32f.rst>
	avx <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1avx.rst>
	avx512 <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1avx512.rst>
	linear <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1linear.rst>
	linear32f <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1linear32f.rst>
	neon <namespaceInferenceEngine_1_1gapi_1_1kernels_1_1neon.rst>
	AreaDownMapper <structInferenceEngine_1_1gapi_1_1kernels_1_1AreaDownMapper.rst>
	MapperUnit <structInferenceEngine_1_1gapi_1_1kernels_1_1MapperUnit.rst>
	avx2_tag <structInferenceEngine_1_1gapi_1_1kernels_1_1avx2_tag.rst>
	avx512_tag <structInferenceEngine_1_1gapi_1_1kernels_1_1avx512_tag.rst>
	concat <structInferenceEngine_1_1gapi_1_1kernels_1_1concat.rst>
	cv_type_to_depth <structInferenceEngine_1_1gapi_1_1kernels_1_1cv_type_to_depth.rst>
	fp_16_t <structInferenceEngine_1_1gapi_1_1kernels_1_1fp_16_t.rst>
	head <structInferenceEngine_1_1gapi_1_1kernels_1_1head.rst>
	is_isa_present <structInferenceEngine_1_1gapi_1_1kernels_1_1is_isa_present.rst>
	linearScratchDesc <structInferenceEngine_1_1gapi_1_1kernels_1_1linearScratchDesc.rst>
	neon_tag <structInferenceEngine_1_1gapi_1_1kernels_1_1neon_tag.rst>
	remove <structInferenceEngine_1_1gapi_1_1kernels_1_1remove.rst>
	scalar_tag <structInferenceEngine_1_1gapi_1_1kernels_1_1scalar_tag.rst>
	sse42_tag <structInferenceEngine_1_1gapi_1_1kernels_1_1sse42_tag.rst>
	type_to_type <structInferenceEngine_1_1gapi_1_1kernels_1_1type_to_type.rst>
	typelist <structInferenceEngine_1_1gapi_1_1kernels_1_1typelist.rst>
	vector_type_of <structInferenceEngine_1_1gapi_1_1kernels_1_1vector_type_of.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace kernels {

	// namespaces

	namespace :ref:`InferenceEngine::gapi::kernels::areaDownscale32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_downscale32f>`;
	namespace :ref:`InferenceEngine::gapi::kernels::areaDownscale8u<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_downscale8u>`;
	namespace :ref:`InferenceEngine::gapi::kernels::areaUpscale<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_upscale>`;
	namespace :ref:`InferenceEngine::gapi::kernels::areaUpscale32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f>`;
	namespace :ref:`InferenceEngine::gapi::kernels::avx<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx>`;
	namespace :ref:`InferenceEngine::gapi::kernels::avx512<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512>`;
	namespace :ref:`InferenceEngine::gapi::kernels::linear<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1linear>`;
	namespace :ref:`InferenceEngine::gapi::kernels::linear32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1linear32f>`;
	namespace :ref:`InferenceEngine::gapi::kernels::neon<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon>`;

	// typedefs

	typedef std::integral_constant<int, 3> :target:`C3<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae2ec95eb2d18cf16e599498aefe926a4>`;
	typedef std::integral_constant<int, 4> :target:`C4<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad6a1aa580f28ef08a2fd73a3982931ca>`;
	typedef :ref:`typelist<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1typelist>`<:ref:`scalar_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1scalar__tag>`> :target:`isas_set<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aef72de52c900c4e61eb3f36b2d5c1d00>`;
	typedef typename :ref:`head<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1head>`<:ref:`typelist<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1typelist>`>::type :target:`head_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae51d0df9edcdb5cda6fa7ac0eac03909>`;
	typedef typename :ref:`concat<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1concat>`<left_typelsist, right_typelsist>::type :target:`concat_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad87fe34f6b6ffc476c0297d17cf41566>`;
	typedef typename std::is_same<T, U>::type :target:`is_same_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aec77f3009a3f9e5a5f20caf8ca0cd95d>`;
	typedef typename if_c_impl<:ref:`C<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a7b88edf4f396b44d0748255cdb960628>`, T, E>::type :target:`if_c<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a597f8d428d55e7b477018c5a1ab41d3b>`;
	typedef typename if_c_impl<C::value !=0, T, E>::type :target:`if_<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a3c5c61b975f654a44864dba6ce1e07bf>`;
	typedef typename :ref:`remove<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove>`<:ref:`typelist<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1typelist>`, type>::type :target:`remove_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a72b1ddcb26e373d12e320feb27f6361f>`;
	typedef uint16_t :target:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>`;
	typedef uint16_t :target:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>`;
	typedef uint8_t :target:`U8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a01f1c75898bdc17b2b87b489f2b1b467>`;
	typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<float, int> :target:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af2874c39f1cee6a3d43cead3b95fe479>`;
	typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>`, short> :target:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6a4922efc1ecffc9c5f367985fa0df08>`;
	typedef typename :ref:`vector_type_of<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1vector__type__of>`<isa_tag_t, scalar_t>::type :target:`vector_type_of_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7f18b7b1e307fbb05d71fc7a1d7778f9>`;

	// structs

	template <typename A, typename I, typename W>
	struct :ref:`AreaDownMapper<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper>`;
	template <typename F, typename I>
	struct :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`;
	struct :ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`;
	struct :ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`;
	template <
		template<typename ...> class left_list,
		typename ... left_types,
		template<typename ...> class right_list,
		typename ... right_types
		>
	struct :ref:`concat<left_list<left_types...>, right_list<right_types...>><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1concat_3_01left__list_3_01left__types_8_8_8_01_4_0247354793ab4792d1cf8ed5ee568fd00>`;
	template <typename left_typelsist, typename right_typelsist>
	struct :ref:`concat<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1concat>`;
	template <>
	struct :ref:`cv_type_to_depth<std::int8_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01std_1_1int8__t_01_4>`;
	template <>
	struct :ref:`cv_type_to_depth<std::uint8_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01std_1_1uint8__t_01_4>`;
	template <>
	struct :ref:`cv_type_to_depth<std::uint16_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01std_1_1uint16__t_01_4>`;
	template <>
	struct :ref:`cv_type_to_depth<std::int32_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01std_1_1int32__t_01_4>`;
	template <>
	struct :ref:`cv_type_to_depth<fp_16_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01fp__16__t_01_4>`;
	template <>
	struct :ref:`cv_type_to_depth<float><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01float_01_4>`;
	template <typename type>
	struct :ref:`cv_type_to_depth<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth>`;
	template <>
	struct :ref:`cv_type_to_depth<std::int16_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1cv__type__to__depth_3_01std_1_1int16__t_01_4>`;
	struct :ref:`fp_16_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1fp__16__t>`;
	template <
		template<typename ...> class list,
		typename head_t,
		typename ... types
		>
	struct :ref:`head<list<head_t, types...>><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1head_3_01list_3_01head__t_00_01types_8_8_8_01_4_01_4>`;
	template <typename type_list>
	struct :ref:`head<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1head>`;
	struct :ref:`is_isa_present<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1is__isa__present>`;
	template <typename T, typename Mapper, int chanNum>
	struct :ref:`linearScratchDesc<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc>`;
	struct :ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`;
	template <typename typelist, typename type>
	struct :ref:`remove<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove>`;
	template <
		template<typename ...> class list,
		typename head_t,
		typename ... types,
		typename t
		>
	struct :ref:`remove<list<head_t, types...>, t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove_3_01list_3_01head__t_00_01types_8_8_8_01_4_00_01t_01_4>`;
	template <template<typename ...> class list, typename t>
	struct :ref:`remove<list<>, t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove_3_01list_3_4_00_01t_01_4>`;
	struct :ref:`scalar_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1scalar__tag>`;
	struct :ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`;
	template <typename type>
	struct :ref:`type_to_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1type__to__type>`;
	template <typename ... types>
	struct :ref:`typelist<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1typelist>`;
	template <typename isa_tag_t, typename scalar_t>
	struct :ref:`vector_type_of<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1vector__type__of>`;
	template <typename isa_tag_t>
	struct :ref:`vector_type_of<isa_tag_t, float><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1vector__type__of_3_01isa__tag__t_00_01float_01_4>`;
	template <typename isa_tag_t>
	struct :ref:`vector_type_of<isa_tag_t, uint8_t><doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1vector__type__of_3_01isa__tag__t_00_01uint8__t_01_4>`;

	// global variables

	static constexpr static const int :target:`ONE<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a60e5b210f13f69a13c4d16e73286234f>` = 1<<15;
	static const int :target:`ITUR_BT_601_CY<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a071e7a3904198471b2a830ddcd5be0ab>` = 1220542;
	static const int :target:`ITUR_BT_601_CUB<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a65613848d829d14f88f2512fffeef8c8>` = 2116026;
	static const int :target:`ITUR_BT_601_CUG<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa324243069a2d28e4e55f0255fc194e1>` = -409993;
	static const int :target:`ITUR_BT_601_CVG<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1abdb1cce3508d712f4425ed3078bd0bb0>` = -852492;
	static const int :target:`ITUR_BT_601_CVR<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af9e266a5209dbd608678c17090828b1e>` = 1673527;
	static const int :target:`ITUR_BT_601_SHIFT<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af10fbb3c7f3c2952f1ab43f759a7f036>` = 20;

	// global functions

	bool :target:`calcRowLinear8UC3C4Impl< neon_tag, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ab2622091ec8980852afd2539dc289d7d>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		std::array<std::array<uint8_t \*, 4>, 3>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC3C4Impl< neon_tag, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a8bd85d515ae6483a46ff8d397c9a5184>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		std::array<std::array<uint8_t \*, 4>, 4>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a26026795f88752bbac692d8422f59caa>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		uint8_t \* dst[],
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2a17b7f813b2b4bad069fd63047eb6e8>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const uint8_t \* in,
		int chan,
		int chs,
		uint8_t \* out,
		const int length
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af0caa8e93bc3df7ca997d3d0a336d3c5>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const float \* in,
		int chan,
		int chs,
		float \* out,
		const int length
		);

	template void :target:`nv12ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1acf5dcf0ba1d48b18c98621b949a6976e>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* uv_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`i420ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a90c8a3bdb3de752c0feb397242e61156>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* u_row,
		const uint8_t \* v_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`splitRowImpl< neon_tag, uint8_t, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a75fb92e08ee8e4f500c8f0c757ae12a8>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< neon_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a5a0e275b731a4f5dbd236604ff768196>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const float \* in,
		std::array<float \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< neon_tag, uint8_t, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ab55724ed93ba77133f560ca09b1844d8>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< neon_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7ce3eb363a19868b83bc8ccbe12b2f24>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const float \* in,
		std::array<float \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< neon_tag, uint8_t, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aed807cc66ffe9f0d164bac2e457d0653>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 4>& outs,
		const int length
		);

	template void :target:`splitRowImpl< neon_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7d15284e8bac11333f68dba33918f760>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const float \* in,
		std::array<float \*, 4>& outs,
		const int length
		);

	template void :target:`mergeRowImpl< neon_tag, uint8_t, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae2f598abdd913676c8117c0f2c7a8f4f>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const std::array<const uint8_t \*, 2>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< neon_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae8bdaa35c3fbfe0e78fc6d10c6430311>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const std::array<const float \*, 2>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< neon_tag, uint8_t, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa8d41bb16e266c674029ff68a5811832>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const std::array<const uint8_t \*, 3>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< neon_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa85f7901c6906b980ffa9ed601298810>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const std::array<const float \*, 3>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< neon_tag, uint8_t, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a389a10700498a77299cfa485eacc2102>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const std::array<const uint8_t \*, 4>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< neon_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aca6f586a4b38de98b9e9a77b1242496b>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		const std::array<const float \*, 4>& ins,
		float \* out,
		const int length
		);

	template void :target:`calcRowLinear32FC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a635c144c970eef7619b4c939ed01dc48>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		float \* dst[],
		const float \* src0[],
		const float \* src1[],
		const float alpha[],
		const int mapsx[],
		const float beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template void :target:`calcRowAreaImpl< neon_tag, uint8_t, Q0_16, short, Q8_8 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a34bd6c529f3d43c63bfb890392d8aeeb>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		uint8_t dst[],
		const uint8_t \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` yalpha,
		const :ref:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6a4922efc1ecffc9c5f367985fa0df08>`& ymap,
		int xmaxdf,
		const short xindex[],
		const :ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` xalpha[],
		:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` vbuf[]
		);

	template void :target:`calcRowAreaImpl< neon_tag, float, float, int, float ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae405833dec2bbeab55a5d4aa77ae2c3f>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
		float dst[],
		const float \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		float yalpha,
		const :ref:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af2874c39f1cee6a3d43cead3b95fe479>`& ymap,
		int xmaxdf,
		const int xindex[],
		const float xalpha[],
		float vbuf[]
		);

	template <typename isa_tag_t, typename T>
	void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa7c374ac1c73b9fbd6148245129a2f60>`(
		isa_tag_t,
		const T \* in,
		const int chan,
		const int chs,
		T \* out,
		const int length
		);

	template <typename isa_tag_t>
	void :target:`nv12ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a5912e2be66edb1049632a56ae530b444>`(
		isa_tag_t,
		const uint8_t \*\* y_rows,
		const uint8_t \* uv_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template <typename isa_tag_t>
	void :target:`i420ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4c179878e69bd60ef7772fd8411185b4>`(
		isa_tag_t,
		const uint8_t \*\* y_rows,
		const uint8_t \* u_row,
		const uint8_t \* v_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template <typename isa_tag_t, typename T, int chs>
	void :target:`splitRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7dd38afa16d51785704eb52a4bab96b9>`(
		isa_tag_t,
		const T \* in,
		std::array<T \*, chs>& outs,
		const int length
		);

	template <typename isa_tag_t, typename T, int chs>
	void :target:`mergeRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ab1d2931524fb9fd0abd5689349ba8ca3>`(
		isa_tag_t,
		const std::array<const T \*, chs>& ins,
		T \* out,
		const int length
		);

	template <typename isa_tag_t>
	bool :target:`calcRowLinear8UC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af7930cac9b3740514b92203dc925ef77>`(
		isa_tag_t,
		uint8_t \* dst[],
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template <typename isa_tag_t>
	void :target:`calcRowLinear32FC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a970b1e70b72fe8a435bca621feb0633f>`(
		isa_tag_t,
		float \* dst[],
		const float \* src0[],
		const float \* src1[],
		const float alpha[],
		const int mapsx[],
		const float beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template <typename isa_tag_t, int chs>
	bool :target:`calcRowLinear8UC3C4Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7536aea40065b26b2ed43f2fb3300cda>`(
		isa_tag_t,
		std::array<std::array<uint8_t \*, 4>, chs>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template <typename isa_tag_t, typename T, typename A, typename I, typename W>
	void :target:`calcRowAreaImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a437c0f3c44948011ef4c4c7a59aafbb2>`(
		isa_tag_t,
		T dst[],
		const T \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		A yalpha,
		const :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<A, I>& ymap,
		int xmaxdf,
		const I xindex[],
		const A xalpha[],
		:ref:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>` vbuf[]
		);

	bool :target:`calcRowLinear8UC3C4Impl< avx2_tag, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a8516aed4ba7bcc724773f3bb9992a2b8>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		std::array<std::array<uint8_t \*, 4>, 3>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC3C4Impl< avx2_tag, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a9c2fbc02604d1addbe04f0f7faf42469>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		std::array<std::array<uint8_t \*, 4>, 4>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4e3bfbb998cf2ab93ac6cea1f831d5d3>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		uint8_t \* dst[],
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a556a9d4b3eaec4dfee6a2e8b3c4771a4>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const uint8_t \* in,
		const int chan,
		const int chs,
		uint8_t \* out,
		const int length
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae7c9ea3d819b41d5e061ff4c4ffbe76c>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const float \* in,
		const int chan,
		const int chs,
		float \* out,
		const int length
		);

	template void :target:`nv12ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a0efbb01477263e9aa8a978ce4c40d33b>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* uv_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`i420ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7381d0174c1ebe66d6c6f589ffef748a>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* u_row,
		const uint8_t \* v_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`splitRowImpl< avx2_tag, uint8_t, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a952b74b1b484eb713cda7de1945731c6>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx2_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a944d83f4ffce9a8dd07dd1a0f4c55f1e>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const float \* in,
		std::array<float \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx2_tag, uint8_t, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a3e8c6958593a62ccbf4083be662ef77a>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx2_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1addc8fa7b85b382cd792752a52187c22d>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const float \* in,
		std::array<float \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx2_tag, uint8_t, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac85c0c5f227d65c5bb43018d938dc7d7>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 4>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx2_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1156500a94b8d707336a70d8cea3bb7c>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const float \* in,
		std::array<float \*, 4>& outs,
		const int length
		);

	template void :target:`mergeRowImpl< avx2_tag, uint8_t, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1d34146e67ce0ac4ea77b126877ae906>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const std::array<const uint8_t \*, 2>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx2_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1addcd56c43b1282edf94b5715c5d3ffe0>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const std::array<const float \*, 2>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx2_tag, uint8_t, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad613fabc6b06f922b5c955ee51480ab1>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const std::array<const uint8_t \*, 3>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx2_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1600a9a9c32aefebf777281b251e369f>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const std::array<const float \*, 3>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx2_tag, uint8_t, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a3a74fbd11267e07312eff200acc8c620>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const std::array<const uint8_t \*, 4>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx2_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2dde4f90a9c56eca2b3587c82098e0e5>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		const std::array<const float \*, 4>& ins,
		float \* out,
		const int length
		);

	template void :target:`calcRowLinear32FC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a9451f1fef8b7f28ea65c309ef6923223>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		float \* dst[],
		const float \* src0[],
		const float \* src1[],
		const float alpha[],
		const int mapsx[],
		const float beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template void :target:`calcRowAreaImpl< avx2_tag, uint8_t, Q0_16, short, Q8_8 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad7e4e10dc169474a3a46a49b26e9bbe3>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		uint8_t dst[],
		const uint8_t \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` yalpha,
		const :ref:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6a4922efc1ecffc9c5f367985fa0df08>`& ymap,
		int xmaxdf,
		const short xindex[],
		const :ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` xalpha[],
		:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` vbuf[]
		);

	template void :target:`calcRowAreaImpl< avx2_tag, float, float, int, float ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a61bdcc720bfc776b62807d3e7ae37a63>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
		float dst[],
		const float \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		float yalpha,
		const :ref:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af2874c39f1cee6a3d43cead3b95fe479>`& ymap,
		int xmaxdf,
		const int xindex[],
		const float xalpha[],
		float vbuf[]
		);

	bool :target:`calcRowLinear8UC3C4Impl< avx512_tag, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4446121036aa3fbb16a9fc0e765c2e44>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		std::array<std::array<uint8_t \*, 4>, 3>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC3C4Impl< avx512_tag, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1512faee57a92455a5722b6e4ef0f7b2>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		std::array<std::array<uint8_t \*, 4>, 4>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1adb7659fd09e8fdbe19f0b2287cb43fbb>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		uint8_t \* dst[],
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad37bda598fd89a75887b8285fe582cfd>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const uint8_t \* in,
		const int chan,
		const int chs,
		uint8_t \* out,
		const int length
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a9c4d04817e1e52ceaedbd17322060b2d>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const float \* in,
		const int chan,
		const int chs,
		float \* out,
		const int length
		);

	template void :target:`nv12ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ab272775d7f61a69a9a0ae5f9764e5b2a>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* uv_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`i420ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1accddade7581fb02b699b20452703696a>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* u_row,
		const uint8_t \* v_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`splitRowImpl< avx512_tag, uint8_t, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af02ca4e59aff0a782e3bb6eaee73fb65>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx512_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac2527b7d77130bd717fa99b5f910ea45>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const float \* in,
		std::array<float \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx512_tag, uint8_t, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7d74e443d6c836297d646adb045868f8>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx512_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a9d44ba186d45d5c54f3d6d9de3619e82>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const float \* in,
		std::array<float \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx512_tag, uint8_t, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a5be2aa30005447941c89ef7d8a2d5809>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 4>& outs,
		const int length
		);

	template void :target:`splitRowImpl< avx512_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a94b915bd088cc41927b617d0102f9384>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const float \* in,
		std::array<float \*, 4>& outs,
		const int length
		);

	template void :target:`mergeRowImpl< avx512_tag, uint8_t, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6bf722781d3d8a4dcfd05ec5bb5a3dee>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const std::array<const uint8_t \*, 2>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx512_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a3be16e51bfe63a0f8feb11d717c8f779>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const std::array<const float \*, 2>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx512_tag, uint8_t, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a97b9ee4d3c82eca20b7113894b954bcf>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const std::array<const uint8_t \*, 3>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx512_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4e96a784433767950a400369bc093ea2>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const std::array<const float \*, 3>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx512_tag, uint8_t, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4e4881a92657fd9e1f1ac0a7d5c68727>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const std::array<const uint8_t \*, 4>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< avx512_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4488db1c2ce03ef5295c15ef60a59e6d>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		const std::array<const float \*, 4>& ins,
		float \* out,
		const int length
		);

	template void :target:`calcRowLinear32FC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6e74ac475722fe2bc5ea361c36d38d42>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		float \* dst[],
		const float \* src0[],
		const float \* src1[],
		const float alpha[],
		const int mapsx[],
		const float beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template void :target:`calcRowAreaImpl< avx512_tag, uint8_t, Q0_16, short, Q8_8 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1afb8c937c08e9854643154067af7073c1>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		uint8_t dst[],
		const uint8_t \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` yalpha,
		const :ref:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6a4922efc1ecffc9c5f367985fa0df08>`& ymap,
		int xmaxdf,
		const short xindex[],
		const :ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` xalpha[],
		:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` vbuf[]
		);

	template void :target:`calcRowAreaImpl< avx512_tag, float, float, int, float ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a025a0afaa976212f738b52294456e004>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
		float dst[],
		const float \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		float yalpha,
		const :ref:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af2874c39f1cee6a3d43cead3b95fe479>`& ymap,
		int xmaxdf,
		const int xindex[],
		const float xalpha[],
		float vbuf[]
		);

	bool :target:`calcRowLinear8UC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a918ad6d28eaef6af8273c1943232e619>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		uint8_t \* dst[],
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	template <int chanNum>
	CV_ALWAYS_INLINE bool :target:`calcRowLinear_8UC_Impl_<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1dbf0c2bc8a93b203123d6eeec2c2490>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		std::array<std::array<uint8_t \*, 4>, chanNum>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi
		);

	bool :target:`calcRowLinear8UC3C4Impl< sse42_tag, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a91b34403ef81c39d367b7621a414d08d>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		std::array<std::array<uint8_t \*, 4>, 3>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	bool :target:`calcRowLinear8UC3C4Impl< sse42_tag, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a99c99aec9c481d27d0415e210cdc403c>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		std::array<std::array<uint8_t \*, 4>, 4>& dst,
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		const short alpha[],
		const short clone[],
		const short mapsx[],
		const short beta[],
		uint8_t tmp[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a18db784a314f11830873f61881637554>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const uint8_t \* in,
		const int chan,
		const int chs,
		uint8_t \* out,
		const int length
		);

	template void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6abb9433b068806740362836ce87714b>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const float \* in,
		const int chan,
		const int chs,
		float \* out,
		const int length
		);

	template void :target:`nv12ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a98cd0a1b244baf40b80644e75946935f>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* uv_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`i420ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae093e65f52905c906d2b8d9d4172bd95>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const uint8_t \*\* y_rows,
		const uint8_t \* u_row,
		const uint8_t \* v_row,
		uint8_t \*\* out_rows,
		const int buf_width
		);

	template void :target:`splitRowImpl< sse42_tag, uchar, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad199cc6dcdb81770e72001bba197d246>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< sse42_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1512bb44bec8971a99163277f3674ca8>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const float \* in,
		std::array<float \*, 2>& outs,
		const int length
		);

	template void :target:`splitRowImpl< sse42_tag, uchar, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a09ac94c6ae6bb141c4636c69bccbc557>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< sse42_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7af01e8391de9c8f9bb205ae51173a70>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const float \* in,
		std::array<float \*, 3>& outs,
		const int length
		);

	template void :target:`splitRowImpl< sse42_tag, uchar, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad12620939ec9f9d3fcfaff35ca0c8ddb>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const uint8_t \* in,
		std::array<uint8_t \*, 4>& outs,
		const int length
		);

	template void :target:`splitRowImpl< sse42_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad71d7a26af27cf49722d5e89a45c351d>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const float \* in,
		std::array<float \*, 4>& outs,
		const int length
		);

	template void :target:`mergeRowImpl< sse42_tag, uchar, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac24aa0f55a577f42a7914a6e0ec5ecc5>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const std::array<const uint8_t \*, 2>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< sse42_tag, float, 2 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa25a4f63eaf7ec78edea30a2f9e65c89>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const std::array<const float \*, 2>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< sse42_tag, uchar, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1f9809aafba2ffe0b91ce08c2780655c>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const std::array<const uint8_t \*, 3>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< sse42_tag, float, 3 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af8c0d1424bfd44d5a3c590cc3cebbb83>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const std::array<const float \*, 3>& ins,
		float \* out,
		const int length
		);

	template void :target:`mergeRowImpl< sse42_tag, uchar, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af47e0de1cc65a9956cbf486358ac9a80>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const std::array<const uint8_t \*, 4>& ins,
		uint8_t \* out,
		const int length
		);

	template void :target:`mergeRowImpl< sse42_tag, float, 4 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a4fe17115690dd239c660fa7d9d394fe5>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		const std::array<const float \*, 4>& ins,
		float \* out,
		const int length
		);

	template void :target:`calcRowLinear32FC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2ed5b611c8504377d64871c34b0e214b>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		float \* dst[],
		const float \* src0[],
		const float \* src1[],
		const float alpha[],
		const int mapsx[],
		const float beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int l
		);

	template void :target:`calcRowAreaImpl< sse42_tag, uint8_t, Q0_16, short, Q8_8 ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a501a1b59c913cd2252abdc59e152c6f2>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		uint8_t dst[],
		const uint8_t \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` yalpha,
		const :ref:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6a4922efc1ecffc9c5f367985fa0df08>`& ymap,
		int xmaxdf,
		const short xindex[],
		const :ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` xalpha[],
		:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` vbuf[]
		);

	template void :target:`calcRowAreaImpl< sse42_tag, float, float, int, float ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1afbc800310ca3eb8ca269d12a42978b56>`(
		:ref:`sse42_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1sse42__tag>`,
		float dst[],
		const float \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		float yalpha,
		const :ref:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af2874c39f1cee6a3d43cead3b95fe479>`& ymap,
		int xmaxdf,
		const int xindex[],
		const float xalpha[],
		float vbuf[]
		);

	void :target:`calcRowArea_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae3683478d9ea2b9870ac07a726da1848>`(
		uchar dst[],
		const uchar \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` yalpha,
		const :ref:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6a4922efc1ecffc9c5f367985fa0df08>`& ymap,
		int xmaxdf,
		const short xindex[],
		const :ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` xalpha[],
		:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` vbuf[]
		);

	void :target:`calcRowArea_32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2aeeba01c1cb2b3f8861a8bd3bd55afb>`(
		float dst[],
		const float \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		float yalpha,
		const :ref:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af2874c39f1cee6a3d43cead3b95fe479>`& ymap,
		int xmaxdf,
		const int xindex[],
		const float xalpha[],
		float vbuf[]
		);

	bool :target:`is_present<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1af46d9bfc2d7122b63da1236089ec2291>`(:ref:`scalar_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1scalar__tag>`);
	static double :target:`invRatio<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a0cb2a9f92f973336df401ae2625a127d>`(int inSz, int outSz);
	static double :target:`ratio<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1f55e34842c07214f7a500d2807fdd49>`(int inSz, int outSz);

	template <typename T, typename Mapper, int chanNum = 1>
	static void :target:`initScratchLinear<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a9fde0725f11aa265b7ac46bacd95f050>`(
		const cv::GMatDesc& in,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		cv::gapi::fluid::Buffer& scratch,
		int lpi
		);

	template <typename T, typename IT, typename AT, class Mapper>
	void :target:`calcRowLinearC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aafef688e31b5e31b8acbcac45e35c192>`(
		T \* dst[],
		const T \* src0[],
		const T \* src1[],
		const AT alpha[],
		const IT mapsx[],
		const AT beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int length
		);

	template <typename Mapper>
	static void :target:`initScratchArea<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a38c856d57faf9f601f0ff6c1a90a7799>`(
		const cv::GMatDesc& in,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		cv::gapi::fluid::Buffer& scratch
		);

	cv::gapi::GKernelPackage :target:`FKernelsChooseISA<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a5ee012cb620bd70c911f610d0b787a78>`();
	:target:`GAPI_COMPOUND_KERNEL<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a76f9eb54826de80615d653a43abc61b1>`(FScalePlane, ScalePlane);
	:target:`GAPI_FLUID_KERNEL<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a554bb480980cd068f6af36088858e1c6>`(FConvertDepth, ConvertDepth, false);
	:target:`GAPI_FLUID_KERNEL<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a86f1d62c1c54cf822e58f34d734075f3>`(FSubC, GSubC, false);
	:target:`GAPI_FLUID_KERNEL<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a637a9d502a61fcc6405fa4976734741b>`(FDivC, GDivC, false);

	template <
		typename typelist,
		typename default_t,
		typename type_id_t,
		typename type_to_id_t,
		typename type_to_value_t,
		typename result_t = decltype(std::declval<type_to_value_t>()(type_to_type<head_t<typelist>> {}))
		>
	result_t :target:`type_dispatch<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1afa8a6eb5c5e67f8486aaaac9cf1a755c>`(
		type_id_t type_id,
		type_to_id_t&& type_to_id,
		type_to_value_t&& type_to_value,
		default_t default_value = {}
		);

	template <
		typename typelist,
		typename default_t,
		typename pred_t,
		typename type_to_value_t,
		typename result_t = decltype(std::declval<type_to_value_t>()(type_to_type<head_t<typelist>> {}))
		>
	result_t :target:`type_dispatch<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7381e6d7b83d09024c4e7dbb8146264d>`(
		pred_t&& pred,
		type_to_value_t&& type_to_value,
		default_t default_value = {}
		);

	template <typename typelist>
	bool :target:`is_cv_type_in_list<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1abc5ad1c1b6ae0421981a6c372a1c133f>`(const int type_id);

	template <typename DST, typename SRC>
	static DST :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a30d404e3ec5c202f52b120e0a83de554>`(SRC x);

	short :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae9a14978ba6519c44aebe80b51bbd98f>`(int x);
	short :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a515eda6c007cda42fa0b16467d223197>`(float x);
	short :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa1201a8f426884f5aebf888fdb309df2>`(short x);
	uint16_t :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a8b5c0691a7e64cb31432cb036c068315>`(uint16_t x);
	uchar :target:`saturate_cast< uchar ><doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aee78211425e1006024643da46acb9ab2>`(int v);
	uint16_t :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a60c08e09e15d076bd96e1c38de277f47>`(uint8_t x);
	float :target:`saturate_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a8bc8e890b924751b8f785f2de168415e>`(double x);
	static uint8_t :target:`calc<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a7b33753854d93ebbf019374dd1319c84>`(short alpha0, uint8_t src0, short alpha1, uint8_t src1);
	static float :target:`calc<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a5f134ce84e3166ccec4d72ccecc610ee>`(float alpha0, float src0, float alpha1, float src1);

	template <typename DST, typename SRC>
	static DST :target:`convert_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad101a3c9dad365fc626c9f498b74da95>`(SRC x);

	uint8_t :target:`convert_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2a340ab80f8c6490c8596ae1170603d0>`(uint8_t x);
	uint8_t :target:`convert_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a85589133795230e651dc6bd854ff305e>`(float x);
	float :target:`convert_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2ae61cd2869cd0a8373c849f7e81eade>`(double x);
	:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` :target:`convert_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1adbdf8002c8b0c2cfe706ecddd50896cf>`(uchar x);
	uchar :target:`convert_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2cd2351db65efad5eee4e2cdc8ca26a0>`(:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` x);

	template <typename DST, typename SRC>
	static DST :target:`checked_cast<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae0df600ec4de2d6acfd491f4dc85f688>`(SRC x);

	static :ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` :target:`mulas<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa5b392d7c52414f88db17ee9ece17d2e>`(:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` a, :ref:`U8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a01f1c75898bdc17b2b87b489f2b1b467>` s);
	static :ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` :target:`mulaw<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1acf477b39cb6c4419bc3e7a46f18a6ec2>`(:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` a, :ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` w);
	static float :target:`mulas<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a802cd0f73935edb7511d8d2ac27779f3>`(float a, float s);
	static float :target:`mulaw<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2a82efe51d15230ff2494fe70bd65c8e>`(float a, float w);

	static void :target:`uvToRGBuv<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aa0b2d72f5cdc4bb8dcabd79a086aa4c6>`(
		const uchar u,
		const uchar v,
		int& ruv,
		int& guv,
		int& buv
		);

	static void :target:`yRGBuvToRGB<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a95023c5a0aa69adf4e811d209b99a7d0>`(
		const uchar vy,
		const int ruv,
		const int guv,
		const int buv,
		uchar& r,
		uchar& g,
		uchar& b
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`mergeRowC2_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad44f7fccb0bdde6758f8f957eeef69ba>`(
		const T in0[],
		const T in1[],
		T out[],
		const int length
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`mergeRowC3_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6f297184e0e369d14f4a21d32f4d198b>`(
		const T in0[],
		const T in1[],
		const T in2[],
		T out[],
		const int length
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`mergeRowC4_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a80eb6e84c60a97c30df8fdf5a037c6ac>`(
		const T in0[],
		const T in1[],
		const T in2[],
		const T in3[],
		T out[],
		const int length
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`splitRowC2_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a1b9a5690cde8f98bee57b912a2933a62>`(
		const T in[],
		T out0[],
		T out1[],
		const int length
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`splitRowC3_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a08094625132c8b1a86dc1551348f14b9>`(
		const T in[],
		T out0[],
		T out1[],
		T out2[],
		const int length
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`splitRowC4_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad72bd8ee0bfb9afb8f41e5c4a38d551d>`(
		const T in[],
		T out0[],
		T out1[],
		T out2[],
		T out3[],
		const int length
		);

	CV_ALWAYS_INLINE void :target:`uvToRGBuv<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a714c48f6e94cd6a11dbfe8345a74dbe9>`(
		const v_uint8& u,
		const v_uint8& v,
		v_int32(&) ruv[4],
		v_int32(&) guv[4],
		v_int32(&) buv[4]
		);

	CV_ALWAYS_INLINE void :target:`yRGBuvToRGB<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1adf1e8785574e27a2d8bfbaa7a5a651c4>`(
		const v_uint8& vy,
		const v_int32(&) ruv[4],
		const v_int32(&) guv[4],
		const v_int32(&) buv[4],
		v_uint8& rr,
		v_uint8& gg,
		v_uint8& bb
		);

	template <typename isa_tag_t>
	CV_ALWAYS_INLINE void :target:`nv12ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a180de114d5bd7060e2a5da26a322c740>`(
		isa_tag_t,
		const uchar \*\* srcY,
		const uchar \* srcUV,
		uchar \*\* dstRGBx,
		const int width
		);

	template <typename isa_tag_t>
	CV_ALWAYS_INLINE void :target:`i420ToRgbRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1abdc84c3a31a1e3a3938985c42ee1bb0f>`(
		isa_tag_t,
		const uint8_t \*\* srcY,
		const uint8_t \* srcU,
		const uint8_t \* srcV,
		uint8_t \*\* dstRGBx,
		const int width
		);

	template <typename T, typename A, typename I, typename W>
	CV_ALWAYS_INLINE void :target:`downy<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a99363167115f5546dd8bbef9883d09ed>`(
		const T \* src[],
		int inWidth,
		const :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<A, I>& ymap,
		A yalpha,
		:ref:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>` vbuf[]
		);

	template <typename T, typename A, typename I, typename W>
	CV_ALWAYS_INLINE void :target:`downx<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a21543ea2ed233361a9ac1ee11e5e62c8>`(
		T dst[],
		int outWidth,
		int xmaxdf,
		const I xindex[],
		const A xalpha[],
		const :ref:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>` vbuf[]
		);

	template <typename isa_tag_t, typename T, typename A, typename I, typename W>
	CV_ALWAYS_INLINE void :target:`calcRowAreaImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a6bc23bf6b164ab46a855b9ef31c1ffe4>`(
		isa_tag_t,
		T dst[],
		const T \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		A yalpha,
		const :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<A, I>& ymap,
		int xmaxdf,
		const I xindex[],
		const A xalpha[],
		:ref:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>` vbuf[]
		);

	template <typename VecT, typename T>
	CV_ALWAYS_INLINE void :target:`copyRow_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a84519614f6bb1a3e65aaf1c5c722f6ab>`(
		const T in[],
		T out[],
		int length
		);

	template <typename isa_tag_t>
	CV_ALWAYS_INLINE void :target:`calcRowLinear32FC1Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ab05f4d5f5e8cc3d97c007a20a580e3b9>`(
		isa_tag_t,
		float \* dst[],
		const float \* src0[],
		const float \* src1[],
		const float alpha[],
		const int mapsx[],
		const float beta[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		const int lpi,
		const int
		);

	template <typename isa_tag_t, typename T>
	CV_ALWAYS_INLINE void :target:`chanToPlaneRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a29d0c729397082331b67cabe73dac04f>`(
		isa_tag_t,
		const T \* in,
		const int chan,
		const int chs,
		T \* out,
		const int length
		);

	template <typename isa_tag_t, typename T, int chs>
	CV_ALWAYS_INLINE void :target:`splitRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a2e27e185ecec8877205e4215b3785cbf>`(
		isa_tag_t,
		const T \* in,
		std::array<T \*, chs>& outs,
		const int length
		);

	template <typename isa_tag_t, typename T, int chs>
	CV_ALWAYS_INLINE void :target:`mergeRowImpl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad6b00f73cc64e9cad5962ddef0962814>`(
		isa_tag_t,
		const std::array<const T \*, chs>& ins,
		T \* out,
		const int length
		);

	} // namespace kernels
