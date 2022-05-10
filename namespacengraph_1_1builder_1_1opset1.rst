.. index:: pair: namespace; ngraph::builder::opset1
.. _doxid-namespacengraph_1_1builder_1_1opset1:

namespace ngraph::builder::opset1
=================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace opset1 {

	// global functions

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`legacy_broadcast_for_binary_operation<doxid-namespacengraph_1_1builder_1_1opset1_1adedabc91eca8e5fd43e2c53db956f801>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& left,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& right,
		size_t start_match_axis
		);

	std::vector<std::size_t> :ref:`get_axes_mapping<doxid-namespacengraph_1_1builder_1_1opset1_1a6618a57d633a7f33b318165df225e85c>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& broadcast_axes
		);

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_axes_mapping_output<doxid-namespacengraph_1_1builder_1_1opset1_1a759eeb2305b3246a9727884fd8180051>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		std::size_t start_match_axis
		);

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_axes_mapping_output<doxid-namespacengraph_1_1builder_1_1opset1_1a1c1538b173810973393a05eeeb507e11>`(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& output_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		std::size_t start_match_axis
		);

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_axes_mapping_output<doxid-namespacengraph_1_1builder_1_1opset1_1ae21d20d651794d9eda9590bb17f7797c>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& broadcast_axes
		);

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_broadcast<doxid-namespacengraph_1_1builder_1_1opset1_1a49271e00a4204ccfdaf54b28f86c5b32>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`Shape<doxid-classov_1_1_shape>`& target_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& broadcast_axes
		);

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_broadcast<doxid-namespacengraph_1_1builder_1_1opset1_1a9366b123e4a356c99b9f40ba04f32571>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`Shape<doxid-classov_1_1_shape>`& target_shape,
		std::size_t start_match_axis
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`l0_norm<doxid-namespacengraph_1_1builder_1_1opset1_1a72f44079cb35ff4887efae41833b9b46>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		bool keep_dims = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`l1_norm<doxid-namespacengraph_1_1builder_1_1opset1_1a28cb637093688d5d17ea247629049bc1>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		float bias = 0.f,
		bool keep_dims = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`l2_norm<doxid-namespacengraph_1_1builder_1_1opset1_1a503c12746fa049fecba22ea04139167d>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		float bias = 0.f,
		:ref:`BiasMode<doxid-namespacengraph_1_1builder_1a1f3571bec2116a0c8e76cf6c9dbf003d>` bias_mode = BiasMode::ADD,
		bool keep_dims = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`lp_norm<doxid-namespacengraph_1_1builder_1_1opset1_1a5c60bd789d580bd57f126aa6a886cb7d>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		std::size_t p_norm = 2,
		float bias = 0.f,
		bool keep_dims = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`mean<doxid-namespacengraph_1_1builder_1_1opset1_1a3377b4f15f56daf79c96a94ccefdb489>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes,
		bool keep_dims = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`mean<doxid-namespacengraph_1_1builder_1_1opset1_1ae0a4c4274f3e2a42d1fac8d8f6a01474>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		bool keep_dims = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`variance<doxid-namespacengraph_1_1builder_1_1opset1_1a1bc1e531b299d3bf5b7ad6f685b7dec4>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes,
		const bool bessel_correction = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`variance<doxid-namespacengraph_1_1builder_1_1opset1_1a5cc7a6d7554a3244ffeada5f3183d371>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		bool keep_dims = false,
		bool bessel_correction = false
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`reshape<doxid-namespacengraph_1_1builder_1_1opset1_1ae436bb386fa882348f9a2a15148af42d>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`reorder_axes<doxid-namespacengraph_1_1builder_1_1opset1_1ae29aecf49318edb54d0c5dd3d586d3a5>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		std::vector<size_t> axes_order = {}
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`transpose<doxid-namespacengraph_1_1builder_1_1opset1_1ae0ce58415f5474a2b293ee74b6d09c40>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value);
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`flatten<doxid-namespacengraph_1_1builder_1_1opset1_1aca36aea320567ef288c2d7b3a16cb4ac>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value, int axis);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`expand_dims<doxid-namespacengraph_1_1builder_1_1opset1_1a036e6503cefa6acc4eddc22cc85feeb7>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		std::size_t axis = 0
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`squeeze<doxid-namespacengraph_1_1builder_1_1opset1_1a3862232fd4fbc3fcaa73046b41d57422>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		std::vector<std::size_t> axes = {0}
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`collapse<doxid-namespacengraph_1_1builder_1_1opset1_1a3fde35d6ea5ba9f863eaa417867fe07a>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const std::size_t start_axis,
		const std::size_t end_axis
		);

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`split<doxid-namespacengraph_1_1builder_1_1opset1_1a380c96c4f6bf6cacc0fc37bbd0f06c06>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const std::vector<int64_t>& split_lengths,
		int64_t axis = 0
		);

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`split<doxid-namespacengraph_1_1builder_1_1opset1_1acbe2cc7594996544480d9a80e2ff6705>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		int64_t num_splits,
		int64_t axis = 0
		);

	} // namespace opset1
