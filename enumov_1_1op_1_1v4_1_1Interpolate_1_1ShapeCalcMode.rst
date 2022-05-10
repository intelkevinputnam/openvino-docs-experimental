.. index:: pair: enum; ShapeCalcMode
.. _doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa:

enum ov::op::v4::Interpolate::ShapeCalcMode
===========================================

Overview
~~~~~~~~

:ref:`PartialShape <doxid-classov_1_1_partial_shape>` calculation mode. :ref:`More...<details-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>

	enum ShapeCalcMode
	{
	    :target:`SIZES<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faaa5e1cef30159d9dc7c0ac211aeb17dc74>`,
	    :target:`SCALES<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faaaa7ba06a3b4388996427890e9889c72c0>`,
	    :target:`OPENVINO_ENUM_DEPRECATED<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faaa818ab456ff0423396ee6fd069cc2396b>` =("Please use SCALES instead") = SCALES,
	};

.. _details-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`PartialShape <doxid-classov_1_1_partial_shape>` calculation mode.

sizes - output shape for interpolated axes is calculated using input ``sizes`` scales - output shape for interpolated axes is calculated using input ``scales``

