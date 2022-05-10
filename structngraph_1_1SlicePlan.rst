.. index:: pair: struct; ngraph::SlicePlan
.. _doxid-structngraph_1_1_slice_plan:

struct ngraph::SlicePlan
========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <slice_plan.hpp>
	
	struct SlicePlan
	{
		// fields
	
		std::vector<int64_t> :target:`begins<doxid-structngraph_1_1_slice_plan_1aa398978099adaea2d27539189a159201>`;
		std::vector<int64_t> :target:`ends<doxid-structngraph_1_1_slice_plan_1a2c9f07bd3ed042508df5d7483afb0b81>`;
		std::vector<int64_t> :target:`strides<doxid-structngraph_1_1_slice_plan_1a3ef9e6dd4b590c2025e296ac681ed744>`;
		Shape :target:`reshape_in_shape<doxid-structngraph_1_1_slice_plan_1a74bc68608bd5d7677f1c79d02631a89f>`;
		Shape :target:`reshape_out_shape<doxid-structngraph_1_1_slice_plan_1a2a63185b692cbcc0a55e07bfc0c67953>`;
		AxisSet :target:`reverse_axes<doxid-structngraph_1_1_slice_plan_1aa3dc52509aee71e77d020f1d18c15335>`;

		// methods
	
		bool :target:`operator ==<doxid-structngraph_1_1_slice_plan_1a84443c609a0d48227b8fc0cffad90b66>` (const SlicePlan& other) const;
		bool :target:`operator !=<doxid-structngraph_1_1_slice_plan_1ac8045838ec74c60a06240b2a4a8adb14>` (const SlicePlan& other) const;
	};

