.. index:: pair: enum; NearestMode
.. _doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2:

enum ov::op::v4::Interpolate::NearestMode
=========================================

Round modes for the nearest interpolation.

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>

	enum NearestMode
	{
	    :target:`ROUND_PREFER_FLOOR<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a288b312c0705906c0939746e0a1a8928>`,
	    :target:`ROUND_PREFER_CEIL<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a396bd6da7c7ee7235973d332fabe6e28>`,
	    :target:`FLOOR<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a56c1e354d36beb85b0d881c5b2e24cbe>`,
	    :target:`CEIL<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a5bdce8e6d9dc3efbbd31e90a8a181dff>`,
	    :target:`SIMPLE<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2ae5564829e2f85f6a6873a9d5c4f26d09>`,
	    :target:`OPENVINO_ENUM_DEPRECATED<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2a818ab456ff0423396ee6fd069cc2396b>` =("Please use SIMPLE instead") = SIMPLE,
	};

