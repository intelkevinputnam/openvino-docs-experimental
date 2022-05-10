.. index:: pair: struct; ngraph::runtime::reference::InterpolateEvalHelper::InfoForGenericLinearONNXMode
.. _doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode:

struct ngraph::runtime::reference::InterpolateEvalHelper::InfoForGenericLinearONNXMode
======================================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	struct InfoForGenericLinearONNXMode
	{
		// fields
	
		int64_t :target:`input_data_ptr_increment<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a1e991fa01e74da2a1bfb34e49e65a5ab>`;
		int64_t :target:`output_data_ptr_increment<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a844caea2f741513480b27f45bf8621c2>`;
		int64_t :target:`batch_size<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a4eaa16bae8a6ce702e5b285278886027>`;
		int64_t :target:`num_channels<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a69b14bf4e4d39302dad6e2a55d5c5b30>`;
		int64_t :target:`spatial_rank<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a9f53fe9fd53f72c4f4071d5e49e5f36b>`;
		std::vector<int64_t> :target:`input_index_multipliers<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a0be8bdc16b30437f3ee8001e00221a56>`;
		std::vector<int64_t> :target:`output_index_multipliers<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1adc248252cbc0a75dde65f0762a80aa90>`;
		std::vector<int64_t> :target:`input_spatial_shape<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1aeb721c03107bfbf2eefe5d6bd28b98b4>`;
		std::vector<int64_t> :target:`output_spatial_shape<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode_1a23b2516ac3eef576787209ad818beed1>`;
	};

