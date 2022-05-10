.. index:: pair: struct; ngraph::runtime::reference::CellArgs
.. _doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args:

struct ngraph::runtime::reference::CellArgs
===========================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <sequences.hpp>
	
	struct CellArgs
	{
		// fields
	
		std::string :target:`activation_f<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1a1b2353e6176ae085b0f9fba0681eeda6>`;
		std::string :target:`activation_g<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1af109fdc659a300278ae71871a2f4ee12>`;
		std::string :target:`activation_h<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1a31fa9272904c46eb8b39b9d5adea03f2>`;
		float :target:`clip<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1a6dc0bc72a85ba22d2629119994b331cd>`;
		bool :target:`linear_before_reset<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1af731f8cf8578de4f7190d111d2b3ff64>` = false;
		:ref:`ov::op::LSTMWeightsFormat<doxid-namespaceov_1_1op_1a6efe5db5f325a937a6662cd2b66e1437>` :target:`weight_format<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1a4df24c4ad40a1a4baac40b0b96017e7b>` = ov::op::LSTMWeightsFormat::FICO;
		bool :target:`input_forget<doxid-structngraph_1_1runtime_1_1reference_1_1_cell_args_1aa80108f87237dbf3f90f4ce46b0fb22c>` = false;
	};