.. _details-namespacengraph_1_1builder_1_1opset1:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespacengraph_1_1builder_1_1opset1_1adedabc91eca8e5fd43e2c53db956f801:
.. index:: pair: function; legacy_broadcast_for_binary_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> legacy_broadcast_for_binary_operation(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& left,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& right,
		size_t start_match_axis
		)

Broadcast right node to left node's shape using legacy scheme.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left

		- The left hand side node of binary operation.

	*
		- right

		- The right hand side node of binary operation. The one to be broadcasted.

	*
		- start_match_axis

		- The axis index starting mutually equal shapes of both nodes.



.. rubric:: Returns:

The Output object connected to node producing broadcasted right node.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a6618a57d633a7f33b318165df225e85c:
.. index:: pair: function; get_axes_mapping

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::size_t> get_axes_mapping(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& broadcast_axes
		)

Reconstructs axes mapping vector for Broadcast:v1 operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_shape

		- The output shape of Broadcast operation.

	*
		- broadcast_axes

		- The broadcast axes used for Broadcast:v0 operator.



.. rubric:: Returns:

The vector with axes indexes mapping .

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a759eeb2305b3246a9727884fd8180051:
.. index:: pair: function; get_axes_mapping_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_axes_mapping_output(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		std::size_t start_match_axis
		)

Creates Node returning the axes mapping for Broadcast:v1 operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_shape

		- The output shape of Broadcast operation.

	*
		- input_shape

		- The input shape.

	*
		- start_match_axis

		- The axis index at which input shape starts to be identical as the output shape.



.. rubric:: Returns:

Returns the Output object pointing to node with the axes mapping.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a1c1538b173810973393a05eeeb507e11:
.. index:: pair: function; get_axes_mapping_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_axes_mapping_output(
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& output_shape,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& input_shape,
		std::size_t start_match_axis
		)

Creates Node returning the axes mapping for Broadcast operation.

Shapes' ranks need to be static.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_shape

		- The output shape of Broadcast operation.

	*
		- input_shape

		- The input shape.

	*
		- start_match_axis

		- The axis index at which input shape starts to be identical to consecutive subset of output shape dimensions.



.. rubric:: Returns:

Returns the Output object pointing to node with the axes mapping.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1ae21d20d651794d9eda9590bb17f7797c:
.. index:: pair: function; get_axes_mapping_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_axes_mapping_output(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& broadcast_axes
		)

Creates Node returning the axes mapping for Broadcast:v1 operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_shape

		- The output shape of Broadcast operation.

	*
		- broadcast_axes

		- The broadcast axes used for Broadcast:v0 operator.



.. rubric:: Returns:

The Output object with Node returning axes mapping.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a72f44079cb35ff4887efae41833b9b46:
.. index:: pair: function; l0_norm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> l0_norm(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		bool keep_dims = false
		)

Calculates L-0 norm of input tensor.

The L-0 norm represents the cardinality of elements different from zero. This actually is not a "true" norm.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The input tensor.

	*
		- reduction_axes

		- The axes along which we calculate norm.

	*
		- keep_dims

		- The flag indicates if axes will be removed or kept.



.. rubric:: Returns:

L-0 norm of value. The output sub-graph is composed of v1 ops.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a28cb637093688d5d17ea247629049bc1:
.. index:: pair: function; l1_norm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> l1_norm(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		float bias = 0.f,
		bool keep_dims = false
		)

Calculates L-1 norm of a value.

