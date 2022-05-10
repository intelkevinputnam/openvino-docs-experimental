.. index:: pair: struct; ngraph::op::InterpolateIEAttrs
.. _doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs:

struct ngraph::op::InterpolateIEAttrs
=====================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interp.hpp>
	
	struct InterpolateIEAttrs
	{
		// fields
	
		int :target:`height<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1a464ced6d6b9cf998cbe42ca17ac8d67b>` = -1;
		int :target:`width<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1a0d719f01d80b4eba81ef581955ab65c0>` = -1;
		float :target:`zoom_factor<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1a4ced42f5903f813148097606ea057b3d>` = 0;
		float :target:`shrink_factor<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1aa8fbb47efde27419913e6d6289cf3f73>` = 0;
		float :target:`scale_factor<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1ad6034fbd9a44835cf9ee1eaf53185f83>` = 1.0;
		bool :target:`align_corners<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1a8c9132613d756a6077732918c0b9600f>` = true;
		bool :target:`antialias<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1a7a81143f4f6c24c29096b7c899747a89>` = true;
		std::string :target:`mode<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1a9836ab8e1e488d4a9da6e1bdb4ceab61>` = "";
		int :target:`pad_beg<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1ae7d0ecac2ff755c461bbdedaa266f5b4>` = 0;
		int :target:`pad_end<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs_1ac8874a1dc2d31c283c40afed3cd4a6a6>` = 0;
	};

