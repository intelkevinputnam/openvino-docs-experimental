.. index:: pair: struct; InferenceEngine::gapi::kernels::areaDownscale32f::Mapper
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_downscale32f_1_1_mapper:

struct InferenceEngine::gapi::kernels::areaDownscale32f::Mapper
===============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct Mapper: public :ref:`InferenceEngine::gapi::kernels::AreaDownMapper<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper>`
	{
		// construction
	
		:target:`Mapper<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1area_downscale32f_1_1_mapper_1aeded3ee5b446d7adb9f41c5e211d4fdf>`(int _inSz, int _outSz);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef A :ref:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a54b9c9310ffd7f50e888275d94598e5a>`;
		typedef I :ref:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1af613f0cf465936203a5b9eb518f04e18>`;
		typedef :ref:`W<doxid-ie__preprocess__gapi_8cpp_1a2dd51e03005d5cb52315290d27f61870>` :ref:`work_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a530695efda3e6493b647db6a2d09cf15>`;
		typedef :ref:`MapperUnit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_mapper_unit>`<:ref:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a54b9c9310ffd7f50e888275d94598e5a>`, :ref:`index_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1af613f0cf465936203a5b9eb518f04e18>`> :ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1aa56a18503094ffe1580522ecbe1a962e>`;

		// fields
	
		int :ref:`inSz<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a9167bdf854489d90a2e662ed37060658>`;
		int :ref:`outSz<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a6d8958fdccd4e8cdd231c70b6a1196e3>`;
		double :ref:`ratio<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a442207a90b9ea006a7933ab317ca1214>`;
		double :ref:`inv_ratio<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a30807b447e1c0a7112950acdaf16d6f7>`;
		:ref:`alpha_type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a54b9c9310ffd7f50e888275d94598e5a>` :ref:`alpha<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a239112e574a1554bb6fac59d6e467d3e>`;

		// methods
	
		:ref:`Unit<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1aa56a18503094ffe1580522ecbe1a962e>` :ref:`map<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1_area_down_mapper_1a974ceba9612355701ea272ded047dc32>`(int outCoord);


