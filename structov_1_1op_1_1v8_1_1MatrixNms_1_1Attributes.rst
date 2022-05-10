.. index:: pair: struct; ov::op::v8::MatrixNms::Attributes
.. _doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes:

struct ov::op::v8::MatrixNms::Attributes
========================================



Structure that specifies attributes of the operation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <matrix_nms.hpp>
	
	struct Attributes
	{
		// fields
	
		:ref:`SortResultType<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2>` :target:`sort_result_type<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a0cfa0f63943b4c3b9b74194bf60a7ef6>` = :ref:`SortResultType::NONE<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2ab50339a10e1de285ac99d4c3990b8693>`;
		bool :target:`sort_result_across_batch<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a5ca20b7742f726194875cf9e14993922>` = false;
		:ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>` :target:`output_type<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1af18feaa8e102ffbcd0a165eee0da3ed7>` = :ref:`ov::element::i64<doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>`;
		float :target:`score_threshold<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a547a169fb867edfe2ff88aa7463ea71b>` = 0.0f;
		int :target:`nms_top_k<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a8240244e624f3a63d628644b6fef7997>` = -1;
		int :target:`keep_top_k<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1adc5c922addaaf82098fe58151278b46f>` = -1;
		int :target:`background_class<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a0266f2cac650868b217b84c4760263e4>` = -1;
		:ref:`DecayFunction<doxid-classov_1_1op_1_1v8_1_1_matrix_nms_1a152a686a5c925bf06d99743101a1a01b>` :target:`decay_function<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a44180325fbcde2f02d29ff4ebc950ece>` = :ref:`DecayFunction::LINEAR<doxid-classov_1_1op_1_1v8_1_1_matrix_nms_1a152a686a5c925bf06d99743101a1a01baaac544aacc3615aada24897a215f5046>`;
		float :target:`gaussian_sigma<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a258d489f7bb541199e199a2031a82da2>` = 2.0f;
		float :target:`post_threshold<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a3587c9b5b4d33bde199b625c7556b623>` = 0.0f;
		bool :target:`normalized<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a9b882078cf99a189ea3a28aa4a17f20c>` = true;

		// construction
	
		:target:`Attributes<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1aa154372cb47bc96e828dc1942fdc8666>`();
	
		:target:`Attributes<doxid-structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes_1a26ae9d1231cc7355dc1f970d58da0b9c>`(
			:ref:`op::v8::MatrixNms::SortResultType<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2>` sort_result_type,
			bool sort_result_across_batch,
			:ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>` output_type,
			float score_threshold,
			int nms_top_k,
			int keep_top_k,
			int background_class,
			:ref:`op::v8::MatrixNms::DecayFunction<doxid-classov_1_1op_1_1v8_1_1_matrix_nms_1a152a686a5c925bf06d99743101a1a01b>` decay_function,
			float gaussian_sigma,
			float post_threshold,
			bool normalized
			);
	};

