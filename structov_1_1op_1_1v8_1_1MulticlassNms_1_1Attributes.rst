.. index:: pair: struct; ov::op::v8::MulticlassNms::Attributes
.. _doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes:

struct ov::op::v8::MulticlassNms::Attributes
============================================



Structure that specifies attributes of the operation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multiclass_nms.hpp>
	
	struct Attributes
	{
		// fields
	
		:ref:`SortResultType<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2>` :target:`sort_result_type<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1a618a633f74eecd70467614f2e4267777>` = :ref:`SortResultType::NONE<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2ab50339a10e1de285ac99d4c3990b8693>`;
		bool :target:`sort_result_across_batch<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1a17dd7ca9503e4ef0473446546f3a9537>` = false;
		:ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>` :target:`output_type<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1a422725e88f01736bda0db8c27e0dc582>` = :ref:`ov::element::i64<doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>`;
		float :target:`iou_threshold<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1a79b1dfb1c0cd097d0d4b16422519f076>` = 0.0f;
		float :target:`score_threshold<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1ac6ab09da153f839651f23546952f4e9f>` = 0.0f;
		int :target:`nms_top_k<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1aa30bad75f184ef81aa91ecd03950dfbe>` = -1;
		int :target:`keep_top_k<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1a00296d79b6142776fad59db55ee0a3d8>` = -1;
		int :target:`background_class<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1ad670e2692b4d11a3f79a9f3b83ae4148>` = -1;
		float :target:`nms_eta<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1a7b304e81b98465c2b9724a6918e66e04>` = 1.0f;
		bool :target:`normalized<doxid-structov_1_1op_1_1v8_1_1_multiclass_nms_1_1_attributes_1af471ad5af245874919afe0f166bb20ce>` = true;
	};

