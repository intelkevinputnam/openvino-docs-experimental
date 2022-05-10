.. index:: pair: struct; ov::op::v6::ExperimentalDetectronDetectionOutput::Attributes
.. _doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes:

struct ov::op::v6::ExperimentalDetectronDetectionOutput::Attributes
===================================================================



Structure that specifies attributes of the operation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <experimental_detectron_detection_output.hpp>
	
	struct Attributes
	{
		// fields
	
		float :target:`score_threshold<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1af79af9f0bebb3bdc07c0d4ba24703494>`;
		float :target:`nms_threshold<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1a6f57f75e5ecbd25869b8936bcc739b78>`;
		float :target:`max_delta_log_wh<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1accaecb867c31b8d4a9b5ebd3fde1d6f5>`;
		int64_t :target:`num_classes<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1a5e567a0afa117bface05dcd0d2ee2a47>`;
		int64_t :target:`post_nms_count<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1a8ea06df53cff1de067238a6c3e2f129e>`;
		size_t :target:`max_detections_per_image<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1ace56678a814b262a6f94e260bc634ddb>`;
		bool :target:`class_agnostic_box_regression<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1aebde4a8d4c2c3dc8ef5b66c466730e94>`;
		std::vector<float> :target:`deltas_weights<doxid-structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes_1a4dc1d9c84138e11f7f7e5cf4454a9c10>`;
	};

