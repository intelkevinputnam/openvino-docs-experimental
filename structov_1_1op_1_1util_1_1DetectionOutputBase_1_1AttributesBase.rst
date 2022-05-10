.. index:: pair: struct; ov::op::util::DetectionOutputBase::AttributesBase
.. _doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base:

struct ov::op::util::DetectionOutputBase::AttributesBase
========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <detection_output_base.hpp>
	
	struct AttributesBase
	{
		// fields
	
		int :ref:`background_label_id<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a8d6da689063467435a960287a32f5de5>` = 0;
		int :ref:`top_k<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1ab5f5cf9ce2edc2e17ca479ad5df97984>` = -1;
		bool :ref:`variance_encoded_in_target<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1ab489c56fdb235c90ccc2bae71a209e09>` = false;
		std::vector<int> :ref:`keep_top_k<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a2f54d2ee28ede0cf43f783e56a66b8da>`;
		std::string :ref:`code_type<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a7ff8ddabc345bc7c5f704547718de67e>` = std::string{"caffe.PriorBoxParameter.CORNER"};
		bool :ref:`share_location<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1ada1b5ef0c2b33bc7f0a1583d029260c7>` = true;
		float :ref:`nms_threshold<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1aa95ae128818768403f3d44fe39b94b79>`;
		float :ref:`confidence_threshold<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a32d5b2e00b5ac000efa6ff966d12d66d>` = 0;
		bool :ref:`clip_after_nms<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a79268d2fc9332f699baa381b794fe46b>` = false;
		bool :ref:`clip_before_nms<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1aead066a4a78c7f092686602bb934c02e>` = false;
		bool :ref:`decrease_label_id<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1af13b4f7d73228faee9d835b67a1aafb5>` = false;
		bool :ref:`normalized<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a523f49613ed20c991f4a0744900385fa>` = false;
		size_t :ref:`input_height<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1ae256bbaf98bcb2ecd21d173a34eb44a2>` = 1;
		size_t :ref:`input_width<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a498b6c2ca2a036da1b1ffd5b4b53a25c>` = 1;
		float :ref:`objectness_score<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base_1a4fa9050715b51015665fb23ca2f01225>` = 0;
	};

	// direct descendants

	struct :ref:`Attributes<doxid-structov_1_1op_1_1v0_1_1_detection_output_1_1_attributes>`;

