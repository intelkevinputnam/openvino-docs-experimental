.. index:: pair: namespace; ngraph::builder
.. _doxid-namespacengraph_1_1builder:

namespace ngraph::builder
=========================

.. toctree::
	:hidden:

	opset1 <namespacengraph_1_1builder_1_1opset1.rst>
	BiasMode <enumngraph_1_1builder_1_1BiasMode.rst>
	numpy_autobroadcast_incompatible_shapes <classngraph_1_1builder_1_1numpy_autobroadcast_incompatible_shapes.rst>

Overview
~~~~~~~~

Convenience functions that create addional graph nodes to implement commonly-used recipes, for example auto-broadcast. :ref:`More...<details-namespacengraph_1_1builder>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace builder {

	// namespaces

	namespace :ref:`ngraph::builder::opset1<doxid-namespacengraph_1_1builder_1_1opset1>`;

	// enums

	enum :ref:`BiasMode<doxid-namespacengraph_1_1builder_1a1f3571bec2116a0c8e76cf6c9dbf003d>`;

	// classes

	class :ref:`numpy_autobroadcast_incompatible_shapes<doxid-classngraph_1_1builder_1_1numpy__autobroadcast__incompatible__shapes>`;

	// global functions

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`numpy_broadcast_outputs<doxid-namespacengraph_1_1builder_1a96067407196af3eea5ac9eac6c4f0367>`(const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& values);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`numpy_broadcast<doxid-namespacengraph_1_1builder_1a62512c0bd11a5531611c1c3ac9fb1625>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape
		);

	std::pair<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`numpy_broadcast<doxid-namespacengraph_1_1builder_1a66f6b1d913e119b0f7ea432f29a7920e>`(const std::pair<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>, :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>>& args);

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`numpy_broadcast_for_matmul_operation<doxid-namespacengraph_1_1builder_1aa2648ca00c0f8fb7d1f28e7f60f9285c>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& left,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& right
		);

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`pdpd_broadcast<doxid-namespacengraph_1_1builder_1a0034c3be5260a728dbb4a6825fadbbb8>`(const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& inputs, int64_t axis);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`calculate_broadcast_axes<doxid-namespacengraph_1_1builder_1a7a8f82f0be74b04788b2a4a305d93374>`(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		std::size_t start_match_axis
		);

	std::pair<:ref:`Shape<doxid-classov_1_1_shape>`, std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>> :ref:`get_numpy_broadcast_shapes<doxid-namespacengraph_1_1builder_1ab29da3ce48b23704748faf12c6d9a1ad>`(const std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>& input_shapes);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_broadcast_node<doxid-namespacengraph_1_1builder_1a56f4e4ed23e360b5ebe79c1c7cebbbaf>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Shape<doxid-classov_1_1_shape>`& new_shape,
		std::size_t start_match_axis
		);

	template <class T>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_constant<doxid-namespacengraph_1_1builder_1adfd72913a3a4d8110810819146442dcd>`(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const T& num
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`make_constant_from_double<doxid-namespacengraph_1_1builder_1acb7e3fc96c0da0549187153f51b18706>`(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		double num
		);

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`split<doxid-namespacengraph_1_1builder_1ace7c5d5253c4c78c36f9c0e4b2cb5ebb>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const std::vector<int64_t>& length_parts,
		int64_t axis = 0
		);

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` :ref:`split<doxid-namespacengraph_1_1builder_1af2321ca7bdb5c602c69ae0d5068f4d82>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value, int64_t split_parts, int axis = 0);

	} // namespace builder
.. _details-namespacengraph_1_1builder:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Convenience functions that create addional graph nodes to implement commonly-used recipes, for example auto-broadcast.

Global Functions
----------------

.. _doxid-namespacengraph_1_1builder_1a96067407196af3eea5ac9eac6c4f0367:
.. index:: pair: function; numpy_broadcast_outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` numpy_broadcast_outputs(const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& values)

Broadcast all values, if necessary, to obtain equal shapes according to NumPy's auto-broadcasting scheme.

There are some shape combinations which the autobroadcast algoritm cannot handle. An exception is thrown when such combinations are provided to this function.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- values

		- Vector of output values.

	*
		- :ref:`ngraph::builder::numpy_autobroadcast_incompatible_shapes <doxid-classngraph_1_1builder_1_1numpy__autobroadcast__incompatible__shapes>`

		- 



.. rubric:: Returns:

Vector of broadcasted values.

.. _doxid-namespacengraph_1_1builder_1a62512c0bd11a5531611c1c3ac9fb1625:
.. index:: pair: function; numpy_broadcast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> numpy_broadcast(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape
		)

Broadcast input value to provided shape using NumPy's auto-broadcasting rules.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- Input value

	*
		- shape

		- Requested output shape



.. rubric:: Returns:

Node producing values with requested shape.

.. _doxid-namespacengraph_1_1builder_1a66f6b1d913e119b0f7ea432f29a7920e:
.. index:: pair: function; numpy_broadcast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> numpy_broadcast(const std::pair<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>, :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>>& args)

Wrap two graph values, if necessary, to obtain values with identical shapes, using NumPy's auto-broadcast rules.

The elements in the std::pair returned by this function correspond to those supplied in the std::pair provided via ``args``.

If ``args.first`` and ``args.second`` produce identical shapes, then the returned std::pair will have the same value as ``args``.

If ``args.first`` and ``args.second`` produce different shapes, then this function creates new ngraph::op::Reshape and/or ngraph::op::Broadcast nodes, as needed, to wrap ``args.first`` and/or ``args.second`` in a manner that yields values with the same shape.

There are some shape combinations which the autobroadcast algoritm cannot handle. An exception is thrown when such combinations are provided to this function.

* ``args.first`` is not null

* ``args.second`` is not null

* The ngraph::Node objects pointed to by ``args.first`` and ``args.second`` have not been altered by this function, except by possibly having added consumers of their values.

* If an exception was not thrown, then the return value's ``first`` and ``second`` elements point to ngraph::Node objects whose output values have the same shape.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ngraph::builder::numpy_autobroadcast_incompatible_shapes <doxid-classngraph_1_1builder_1_1numpy__autobroadcast__incompatible__shapes>`

		-