The L-1 norm represents the sum of absolute values.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The input tensor.

	*
		- reduction_axes

		- The axes along which we calculate norm.

	*
		- bias

		- The bias added to the calculated sum.

	*
		- keep_dims

		- The flag indicates if axes will be removed or kept.



.. rubric:: Returns:

L-1 norm of value. The output sub-graph is composed of v1 ops.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a503c12746fa049fecba22ea04139167d:
.. index:: pair: function; l2_norm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> l2_norm(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		float bias = 0.f,
		:ref:`BiasMode<doxid-namespacengraph_1_1builder_1a1f3571bec2116a0c8e76cf6c9dbf003d>` bias_mode = BiasMode::ADD,
		bool keep_dims = false
		)

Calculates L-2 norm of input tensor.

The L-2 norm represents the square root of sum of squares of each individual element.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The input tensor.

	*
		- reduction_axes

		- The axes along which we calculate norm.

	*
		- bias

		- The bias combined with calculated sum.

	*
		- bias_mode

		- The method of bias application.

	*
		- keep_dims

		- The flag indicates if axes will be removed or kept.



.. rubric:: Returns:

L-2 norm of value. The output sub-graph is composed of v1 ops.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a5c60bd789d580bd57f126aa6a886cb7d:
.. index:: pair: function; lp_norm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> lp_norm(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& reduction_axes,
		std::size_t p_norm = 2,
		float bias = 0.f,
		bool keep_dims = false
		)

Creates node which calculates L-p norm on input tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The input tensor.

	*
		- reduction_axes

		- The axes along which we calculate norm.

	*
		- p_norm

		- The p norm to calculate.

	*
		- bias

		- The bias added to the calculated sum.

	*
		- keep_dims

		- The flag indicates if axes will be removed or kept.



.. rubric:: Returns:

L-p norm of value. The output sub-graph is composed of v1 ops.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a3377b4f15f56daf79c96a94ccefdb489:
.. index:: pair: function; mean

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> mean(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes,
		bool keep_dims = false
		)

Sum-based Mean of a Tensor.

Calculates

:math:`\sum_{i=1}^{N} \frac{x_i}{N}`

Where ``i`` traverses all of the axes provided in ``reduction_axes``

Inputs
------

| | Type | Description | | | ------------- | ------------------------------ | ---------------------------------------------------- | | ``node`` | :math:`E[d_1,\dots,d_n]~(n \geq 0)` | An input tensor of any shape | | ``reduction_axes`` | AxesSet | The axes to eliminate through reduction (0 indexed). | | ``keep_dims`` | bool | If set to true it holds reduced axes. |

Output
------

.. list-table::
    :header-rows: 1

    * - Type
      - Description
    * - :math:`E[\textit{delete}(A,d_1,\dots,d_n)]`
      - The tensor :math:`T` , where :math:`T` is the input tensor with the ``reduction_axes`` :math:`A` eliminated by reduction.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a1bc1e531b299d3bf5b7ad6f685b7dec4:
.. index:: pair: function; variance

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> variance(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`AxisSet<doxid-classov_1_1_axis_set>`& reduction_axes,
		const bool bessel_correction = false
		)

Sum-based Variance of a Tensor.

If bessel_correct is true, calculates

:math:`\frac{\sum_{i=1}^{N}\left(x_i-\bar{x}\right)^2}{N-1}`

else, calculates

:math:`\frac{\sum_{i=1}^{N}\left(x_i-\bar{x}\right)^2}{N}`

Where ``i`` traverses all of the axes provided in ``reduction_axes`` and :math:`\bar{x} = \sum_{i=1}^{N} \frac{x_i}{N}`

Inputs
------

