.. index:: pair: struct; InferenceEngine::gapi::kernels::linear::Mapper
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper:

struct InferenceEngine::gapi::kernels::linear::Mapper
=====================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct Mapper
	{
		// typedefs
	
		typedef short :target:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper_1a7977287d9ce4e4eb7c1d8a6e01faf766>`;
		typedef short :target:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper_1a1cccb36f9d4b504a0520f740564f574f>`;
		typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<short, short> :target:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper_1a498b1d63d699c402072da708e1ba7388>`;

		// fields
	
		static constexpr static const int :target:`unity<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper_1a0a343b5495b909157032cf687346c1a1>` = :ref:`ONE<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a60e5b210f13f69a13c4d16e73286234f>`;

		// methods
	
		static :ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper_1a498b1d63d699c402072da708e1ba7388>` :target:`map<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_1_1_mapper_1a5d97c5bf1f9c4f5a93438a64e445b566>`(double ratio, int start, int max, int outCoord);
	};

