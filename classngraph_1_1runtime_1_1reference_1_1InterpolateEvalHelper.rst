.. index:: pair: class; ngraph::runtime::reference::InterpolateEvalHelper
.. _doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper:

class ngraph::runtime::reference::InterpolateEvalHelper
=======================================================

.. toctree::
	:hidden:

	ICoords <structngraph_1_1runtime_1_1reference_1_1InterpolateEvalHelper_1_1ICoords.rst>
	InfoForGenericLinearONNXMode <structngraph_1_1runtime_1_1reference_1_1InterpolateEvalHelper_1_1InfoForGenericLinearONNXMode.rst>
	InfoForLinearMode <structngraph_1_1runtime_1_1reference_1_1InterpolateEvalHelper_1_1InfoForLinearMode.rst>
	LinearModeInnerIterationResult <structngraph_1_1runtime_1_1reference_1_1InterpolateEvalHelper_1_1LinearModeInnerIterationResult.rst>

Helper class to implent non-template parts of the interpolation calculation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	class InterpolateEvalHelper
	{
	public:
		// structs
	
		struct :ref:`ICoords<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_i_coords>`;
		struct :ref:`InfoForGenericLinearONNXMode<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode>`;
		struct :ref:`InfoForLinearMode<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_linear_mode>`;
		struct :ref:`LinearModeInnerIterationResult<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_linear_mode_inner_iteration_result>`;

		// construction
	
		:target:`InterpolateEvalHelper<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1aa7124f934773a75a577e5a5ff7eca05a>`();
	
		:target:`InterpolateEvalHelper<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a8690adc2ca72b8ac3ea58407dd528812>`(
			const :ref:`op::v4::Interpolate::InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs>`& attrs,
			const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
			const std::vector<int64_t>& axes,
			const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
			const std::vector<float>& scales
			);

		// methods
	
		float :target:`triangle_coeff<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a3874d4c9690a28eecc9814832efaa9ef>`(float dz);
		std::array<float, 4> :target:`get_cubic_coeff<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a9abe3c3d37d1b333ed34ab899da047bc>`(float s, float a);
		float :target:`get_in_coord<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a299c56b199a5f82405d5ceddbf60daa3>`(float coord, int64_t axis_idx);
		:ref:`Coordinate<doxid-classov_1_1_coordinate>` :target:`get_input_coords_for_nearest_mode<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1aabb09f43a10a669027ce1b4b961e89c2>`(const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& output_coord);
		:ref:`InfoForGenericLinearONNXMode<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_generic_linear_o_n_n_x_mode>` :target:`get_info_for_generic_linear_onnx<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a4e24d423b1f5eb31164f4bac4cd5df9b>`();
		:ref:`InfoForLinearMode<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_linear_mode>` :target:`get_info_for_linear_mode<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a7ba8312c26eba4f26f102f66e46bae09>`();
		:ref:`ICoords<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_i_coords>` :target:`get_icoords<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a5af66bfce8c5887a479036c0a043c5eb>`(const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& output_coord);
	
		:ref:`LinearModeInnerIterationResult<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_linear_mode_inner_iteration_result>` :target:`inner_calculation<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1a04dfbbfb472556095642afd8fa0b948f>`(
			const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& output_coord,
			const :ref:`ICoords<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_i_coords>`& icoords_data,
			const :ref:`InfoForLinearMode<doxid-structngraph_1_1runtime_1_1reference_1_1_interpolate_eval_helper_1_1_info_for_linear_mode>`& info,
			const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& index
			);
	};

