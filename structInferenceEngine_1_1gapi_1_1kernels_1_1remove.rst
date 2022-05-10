.. index:: pair: struct; InferenceEngine::gapi::kernels::remove
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove:

struct InferenceEngine::gapi::kernels::remove
=============================================






.. index:: pair: struct; InferenceEngine::gapi::kernels::remove<list<head_t, types...>, t>
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove_3_01list_3_01head__t_00_01types_8_8_8_01_4_00_01t_01_4:

struct InferenceEngine::gapi::kernels::remove<list<head_t, types...>, t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess_gapi_kernels.hpp>
	
	template <
		template<typename ...> class list,
		typename head_t,
		typename ... types,
		typename t
		>
	struct remove<list<head_t, types...>, t>
	{
		// typedefs
	
		typedef :ref:`concat_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ad87fe34f6b6ffc476c0297d17cf41566>`<:ref:`if_<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a3c5c61b975f654a44864dba6ce1e07bf>`<:ref:`is_same_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1aec77f3009a3f9e5a5f20caf8ca0cd95d>`<:ref:`head_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae51d0df9edcdb5cda6fa7ac0eac03909>`, t>, list<>, list<:ref:`head_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1ae51d0df9edcdb5cda6fa7ac0eac03909>`>>, :ref:`remove_t<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1a72b1ddcb26e373d12e320feb27f6361f>`<list<types...>, t>> :target:`type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove_3_01list_3_01head__t_00_01types_8_8_8_01_4_00_01t_01_4_1a47d8fe34ea9efb3e85aa453c88032d12>`;
	};

.. index:: pair: struct; InferenceEngine::gapi::kernels::remove<list<>, t>
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove_3_01list_3_4_00_01t_01_4:

struct InferenceEngine::gapi::kernels::remove<list<>, t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess_gapi_kernels.hpp>
	
	template <template<typename ...> class list, typename t>
	struct remove<list<>, t>
	{
		// typedefs
	
		typedef list<> :target:`type<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1remove_3_01list_3_4_00_01t_01_4_1a933b79b3594a2b568f346e1944d9d587>`;
	};

