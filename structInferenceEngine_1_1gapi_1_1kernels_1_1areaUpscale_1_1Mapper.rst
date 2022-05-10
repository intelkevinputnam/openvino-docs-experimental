.. index:: pair: struct; InferenceEngine::gapi::kernels::areaUpscale::Mapper
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper:

struct InferenceEngine::gapi::kernels::areaUpscale::Mapper
==========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct Mapper
	{
		// typedefs
	
		typedef short :target:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper_1ac131e3e7c9ee55bec0d7b74edc020687>`;
		typedef short :target:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper_1a7318d4bec8865bad8a5f8765d25040af>`;
		typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<short, short> :target:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper_1a1d0fef769649d4b7837f38befe14c314>`;

		// fields
	
		static constexpr static const int :target:`unity<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper_1aafc08a7523c724dbc117d7d3f8c9e155>` = :ref:`ONE<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a60e5b210f13f69a13c4d16e73286234f>`;

		// methods
	
		static :ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper_1a1d0fef769649d4b7837f38befe14c314>` :target:`map<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_upscale_1_1_mapper_1ac2cdddb77269ae2030628ff671d259c2>`(double ratio, int start, int max, int outCoord);
	};

