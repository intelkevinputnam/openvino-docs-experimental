.. index:: pair: struct; ov::op::v0::Proposal::Attributes
.. _doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes:

struct ov::op::v0::Proposal::Attributes
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <proposal.hpp>
	
	struct Attributes
	{
		// fields
	
		size_t :ref:`base_size<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a37b9eab2a4780b7d48b177bf6e100a1c>`;
		size_t :ref:`pre_nms_topn<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1ad9c730a716ea73a5aea1c047745a306b>`;
		size_t :ref:`post_nms_topn<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1ae77af0f764ba2f7a86b121c23437e0ff>`;
		float :ref:`nms_thresh<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a5e6be5b89a0d530174b6f95fe1f4e05b>` = 0.0f;
		size_t :ref:`feat_stride<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a263d85583f8481bceb5bd9d07642947d>` = 1;
		size_t :ref:`min_size<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a574b006bec3db81a9c6e00deee05f950>` = 1;
		std::vector<float> :ref:`ratio<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a77137eacc96b71f1553669a71122a8f0>`;
		std::vector<float> :ref:`scale<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1adf607f6aa014040eef31b83c8d837309>`;
		bool :ref:`clip_before_nms<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a2efd0b4b5a29945be4e5409fdf688b41>` = true;
		bool :ref:`clip_after_nms<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a7560f12edfefdab12f7079e515fe860f>` = false;
		bool :ref:`normalize<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a5b0b467dd07d805d5546c88853a4a57b>` = false;
		float :ref:`box_size_scale<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a7d86e20a7f68eddfda7bb04419e0962c>` = 1.0f;
		float :ref:`box_coordinate_scale<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1aab5e888382ed051228300b68f219c546>` = 1.0f;
		std::string :ref:`framework<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a55e8d19544a465c0be2ce47b27bbf606>`;
		bool :ref:`infer_probs<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes_1a6e3721c419753686453394c6a039978c>` = false;
	};

