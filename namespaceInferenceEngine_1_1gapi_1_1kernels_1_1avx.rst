.. index:: pair: namespace; InferenceEngine::gapi::kernels::avx
.. _doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx:

namespace InferenceEngine::gapi::kernels::avx
=============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace avx {

	// typedefs

	typedef std::integral_constant<int, 3> :target:`C3<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1a0c3b35567d356e680e680e8657828357>`;
	typedef std::integral_constant<int, 4> :target:`C4<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1a7a3b670c84e2e41027e63046c2cb25ea>`;

	// global functions

	CV_ALWAYS_INLINE void :target:`main_computation_horizontalPass_lpi4<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1abd0bcbf224d3931e56a2a16343f380d4>`(
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
		v_uint8& res1,
		v_uint8& res2
		);

	CV_ALWAYS_INLINE void :target:`verticalPass_lpi4_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1ab3ed0e9e55133f239bd6630fa231347b>`(
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		uint8_t tmp[],
		const short beta[],
		const int& length
		);

	CV_ALWAYS_INLINE v_uint8 :target:`setHorizontalShufMask1<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1adf8681f7a5bc3dca06688ea294363938>`();
	CV_ALWAYS_INLINE v_uint8 :target:`setHorizontalShufMask2<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1a94e1610d4155605996e1bc4814c08e24>`();

	CV_ALWAYS_INLINE void :target:`verticalPass_anylpi_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1aa0741b9aaf74c45d39eb3b197a18ada3>`(
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		uint8_t tmp[],
		const int& beta0,
		const int l,
		const int length1,
		const int length2
		);

	template <int chanNum>
	CV_ALWAYS_INLINE bool :target:`calcRowLinear_8UC_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1a56e542776cb0c065b71a6b3f26e6309b>`(
		:ref:`avx2_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1avx2__tag>`,
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

	CV_ALWAYS_INLINE void :target:`horizontalPass_lpi4_8UC1<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1a8616a79f49b183186689adc39be8fb48>`(
		const short clone[],
		const short mapsx[],
		uint8_t tmp[],
		uint8_t \* dst[],
		const int& length
		);

	CV_ALWAYS_INLINE void :target:`horizontalPass_anylpi_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1ae8ebe4d3dcd7a12e3c26a461de52b9ed>`(
		const short alpha[],
		const short mapsx[],
		uint8_t \* dst[],
		const uchar tmp[],
		const int l,
		const int length
		);

	void :target:`calcRowArea_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1ae7e25a8d761ff873112202638a7cddff>`(
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

	void :target:`calcRowArea_32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx_1abed884ca734d4e60b8abd81e25703647>`(
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

	} // namespace avx
