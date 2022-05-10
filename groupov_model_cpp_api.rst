.. index:: pair: group; Basics
.. _doxid-group__ov__model__cpp__api:

Basics
======

.. toctree::
	:hidden:

	groupov_element_cpp_api.rst
	groupov_layout_cpp_api.rst
	DiscreteTypeInfo <structov_1_1DiscreteTypeInfo.rst>
	Dimension <classov_1_1Dimension.rst>
	Extension <classov_1_1Extension.rst>
	Input <classov_1_1Input.rst>
	Model <classov_1_1Model.rst>
	Node <classov_1_1Node.rst>
	Output <classov_1_1Output.rst>
	PartialShape <classov_1_1PartialShape.rst>
	PrePostProcessor <classov_1_1preprocess_1_1PrePostProcessor.rst>
	Shape <classov_1_1Shape.rst>

Overview
~~~~~~~~

OpenVINO Core C++ API to work with :ref:`ov::Model <doxid-classov_1_1_model>`, dynamic and static shapes, types :ref:`More...<details-group__ov__model__cpp__api>`

|	:ref:`Element types<doxid-group__ov__element__cpp__api>`
|	:ref:`Layout<doxid-group__ov__layout__cpp__api>`



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// structs

	struct :ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`;

	// classes

	class :ref:`ov::Dimension<doxid-classov_1_1_dimension>`;
	class :ref:`ov::Extension<doxid-classov_1_1_extension>`;
	template <>
	class :ref:`ov::Input<Node><doxid-classov_1_1_input_3_01_node_01_4>`;
	template <>
	class :ref:`ov::Input<const Node><doxid-classov_1_1_input_3_01const_01_node_01_4>`;
	class :ref:`ov::Model<doxid-classov_1_1_model>`;
	class :ref:`ov::Node<doxid-classov_1_1_node>`;
	template <>
	class :ref:`ov::Output<const Node><doxid-classov_1_1_output_3_01const_01_node_01_4>`;
	template <>
	class :ref:`ov::Output<Node><doxid-classov_1_1_output_3_01_node_01_4>`;
	class :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`;
	class :ref:`ov::preprocess::PrePostProcessor<doxid-classov_1_1preprocess_1_1_pre_post_processor>`;
	class :ref:`ov::Shape<doxid-classov_1_1_shape>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> :ref:`ov::clone_model<doxid-group__ov__model__cpp__api_1ga1a35bdeb865b10fc5b45b2e94632e77c>`(const :ref:`ov::Model<doxid-classov_1_1_model>`& model);

	template <typename SHAPE_TYPE>
	size_t :ref:`ov::shape_size<doxid-group__ov__model__cpp__api_1gafe8cdd6477ae9810c2bf368602d35883>`(const SHAPE_TYPE& shape);

	template <typename ForwardIt>
	size_t :ref:`ov::shape_size<doxid-group__ov__model__cpp__api_1ga0c2dadfcf0a5473a51bea86736da9045>`(
		ForwardIt start_dim,
		const ForwardIt end_dim
		);

.. _details-group__ov__model__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

OpenVINO Core C++ API to work with :ref:`ov::Model <doxid-classov_1_1_model>`, dynamic and static shapes, types

Global Functions
----------------

.. _doxid-group__ov__model__cpp__api_1ga1a35bdeb865b10fc5b45b2e94632e77c:
.. index:: pair: function; clone_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> ov::clone_model(const :ref:`ov::Model<doxid-classov_1_1_model>`& model)

input model is cloned and returned

.. _doxid-group__ov__model__cpp__api_1gafe8cdd6477ae9810c2bf368602d35883:
.. index:: pair: function; shape_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename SHAPE_TYPE>
	size_t ov::shape_size(const SHAPE_TYPE& shape)

Number of elements in spanned by a shape.

.. _doxid-group__ov__model__cpp__api_1ga0c2dadfcf0a5473a51bea86736da9045:
.. index:: pair: function; shape_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename ForwardIt>
	size_t ov::shape_size(
		ForwardIt start_dim,
		const ForwardIt end_dim
		)

Number of elements in a subset of dimensions of a shape. Returns a product of dimensions in a range [start_dim;end_dim)

