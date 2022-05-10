.. index:: pair: struct; ov::op::v0::PriorBoxClustered::Attributes
.. _doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes:

struct ov::op::v0::PriorBoxClustered::Attributes
================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <prior_box_clustered.hpp>
	
	struct Attributes
	{
		// fields
	
		std::vector<float> :target:`widths<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1a96cf0dca216c3ec697b302e11bc29d70>`;
		std::vector<float> :target:`heights<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1a353c10e29f3623bf2d75ed51175cc491>`;
		bool :target:`clip<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1aa5c03e40030da31a6cb95efbdb993245>` = true;
		float :target:`step_widths<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1a03e51eb32df87fc3cef54be1d721d85b>` = 0.0f;
		float :target:`step_heights<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1af83d708c6378545ee77e1b7dcf5deb5a>` = 0.0f;
		float :target:`step<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1a8ceb70304f41ab6dc67e6730cb0c876a>` = 0.0f;
		float :target:`offset<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1a37a84a98b9a475b659ee24395c397923>` = 0.0f;
		std::vector<float> :target:`variances<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes_1a4e9c05595d6002ae0342c2835150e2a6>`;
	};

