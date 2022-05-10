.. index:: pair: struct; InferenceEngine::is_one_of<F, S, T...>
.. _doxid-struct_inference_engine_1_1is__one__of_3_01_f_00_01_s_00_01_t_8_8_8_01_4:

struct InferenceEngine::is_one_of<F, S, T...>
=============================================



Overview
~~~~~~~~

checks that given type is one of specified in variadic template list :ref:`More...<details-struct_inference_engine_1_1is__one__of_3_01_f_00_01_s_00_01_t_8_8_8_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers_internal.hpp>
	
	template <typename F, typename S, typename... T>
	struct is_one_of<F, S, T...>
	{
		// fields
	
		static constexpr bool :target:`value<doxid-struct_inference_engine_1_1is__one__of_3_01_f_00_01_s_00_01_t_8_8_8_01_4_1accd3f0905ec5bf17c8142465b8aefd3a>` = std::is_same<F, S>::value || :ref:`is_one_of<doxid-struct_inference_engine_1_1is__one__of>`<F, T...>::value;
	};
.. _details-struct_inference_engine_1_1is__one__of_3_01_f_00_01_s_00_01_t_8_8_8_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

checks that given type is one of specified in variadic template list



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ...

		-


.. index:: pair: struct; InferenceEngine::is_one_of
.. _doxid-struct_inference_engine_1_1is__one__of:

struct InferenceEngine::is_one_of
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

checks that given type is one of specified in variadic template list :ref:`More...<details-struct_inference_engine_1_1is__one__of>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers_internal.hpp>
	
	template <typename...>
	struct is_one_of
	{
		// fields
	
		static constexpr bool :target:`value<doxid-struct_inference_engine_1_1is__one__of_1a200b8f1de737718059f57d9ced8c467e>` = false;
	};
.. _details-struct_inference_engine_1_1is__one__of:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

checks that given type is one of specified in variadic template list



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ...

		-


