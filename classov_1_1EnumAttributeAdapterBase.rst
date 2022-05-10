.. index:: pair: class; ov::EnumAttributeAdapterBase
.. _doxid-classov_1_1_enum_attribute_adapter_base:

class ov::EnumAttributeAdapterBase
==================================



Overview
~~~~~~~~

Access an enum via a string. :ref:`More...<details-classov_1_1_enum_attribute_adapter_base>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <typename AT>
	class EnumAttributeAdapterBase: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// construction
	
		:target:`EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base_1ac3b5aaea5360d7ead420c8ad53f658d7>`(AT& value);

		// methods
	
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:target:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :target:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
	};

	// direct descendants

	template <>
	class :ref:`AttributeAdapter<ELTWISE_TYPE><doxid-classov_1_1_attribute_adapter_3_01_e_l_t_w_i_s_e___t_y_p_e_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ngraph::reduction::Type><doxid-classov_1_1_attribute_adapter_3_01ngraph_1_1reduction_1_1_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::AutoBroadcastType><doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::BroadcastType><doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::EpsMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1_eps_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::GeluApproximationMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1_gelu_approximation_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::LSTMWeightsFormat><doxid-classov_1_1_attribute_adapter_3_01op_1_1_l_s_t_m_weights_format_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::MVNEpsMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1_m_v_n_eps_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::PadMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::PadType><doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::RecurrentSequenceDirection><doxid-classov_1_1_attribute_adapter_3_01op_1_1_recurrent_sequence_direction_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::RoundingType><doxid-classov_1_1_attribute_adapter_3_01op_1_1_rounding_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::TopKMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::TopKSortType><doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_sort_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::util::NmsBase::SortResultType><doxid-classov_1_1_attribute_adapter_3_01op_1_1util_1_1_nms_base_1_1_sort_result_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v0::DepthToSpace::DepthToSpaceMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_depth_to_space_1_1_depth_to_space_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v0::Interpolate::InterpolateMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_interpolate_1_1_interpolate_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v0::SpaceToDepth::SpaceToDepthMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_space_to_depth_1_1_space_to_depth_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v1::BinaryConvolution::BinaryConvolutionMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_binary_convolution_1_1_binary_convolution_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v1::NonMaxSuppression::BoxEncodingType><doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_non_max_suppression_1_1_box_encoding_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v1::Reverse::Mode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_reverse_1_1_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v3::NonMaxSuppression::BoxEncodingType><doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_non_max_suppression_1_1_box_encoding_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v3::ROIAlign::PoolingMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_r_o_i_align_1_1_pooling_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v4::Interpolate::CoordinateTransformMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_coordinate_transform_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v4::Interpolate::InterpolateMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_interpolate_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v4::Interpolate::NearestMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_nearest_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v4::Interpolate::ShapeCalcMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_shape_calc_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v5::NonMaxSuppression::BoxEncodingType><doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_non_max_suppression_1_1_box_encoding_type_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v5::Round::RoundMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_round_1_1_round_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v8::MatrixNms::DecayFunction><doxid-classov_1_1_attribute_adapter_3_01op_1_1v8_1_1_matrix_nms_1_1_decay_function_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v9::ROIAlign::AlignedMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_aligned_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v9::ROIAlign::PoolingMode><doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_pooling_mode_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::element::Type_t><doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type__t_01_4>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_enum_attribute_adapter_base:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Access an enum via a string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AT

		- The attribute type enum class

Methods
-------

.. _doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& get()

Returns the value.

.. _doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const std::string& value)

Sets the value.


