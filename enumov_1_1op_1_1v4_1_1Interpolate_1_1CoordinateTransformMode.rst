.. index:: pair: enum; CoordinateTransformMode
.. _doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5:

enum ov::op::v4::Interpolate::CoordinateTransformMode
=====================================================

Overview
~~~~~~~~

Mode of the calculation of the source coordinate from resized one. :ref:`More...<details-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>

	enum CoordinateTransformMode
	{
	    :target:`HALF_PIXEL<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5a056f843a4f60fd0c1e37a469eba69b6d>`,
	    :target:`PYTORCH_HALF_PIXEL<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5ad2184537ce8c0bfdd871cb1055fc4562>`,
	    :target:`ASYMMETRIC<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5ad4cb95b2d550c20b06f46e10d4c7c7b2>`,
	    :target:`TF_HALF_PIXEL_FOR_NN<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5af115dccd0185ea5104aa1cd328ed4d20>`,
	    :target:`ALIGN_CORNERS<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5a61382f48a544456b2447c1649c399a68>`,
	    :target:`OPENVINO_ENUM_DEPRECATED<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5a818ab456ff0423396ee6fd069cc2396b>` =("Please use ALIGN_CORNERS instead") = ALIGN_CORNERS,
	};

.. _details-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Mode of the calculation of the source coordinate from resized one.

These modes are modes from ONNX runtime.

