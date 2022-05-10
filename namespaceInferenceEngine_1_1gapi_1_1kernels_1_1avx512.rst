.. index:: pair: namespace; InferenceEngine::gapi::kernels::avx512
.. _doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512:

namespace InferenceEngine::gapi::kernels::avx512
================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace avx512 {

	// typedefs

	typedef std::integral_constant<int, 3> :target:`C3<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a558c25cfc94986257ec081c39f66ce8e>`;
	typedef std::integral_constant<int, 4> :target:`C4<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1ae3ab6cc35671c54c4d079cb85a82714d>`;

	// global functions

	CV_ALWAYS_INLINE void :target:`verticalPass_lpi4_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a752c86f6377619e9733ddef7f118b543>`(
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		uint8_t tmp[],
		const short beta[],
		const v_uint8& shuf_mask,
		const int width
		);

	CV_ALWAYS_INLINE void :target:`main_computation_horizontalPass_lpi4<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a43c81a76a6192a215d402f74b8a1e60c>`(
		const v_uint8& val_0,
		const v_uint8& val_1,
		const v_uint8& val_2,
		const v_uint8& val_3,
		const v_int16& a10,
		const v_int16& a32,
		const v_int16& a54,
		const v_int16& a76,
		v_uint8& shuf_mask1,
		v_uint8& shuf_mask2,
		v_uint32& idxs1,
		v_uint32& idxs2,
		v_uint8& res1,
		v_uint8& res2
		);

	CV_ALWAYS_INLINE void :target:`verticalPass_anylpi_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a4a94f51d52462135e62363c7ab78ddd1>`(
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		uint8_t tmp[],
		const int beta0,
		const int l,
		const int length1,
		const int length2
		);

	template <int chanNum>
	CV_ALWAYS_INLINE bool :target:`calcRowLinear_8UC_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a1741d64edbd49341daa8b3fed75bec3c>`(
		:ref:`avx512_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx512__tag>`,
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

	CV_ALWAYS_INLINE void :target:`horizontalPass_lpi4_U8C1<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a5c5bb0d378a8253b3afcb834d265791a>`(
		const short clone[],
		const short mapsx[],
		uint8_t tmp[],
		uint8_t \* dst[],
		v_uint8& shuf_mask1,
		const int width
		);

	CV_ALWAYS_INLINE void :target:`horizontalPass_anylpi_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a9dfc01b7d8d5b42616afb7c9458a999e>`(
		const short alpha[],
		const short mapsx[],
		uint8_t \* dst[],
		const uchar tmp[],
		const int l,
		const int length
		);

	void :target:`calcRowArea_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1abb940e7696e54102de212fe2a24f31a1>`(
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

	void :target:`calcRowArea_32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512_1a3e14e416465f048b353daad22681628b>`(
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

	} // namespace avx512
