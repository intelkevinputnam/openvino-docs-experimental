.. index:: pair: struct; InferenceEngine::gapi::kernels::linear32f::Mapper
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper:

struct InferenceEngine::gapi::kernels::linear32f::Mapper
========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct Mapper
	{
		// typedefs
	
		typedef float :target:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper_1a1d4f3bc3a03c3d17051d9961172a1bd4>`;
		typedef int :target:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper_1a50af6b344f71ddef4e9d9d8f952dd571>`;
		typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<float, int> :target:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper_1ad0628a101c74a1b632f97f07df741cb9>`;

		// fields
	
		static constexpr static const float :target:`unity<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper_1adaceaa58779bc19e4d6b8017dbaa0551>` = 1;

		// methods
	
		static :ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper_1ad0628a101c74a1b632f97f07df741cb9>` :target:`map<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear32f_1_1_mapper_1a5b016494ad88b2651df07836fea10350>`(double ratio, int start, int max, int outCoord);
	};

