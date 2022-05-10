.. index:: pair: struct; ov::op::v4::Interpolate::InterpolateAttrs
.. _doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs:

struct ov::op::v4::Interpolate::InterpolateAttrs
================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	struct InterpolateAttrs
	{
		// fields
	
		:ref:`InterpolateMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1a567d8870044804dc59d6d6e3df290da7>` :target:`mode<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1ac5527a985886a49eacf4106da2cb7228>` = :ref:`InterpolateMode::NEAREST<doxid-classov_1_1op_1_1v4_1_1_interpolate_1a567d8870044804dc59d6d6e3df290da7aad135772d7cf93dd0ccf9d2474b34e6a>`;
		:ref:`ShapeCalcMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa>` :target:`shape_calculation_mode<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1aae71f8013a8ac072ffa56897710146f4>` = :ref:`ShapeCalcMode::SIZES<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faaa5e1cef30159d9dc7c0ac211aeb17dc74>`;
		std::vector<size_t> :target:`pads_begin<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a38986f0b1fd0df463cb8a3afa6c7923a>`;
		std::vector<size_t> :target:`pads_end<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a2953e42c84a93efa86d265ff9bf775be>`;
		:ref:`CoordinateTransformMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>` :target:`coordinate_transformation_mode<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a4e620563bfa9ccde4f31cb0889d3d7cf>` = :ref:`CoordinateTransformMode::HALF_PIXEL<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5a056f843a4f60fd0c1e37a469eba69b6d>`;
		:ref:`NearestMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>` :target:`nearest_mode<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a0f5408ad57d99ee495666fe4d01baff4>` = :ref:`NearestMode::ROUND_PREFER_FLOOR<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a288b312c0705906c0939746e0a1a8928>`;
		bool :target:`antialias<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a9ec11a1a75d904ed1185ffa9f3525f90>` = false;
		double :target:`cube_coeff<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a0930a5769530b57f338b88e573acf60b>` = -0.75f;

		// construction
	
		:target:`InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a3b110d973f672f506e13e16f5993d5b4>`();
	
		:target:`InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a32f3fac4a3e5be43c059e9d0e6ccd04e>`(
			:ref:`InterpolateMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1a567d8870044804dc59d6d6e3df290da7>` mode,
			:ref:`ShapeCalcMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa>` shape_calculation_mode,
			const std::vector<size_t>& pads_begin,
			const std::vector<size_t>& pads_end,
			:ref:`CoordinateTransformMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>` coordinate_transformation_mode = :ref:`CoordinateTransformMode::HALF_PIXEL<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5a056f843a4f60fd0c1e37a469eba69b6d>`,
			:ref:`NearestMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>` nearest_mode = :ref:`NearestMode::ROUND_PREFER_FLOOR<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a288b312c0705906c0939746e0a1a8928>`,
			bool antialias = false,
			double cube_coeff = -0.75
			);

		// methods
	
		bool :target:`operator ==<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1ad384d907fc03da511188c0ce30a081bc>` (const InterpolateAttrs& other) const;
		bool :target:`operator !=<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs_1a1a1f217acca9ce48d5ced254582d06b4>` (const InterpolateAttrs& other) const;
	};

