.. index:: pair: enum; ColorConversion
.. _doxid-classov_1_1op_1_1util_1_1_convert_color_n_v12_base_1afbdb3631faab232fb42d01ff83c5573b:

enum ov::op::util::ConvertColorNV12Base::ColorConversion
========================================================

Exact conversion format details Currently supports conversion from NV12 to RGB or BGR, in future can be extended with NV21_to_RGBA/BGRA, etc.

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <convert_color_nv12_base.hpp>

	enum ColorConversion
	{
	    :target:`NV12_TO_RGB<doxid-classov_1_1op_1_1util_1_1_convert_color_n_v12_base_1afbdb3631faab232fb42d01ff83c5573ba155b9aa0f0c773510db05521da6ecb7c>` = 0,
	    :target:`NV12_TO_BGR<doxid-classov_1_1op_1_1util_1_1_convert_color_n_v12_base_1afbdb3631faab232fb42d01ff83c5573ba1c1d62de292c6ce13f6e8808cf52641d>` = 1,
	};

