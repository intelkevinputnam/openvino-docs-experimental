.. index:: pair: struct; ov::op::v0::Interpolate::Attributes
.. _doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes:

struct ov::op::v0::Interpolate::Attributes
==========================================



Structure that specifies attributes for interpolation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	struct Attributes
	{
		// fields
	
		:ref:`AxisSet<doxid-classov_1_1_axis_set>` :target:`axes<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes_1a497e382cd7e30f412d6ec9b5545af731>`;
		std::string :target:`mode<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes_1a404eafc93f626a2622c9ef2a58c02b72>`;
		bool :target:`align_corners<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes_1a05c9296a04a715a3e15fe2ace15cbc3b>` = true;
		bool :target:`antialias<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes_1a9d21435a66b3a906c1281868f334e2b4>` = false;
		std::vector<size_t> :target:`pads_begin<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes_1ae9f3588b01254d8123a33c2d2b127a0c>`;
		std::vector<size_t> :target:`pads_end<doxid-structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes_1a1c0b35b07c258353df187eb9be0e6519>`;
	};

