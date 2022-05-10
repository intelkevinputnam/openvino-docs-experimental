.. index:: pair: namespace; InferenceEngine::gapi::kernels::neon
.. _doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon:

namespace InferenceEngine::gapi::kernels::neon
==============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace neon {

	// typedefs

	typedef std::integral_constant<int, 3> :target:`C3<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a009678c11665c9050cad8ba66bc9227d>`;
	typedef std::integral_constant<int, 4> :target:`C4<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1ab980806c2b396517d13417cc9a57b87e>`;
	typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<float, int> :target:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a00b76ac4328fff4842f912c223092ad3>`;
	typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>`, short> :target:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a66bfce57982af2dd35a73592f856cfdd>`;

	// global functions

	template <int chanNum>
	CV_ALWAYS_INLINE void :target:`channels2planes_store<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a62a6aa636929fb337363a7eb6125b06b>`(
		std::array<std::array<uint8_t \*, 4>, chanNum>& dst,
		const uchar \* src,
		const int width,
		const int line
		);

	CV_ALWAYS_INLINE void :target:`vertical_anyLPI<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a22752767519b0f853ce0df14dcb971f4>`(
		const uchar \* src0,
		const uchar \* src1,
		uchar \* tmp,
		const int inLength,
		const short beta
		);

	template <int chanNum>
	CV_ALWAYS_INLINE void :target:`horizontal_anyLPI<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1acacbe5a61e2646d9f0b5ca974962af0d>`(
		std::array<std::array<uint8_t \*, 4>, chanNum>& dst,
		const uchar \* src,
		const short mapsx[],
		const short alpha[],
		const int width,
		const int line
		);

	CV_ALWAYS_INLINE void :target:`vertical_4LPI<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1ae805e3bb18e6c18dfd2e2aba774ded06>`(
		const uint8_t \* src0[],
		const uint8_t \* src1[],
		uchar tmp[],
		const short beta[],
		const int length
		);

	template <int chanNum>
	CV_ALWAYS_INLINE void :target:`horizontal_4LPI<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a9c4d642e17ab7dcfd05564d438c29f24>`(
		std::array<std::array<uint8_t \*, 4>, chanNum>& dst,
		const uchar \* tmp,
		const short mapsx[],
		const uchar _mask_horizontal[],
		const short clone[],
		const int length
		);

	template <int chanNum>
	CV_ALWAYS_INLINE bool :target:`calcRowLinear_8UC_Impl<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a12e150d91ab35b39d800df6af3bbdedf>`(
		:ref:`neon_tag<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1neon__tag>`,
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

	CV_ALWAYS_INLINE void :target:`horizontal_4LPI<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a71b8ab5a56dcffc2f457c4c89bc8450d>`(
		uint8_t \* dst[],
		const uchar \* tmp,
		const short mapsx[],
		const short clone[],
		const int length
		);

	CV_ALWAYS_INLINE void :target:`horizontal_anyLPI<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a1613daa490e39bbdb5f6cc5098798617>`(
		uint8_t \* dst,
		const uchar \* src,
		const short mapsx[],
		const short alpha[],
		const int length
		);

	void :target:`calcRowArea_8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a32c09f659843800eafbda7b0cd80f7a5>`(
		uchar dst[],
		const uchar \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		:ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` yalpha,
		const :ref:`MapperUnit8U<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a66bfce57982af2dd35a73592f856cfdd>`& ymap,
		int xmaxdf,
		const short xindex[],
		const :ref:`Q0_16<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aad0538fc8c280fc97bb8847d5dbeac46>` xalpha[],
		:ref:`Q8_8<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ac1d897efaf8b091b25600437bea4b796>` vbuf[]
		);

	void :target:`calcRowArea_32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a19103078d4302b51ed4d74626750e3f3>`(
		float dst[],
		const float \* src[],
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& inSz,
		const :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`& outSz,
		float yalpha,
		const :ref:`MapperUnit32F<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon_1a00b76ac4328fff4842f912c223092ad3>`& ymap,
		int xmaxdf,
		const int xindex[],
		const float xalpha[],
		float vbuf[]
		);

	} // namespace neon
