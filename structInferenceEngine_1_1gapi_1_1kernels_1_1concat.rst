.. index:: pair: struct; InferenceEngine::gapi::kernels::concat<left_list<left_types...>, right_list<right_types...>>
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1concat_3_01left__list_3_01left__types_8_8_8_01_4_0247354793ab4792d1cf8ed5ee568fd00:

struct InferenceEngine::gapi::kernels::concat<left_list<left_types...>, right_list<right_types...>>
===================================================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess_gapi_kernels.hpp>
	
	template <
		template<typename ...> class left_list,
		typename ... left_types,
		template<typename ...> class right_list,
		typename ... right_types
		>
	struct concat<left_list<left_types...>, right_list<right_types...>>
	{
		// typedefs
	
		typedef left_list<left_types..., right_types...> :target:`type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1concat_3_01left__list_3_01left__types_8_8_8_01_4_0247354793ab4792d1cf8ed5ee568fd00_1a1c3915657224ce153871977c1fcf5c61>`;
	};

.. index:: pair: struct; InferenceEngine::gapi::kernels::concat
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1concat:

struct InferenceEngine::gapi::kernels::concat
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






