.. index:: pair: struct; ov::op::v0::PriorBox::Attributes
.. _doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes:

struct ov::op::v0::PriorBox::Attributes
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <prior_box.hpp>
	
	struct Attributes
	{
		// fields
	
		std::vector<float> :target:`min_size<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1accd48151dd44251520c712d1201325e9>`;
		std::vector<float> :target:`max_size<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a2866c1ab738c3ba4c3d9b864ebeb9faf>`;
		std::vector<float> :target:`aspect_ratio<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1ae2f0558bdc4e1979c84db80bb7e63a23>`;
		std::vector<float> :target:`density<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a74f2a25202d98e1a9c9deb50209d8bcc>`;
		std::vector<float> :target:`fixed_ratio<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a5f89b7ed3abfbc28a48a9314a9f50e09>`;
		std::vector<float> :target:`fixed_size<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1af3b38e77d76f0c2547608a1d0ffd0c3d>`;
		bool :target:`clip<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a5940b98966e387018245bea502075899>` = false;
		bool :target:`flip<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1ab2308810da2a1c523ddb92c8657cbd44>` = false;
		float :target:`step<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a285bcbe1efd20cdb3b44fac876582379>` = 0.0f;
		float :target:`offset<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a1e9925ecf640c0f8d661f7222aee2371>` = 0.0f;
		std::vector<float> :target:`variance<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1a5ecca0116023719b8a38b31b64cbef4e>`;
		bool :target:`scale_all_sizes<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes_1aba339daa2c5a054dd22a24ba00f48a5b>` = true;
	};

