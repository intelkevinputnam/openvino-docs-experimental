.. index:: pair: namespace; ngraph::opset1
.. _doxid-namespacengraph_1_1opset1:

namespace ngraph::opset1
========================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace opset1 {

	// global functions

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :ref:`infer_conv_backprop_auto_padding<doxid-namespacengraph_1_1opset1_1afb7779b3b0381ddda15f3fb4e12ab99b>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filters_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const op::PadType auto_pad_type,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& output_padding,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		);

	} // namespace opset1
.. _details-namespacengraph_1_1opset1:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespacengraph_1_1opset1_1afb7779b3b0381ddda15f3fb4e12ab99b:
.. index:: pair: function; infer_conv_backprop_auto_padding

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void infer_conv_backprop_auto_padding(
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filters_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const op::PadType auto_pad_type,
		const :ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& output_padding,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_begin,
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& pads_end
		)

Calculates padding values for ConvolutionBackpropData operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_data_shape

		- The input data shape.

	*
		- filters_shape

		- The filters shape.

	*
		- output_shape

		- The output shape defined only for spatial dimentions.

	*
		- strides

		- The strides values.

	*
		- dilations

		- The dilations values.

	*
		- auto_pad_type

		- The automatic padding mode.

	*
		- output_padding

		- The output padding values.

	*
		- pads_begin

		- The placeholder for paddings at the beginning of axis.

	*
		- pads_end

		- The placeholder for paddings at the end of axis.

