.. index:: pair: struct; ov::op::v8::PriorBox::Attributes
.. _doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes:

struct ov::op::v8::PriorBox::Attributes
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <prior_box.hpp>
	
	struct Attributes
	{
		// fields
	
		std::vector<float> :target:`min_size<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a2c8e1a53c528e987b3f708d6b76cca34>`;
		std::vector<float> :target:`max_size<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a89a207b288d97447439fd7a155539698>`;
		std::vector<float> :target:`aspect_ratio<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a270c2dac496f3d62f25106d41d572360>`;
		std::vector<float> :target:`density<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a7de4df6668ec9e9b948961e71f1d30df>`;
		std::vector<float> :target:`fixed_ratio<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1af3bdef2ee9fb9497331281eac0b885c7>`;
		std::vector<float> :target:`fixed_size<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a1388f33f0136150b3bdca19212f70e85>`;
		bool :target:`clip<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a5cb71a2e9c1dd17b63de1a161ccc6821>` = false;
		bool :target:`flip<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a23df66bc063d80ce9fad019a05248c89>` = false;
		float :target:`step<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1afd2c68cd65df7e4c4539c81316e69791>` = 0.0f;
		float :target:`offset<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a139650abc1d300ba6be1d5ca9e19befe>` = 0.0f;
		std::vector<float> :target:`variance<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1aab8665424b3053b18262a4d55a5e8e8d>`;
		bool :target:`scale_all_sizes<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a55043b05b31b1403f15f02855ab475f9>` = true;
		bool :target:`min_max_aspect_ratios_order<doxid-structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes_1a638c9c29a9557d4fe32abfcb1b96a185>` = true;
	};