.. list-table::
    :header-rows: 1

    * - 
      - Type
      - Description
    * - ``value\ilinebr </td> <td class="markdownTableBodyNone"> \f$E[d_1,\dots,d_n]~(n \geq 0)\f$\ilinebr </td> <td class="markdownTableBodyNone"> An input tensor of any shape\ilinebr </td> </tr> <tr class="markdownTableRowEven"> <td class="markdownTableBodyNone">`` reduction_axes ``\ilinebr </td> <td class="markdownTableBodyNone"> AxesSet\ilinebr </td> <td class="markdownTableBodyNone"> The axes to eliminate through reduction (0 indexed).\ilinebr </td> </tr> <tr class="markdownTableRowOdd"> <td class="markdownTableBodyNone">`` bessel_correction`
      - bool (default = false)
      - Enable Bessel's correction to std_dev for Small sample sizes

Output
------

.. list-table::
    :header-rows: 1

    * - Type
      - Description
    * - :math:`E[\textit{delete}(A,d_1,\dots,d_n)]`
      - The tensor :math:`T` , where :math:`T` is the input tensor with the ``reduction_axes`` :math:`A` eliminated by reduction.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1ae436bb386fa882348f9a2a15148af42d:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> reshape(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value, const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

Change shape of a value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to be reshaped.

	*
		- shape

		- The new shape.



.. rubric:: Returns:

Reshape:v1 op.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1ae29aecf49318edb54d0c5dd3d586d3a5:
.. index:: pair: function; reorder_axes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> reorder_axes(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		std::vector<size_t> axes_order = {}
		)

Permute axes according to specified axes_order parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- The

		- vlaue whose axes we want to permute.

	*
		- axes_order

		- The permutation of axes.



.. rubric:: Returns:

Transpose:v1 op.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1ae0ce58415f5474a2b293ee74b6d09c40:
.. index:: pair: function; transpose

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> transpose(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value)

Return transposed value (with axes in reversed order).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Value

		- to transpose.



.. rubric:: Returns:

Transpose:v1 op.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1aca36aea320567ef288c2d7b3a16cb4ac:
.. index:: pair: function; flatten

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> flatten(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value, int axis)

Flatten a value into a 2D matrix, with a static dividing axis.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- The

		- tensor to be flattened.

	*
		- The

		- axis dividing shape.



.. rubric:: Returns:

The new value will be a 2D matrix representing the flattened input node.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a036e6503cefa6acc4eddc22cc85feeb7:
.. index:: pair: function; expand_dims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> expand_dims(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		std::size_t axis = 0
		)

Expands node tensor shape with empty axis at specified position.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to be expanded.

	*
		- axis

		- The position in the expanded axes where the new axis is placed.



.. rubric:: Returns:

Reshape:v1 op.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a3862232fd4fbc3fcaa73046b41d57422:
.. index:: pair: function; squeeze

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> squeeze(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		std::vector<std::size_t> axes = {0}
		)

Remove empty axes from input tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to be squeezed.

	*
		- axes

		- The vector defining indexes of axes to be removed.



.. rubric:: Returns:

Reshape:v1 op.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a3fde35d6ea5ba9f863eaa417867fe07a:
.. index:: pair: function; collapse

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> collapse(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const std::size_t start_axis,
		const std::size_t end_axis
		)

Collapse specified axes into single one.

Collapsed axes create a continuous range starting from outermost axis.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to be reshaped.

	*
		- start_axis

		- The start axis index.

	*
		- end_axis

		- The end axis (inclusive) index.



.. rubric:: Returns:

The node with collapsed specified axes.

.. _doxid-namespacengraph_1_1builder_1_1opset1_1a380c96c4f6bf6cacc0fc37bbd0f06c06:
.. index:: pair: function; split

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` split(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const std::vector<int64_t>& split_lengths,
		int64_t axis = 0
		)

Split value on specified axis into multiple parts.

This implementation supports negative ``axis`` values (similar to NumPy indexing). This means that the axis to split on will be counted from the back of the tensor (negative values are subtracted from its rank).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to be split.

	*
		- split_lengths

		- The vector defining the lengths of each split part.

	*
		- axis

		- The axis we split input node on. Default value is zero axis.



.. rubric:: Returns:

The vector containing multiple outputs we split input node into. The vector is output of Split:v1 op

.. _doxid-namespacengraph_1_1builder_1_1opset1_1acbe2cc7594996544480d9a80e2ff6705:
.. index:: pair: function; split

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` split(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		int64_t num_splits,
		int64_t axis = 0
		)

Split value on specified axis into multiple parts.

This implementation supports negative ``axis`` values (similar to NumPy indexing). This means that the axis to split on will be counted from the back of the tensor (negative values are subtracted from its rank).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to split.

	*
		- num_splits

		- The number of parts we want to split output at given axis. The length of the axis to split must be divisible by this value.

	*
		- axis

		- The axis we split input node on. Default value is zero axis.



.. rubric:: Returns:

The vector containing multiple nodes we split input node into. The vector is output of VariadicSplit:v1 op

