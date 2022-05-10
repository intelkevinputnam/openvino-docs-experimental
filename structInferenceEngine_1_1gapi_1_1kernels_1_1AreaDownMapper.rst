.. index:: pair: struct; InferenceEngine::gapi::kernels::AreaDownMapper
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper:

struct InferenceEngine::gapi::kernels::AreaDownMapper
=====================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename A, typename I, typename W>
	struct AreaDownMapper
	{
		// typedefs
	
		typedef A :target:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a54b9c9310ffd7f50e888275d94598e5a>`;
		typedef I :target:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1af613f0cf465936203a5b9eb518f04e18>`;
		typedef :ref:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>` :target:`work_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a530695efda3e6493b647db6a2d09cf15>`;
		typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<:ref:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a54b9c9310ffd7f50e888275d94598e5a>`, :ref:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1af613f0cf465936203a5b9eb518f04e18>`> :target:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1aa56a18503094ffe1580522ecbe1a962e>`;

		// fields
	
		int :target:`inSz<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a9167bdf854489d90a2e662ed37060658>`;
		int :target:`outSz<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a6d8958fdccd4e8cdd231c70b6a1196e3>`;
		double :target:`ratio<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a442207a90b9ea006a7933ab317ca1214>`;
		double :target:`inv_ratio<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a30807b447e1c0a7112950acdaf16d6f7>`;
		:ref:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a54b9c9310ffd7f50e888275d94598e5a>` :target:`alpha<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a239112e574a1554bb6fac59d6e467d3e>`;

		// construction
	
		:target:`AreaDownMapper<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1aecb66ba8a022eda7ebef2ab57002d9b9>`(int _inSz, int _outSz);

		// methods
	
		:ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1aa56a18503094ffe1580522ecbe1a962e>` :target:`map<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a974ceba9612355701ea272ded047dc32>`(int outCoord);
	};

	// direct descendants

	struct :ref:`Mapper<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_downscale8u_1_1_mapper>`;
	struct :ref:`Mapper<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_downscale32f_1_1_mapper>`;

