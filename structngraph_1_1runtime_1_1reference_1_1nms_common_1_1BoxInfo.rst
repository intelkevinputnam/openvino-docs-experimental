.. index:: pair: struct; ngraph::runtime::reference::nms_common::BoxInfo
.. _doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info:

struct ngraph::runtime::reference::nms_common::BoxInfo
======================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <nms_common.hpp>
	
	struct BoxInfo
	{
		// fields
	
		:ref:`Rectangle<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_rectangle>` :target:`box<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a97c92904cf6b94b6b1cd51530c2b1834>`;
		int64_t :target:`index<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a1965fae7ae1a61892153c78db5648162>` = 0;
		int64_t :target:`suppress_begin_index<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a630c1721a25f67971ec8dd9d5a7ba6e2>` = 0;
		int64_t :target:`batch_index<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a54e621a4f9c35a7fb7ddd8f28db9a47f>` = 0;
		int64_t :target:`class_index<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1ab7b370fcca7b57e9041dfb4a3bbb1a9d>` = 0;
		float :target:`score<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a6e9bbf3fdb2a96372781bbbff9a9d544>` = 0.0f;

		// construction
	
		:target:`BoxInfo<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1ae9b0e473816c6cca23aa26a76b37a59b>`(
			const :ref:`Rectangle<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_rectangle>`& r,
			int64_t idx,
			float sc,
			int64_t suppress_idx,
			int64_t batch_idx,
			int64_t class_idx
			);
	
		:target:`BoxInfo<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a7ab1138b01ae10d3a145c7b8df267a6b>`();

		// methods
	
		bool :target:`operator <<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1a12b765f8241e9b1065bfe9fb7a58bc9e>` (const BoxInfo& rhs) const;
		bool :target:`operator ><doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info_1ab5b474c3f22c3534e5cfb91f162a9e1f>` (const BoxInfo& rhs) const;
	};

