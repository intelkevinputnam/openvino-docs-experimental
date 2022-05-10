.. index:: pair: struct; InferenceEngine::gapi::kernels::areaUpscale32f::Mapper
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper:

struct InferenceEngine::gapi::kernels::areaUpscale32f::Mapper
=============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct Mapper
	{
		// typedefs
	
		typedef float :target:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper_1a9373e522a0b6492abf105b46cbaeb26b>`;
		typedef int :target:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper_1a915157c17e95dd9ae44253c98e4d1cde>`;
		typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<float, int> :target:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper_1a0253eaf7c9eef430d1da4c521b35d690>`;

		// fields
	
		static constexpr static const float :target:`unity<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper_1a3f45aedd6e0444cd05e00ef5629ce236>` = 1;

		// methods
	
		static :ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper_1a0253eaf7c9eef430d1da4c521b35d690>` :target:`map<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f_1_1_mapper_1a0510a5832103056092c7dd0fc6ff4c17>`(double ratio, int start, int max, int outCoord);
	};