.. _doxid-namespacengraph_1_1builder_1aa2648ca00c0f8fb7d1f28e7f60f9285c:
.. index:: pair: function; numpy_broadcast_for_matmul_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` numpy_broadcast_for_matmul_operation(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& left,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& right
		)

Broadcast shape of two nodes to make them compatible for a matrix multiplication.

This function is reflecting broadcasting behaviour of NumPy's ``matmul`` operation. (`https://docs.scipy.org/doc/numpy/reference/generated/numpy.matmul.html <https://docs.scipy.org/doc/numpy/reference/generated/numpy.matmul.html>`__) This mean that only "stack of matrices" axes are bidirectionally broadcasted. The last two dimension are left untouched.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left

		- The Node providing data for the left-hand side of matrix multiplication.

	*
		- right

		- The Node providing data for the right-hand side of matrix multiplication.



.. rubric:: Returns:

The vector containing both outputs broadcasted.

.. _doxid-namespacengraph_1_1builder_1a0034c3be5260a728dbb4a6825fadbbb8:
.. index:: pair: function; pdpd_broadcast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` pdpd_broadcast(const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& inputs, int64_t axis)

Cast shape of all input nodes for an element-wise operation that requires shape-compatibility.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- Original list of inputs

	*
		- axis

		- Index starting to align



.. rubric:: Returns:

pdpd-style broadcasted list of nodes.

.. _doxid-namespacengraph_1_1builder_1a7a8f82f0be74b04788b2a4a305d93374:
.. index:: pair: function; calculate_broadcast_axes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> calculate_broadcast_axes(
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape,
		std::size_t start_match_axis
		)

Generate a list of broadcast axes.

Informally, a broadcast "adds" axes to the input tensor, replicating elements from the input tensor as needed to fill the new dimensions. Function calculate which of the output axes are added in this way.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_shape

		- The new shape for the output tensor.

	*
		- input_shape

		- The shape of input tensor.

	*
		- start_match_axis

		- The axis along which we want to replicate elements. The starting axis position (0-based) int the output shape from which the current shape of the tensor matches the desired new shape.



.. rubric:: Returns:

The indices of added axes.

.. _doxid-namespacengraph_1_1builder_1ab29da3ce48b23704748faf12c6d9a1ad:
.. index:: pair: function; get_numpy_broadcast_shapes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<:ref:`Shape<doxid-classov_1_1_shape>`, std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>> get_numpy_broadcast_shapes(const std::vector<:ref:`Shape<doxid-classov_1_1_shape>`>& input_shapes)

Calculate the output shape of numpy-style broadcast operation for all input shapes.

This function finds the maximum tensor shape that will be the result of element-wise operation that will be applied to the input shapes vector. The function also prepares the shape of each input for the element-wise operation by left-padding those shapes so that their rank is equal to the left_shape's rank.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_shapes

		- A vector of input shapes for which a common shape should be found



.. rubric:: Returns:

A pair that contains the target shape as its first object and a vector of padded input shapes ready to be broadcasted as the second object

.. _doxid-namespacengraph_1_1builder_1acb7e3fc96c0da0549187153f51b18706:
.. index:: pair: function; make_constant_from_double

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> make_constant_from_double(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		double num
		)

Create constant filled with double value.

If num value exeeds capacity of type, the value is clamped.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The type of produced Constant node.

	*
		- shape

		- The shape of produced Constant node.

	*
		- num

		- The value used to fill Constant node.



.. rubric:: Returns:

The Constant node which have expected type, shape and value.

.. _doxid-namespacengraph_1_1builder_1ace7c5d5253c4c78c36f9c0e4b2cb5ebb:
.. index:: pair: function; split

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` split(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const std::vector<int64_t>& length_parts,
		int64_t axis = 0
		)

Split value on specified axis into multiple parts.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to be split.

	*
		- length_parts

		- The vector defining the lengths of each split part.

	*
		- axis

		- The axis we split input node on. Default value is zero axis.



.. rubric:: Returns:

The vector containing multiple nodes we split input node into.

.. _doxid-namespacengraph_1_1builder_1af2321ca7bdb5c602c69ae0d5068f4d82:
.. index:: pair: function; split

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>` split(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value, int64_t split_parts, int axis = 0)

Split node on specified axis into multiple parts.

This implementation supports negative ``axis`` values (similar to NumPy indexing). This means that the axis to split on will be counted from the back of the tensor (negative values are subtracted from its rank).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value to split.

	*
		- split_parts

		- The number of parts we want to split output at given axis. The length of the axis to split must be divisible by this value.

	*
		- axis

		- The axis we split input node on. Default value is zero axis.



.. rubric:: Returns:

The vector containing multiple outputs we split input node into.

