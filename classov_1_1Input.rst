.. index:: pair: class; ov::Input<Node>
.. _doxid-classov_1_1_input_3_01_node_01_4:

class ov::Input<Node>
=====================



Overview
~~~~~~~~

A handle for one of a node's inputs. :ref:`More...<details-classov_1_1_input_3_01_node_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node_input.hpp>
	
	template <>
	class Input<Node>
	{
	public:
		// construction
	
		:ref:`Input<doxid-classov_1_1_input_3_01_node_01_4_1ab5099655691dddf294cbb476abd0ea46>`(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index);

		// methods
	
		:ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_node<doxid-classov_1_1_input_3_01_node_01_4_1a54b344da2b83526d3e369679fd66b330>`() const;
		size_t :ref:`get_index<doxid-classov_1_1_input_3_01_node_01_4_1a20e4cebacc4ffa9739f3707cdaa526a6>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1_input_3_01_node_01_4_1a36b399c6fe910ca1e83b5edc472c3c64>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1_input_3_01_node_01_4_1aae226e345b0f92a642f97987e9f0e3d2>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classov_1_1_input_3_01_node_01_4_1acaf00fb60c88cad3fd547848bc316aef>`() const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_source_output<doxid-classov_1_1_input_3_01_node_01_4_1a925b0c528107d8d6e471f83fc5346b16>`() const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_tensor<doxid-classov_1_1_input_3_01_node_01_4_1aab10ba69120ff7913fb1445dcc243f32>`() const;
		std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> :ref:`get_tensor_ptr<doxid-classov_1_1_input_3_01_node_01_4_1a35b924cd11bd620e2679ebe858fcb06f>`() const;
		bool :ref:`get_is_relevant_to_shapes<doxid-classov_1_1_input_3_01_node_01_4_1a137d23074de8edd54e7dd69f77f6fb30>`() const;
		bool :ref:`get_is_relevant_to_values<doxid-classov_1_1_input_3_01_node_01_4_1a7b322b8d4f80fe86f24f7be8345ceffd>`() const;
		void :ref:`replace_source_output<doxid-classov_1_1_input_3_01_node_01_4_1aae2e9001c0ea40301018012d813a0782>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& new_source_output) const;
		:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :ref:`get_rt_info<doxid-classov_1_1_input_3_01_node_01_4_1ab2d353c52bbbacad8866fa06d0d06eaf>`();
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :ref:`get_rt_info<doxid-classov_1_1_input_3_01_node_01_4_1a1e0a3d3b4193e04a4ffd5816a982a476>`() const;
		bool :target:`operator ==<doxid-classov_1_1_input_3_01_node_01_4_1a0d7a528ab327f2ed06b1a353c3fdaca4>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator !=<doxid-classov_1_1_input_3_01_node_01_4_1a6f7e4c9eaa43b9da5a935c12ed016400>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator <<doxid-classov_1_1_input_3_01_node_01_4_1a8b8f1b2a312521f885cbc041eaf49c81>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator ><doxid-classov_1_1_input_3_01_node_01_4_1af6f2be9921664dbedd7902cf106ac9c2>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator <=<doxid-classov_1_1_input_3_01_node_01_4_1a49d1420768197580b11d1cb9547c7f22>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator >=<doxid-classov_1_1_input_3_01_node_01_4_1a9b1e762f7bbcbbd67c673232ecec23e4>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
	};
.. _details-classov_1_1_input_3_01_node_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A handle for one of a node's inputs.

Construction
------------

.. _doxid-classov_1_1_input_3_01_node_01_4_1ab5099655691dddf294cbb476abd0ea46:
.. index:: pair: function; Input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Input(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index)

Constructs a :ref:`Input <doxid-classov_1_1_input>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- Pointer to the node for the input handle.

	*
		- index

		- The index of the input.

Methods
-------

.. _doxid-classov_1_1_input_3_01_node_01_4_1a54b344da2b83526d3e369679fd66b330:
.. index:: pair: function; get_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Node<doxid-classov_1_1_node>` \* get_node() const



.. rubric:: Returns:

A pointer to the node referenced by this input handle.

.. _doxid-classov_1_1_input_3_01_node_01_4_1a20e4cebacc4ffa9739f3707cdaa526a6:
.. index:: pair: function; get_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_index() const



.. rubric:: Returns:

The index of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01_node_01_4_1a36b399c6fe910ca1e83b5edc472c3c64:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const



.. rubric:: Returns:

The element type of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01_node_01_4_1aae226e345b0f92a642f97987e9f0e3d2:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_shape() const



.. rubric:: Returns:

The shape of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01_node_01_4_1acaf00fb60c88cad3fd547848bc316aef:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const



.. rubric:: Returns:

The partial shape of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01_node_01_4_1a925b0c528107d8d6e471f83fc5346b16:
.. index:: pair: function; get_source_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_source_output() const



.. rubric:: Returns:

A handle to the output that is connected to this input.

.. _doxid-classov_1_1_input_3_01_node_01_4_1aab10ba69120ff7913fb1445dcc243f32:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& get_tensor() const



.. rubric:: Returns:

A reference to the tensor descriptor for this input.

.. _doxid-classov_1_1_input_3_01_node_01_4_1a35b924cd11bd620e2679ebe858fcb06f:
.. index:: pair: function; get_tensor_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> get_tensor_ptr() const



.. rubric:: Returns:

A shared pointer to the tensor descriptor for this input.

.. _doxid-classov_1_1_input_3_01_node_01_4_1a137d23074de8edd54e7dd69f77f6fb30:
.. index:: pair: function; get_is_relevant_to_shapes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_is_relevant_to_shapes() const



.. rubric:: Returns:

true if this input is relevant to its node's output shapes; else false.

.. _doxid-classov_1_1_input_3_01_node_01_4_1a7b322b8d4f80fe86f24f7be8345ceffd:
.. index:: pair: function; get_is_relevant_to_values

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_is_relevant_to_values() const



.. rubric:: Returns:

true if this input is relevant to its node's output values; else false.

.. _doxid-classov_1_1_input_3_01_node_01_4_1aae2e9001c0ea40301018012d813a0782:
.. index:: pair: function; replace_source_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void replace_source_output(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& new_source_output) const

Replaces the source output of this input.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- new_source_output

		- A handle for the output that will replace this input's source.

.. _doxid-classov_1_1_input_3_01_node_01_4_1ab2d353c52bbbacad8866fa06d0d06eaf:
.. index:: pair: function; get_rt_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& get_rt_info()



.. rubric:: Returns:

The reference to runtime info map

.. _doxid-classov_1_1_input_3_01_node_01_4_1a1e0a3d3b4193e04a4ffd5816a982a476:
.. index:: pair: function; get_rt_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& get_rt_info() const



.. rubric:: Returns:

The constant reference to runtime info map


.. index:: pair: class; ov::Input<const Node>
.. _doxid-classov_1_1_input_3_01const_01_node_01_4:

class ov::Input<const Node>
^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

A handle for one of a node's inputs. :ref:`More...<details-classov_1_1_input_3_01const_01_node_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node_input.hpp>
	
	template <>
	class Input<const Node>
	{
	public:
		// construction
	
		:ref:`Input<doxid-classov_1_1_input_3_01const_01_node_01_4_1a4504abfb951572953884912aca9c19e8>`(const :ref:`Node<doxid-classov_1_1_node>` \* node, size_t index);

		// methods
	
		const :ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_node<doxid-classov_1_1_input_3_01const_01_node_01_4_1a28a55a50200468bf017fcac3762494db>`() const;
		size_t :ref:`get_index<doxid-classov_1_1_input_3_01const_01_node_01_4_1adb311842616a8442e14de4eee346ea54>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1_input_3_01const_01_node_01_4_1a78d7975849240448426625091b707da7>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1_input_3_01const_01_node_01_4_1a08e5472b398d5e0e164befa3b271415f>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classov_1_1_input_3_01const_01_node_01_4_1aebec7b74f51d5eabb49cc569c7a723ff>`() const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_source_output<doxid-classov_1_1_input_3_01const_01_node_01_4_1a11690a3ab4a5b33f0d8508ef278640d1>`() const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_tensor<doxid-classov_1_1_input_3_01const_01_node_01_4_1a2344e30bbefbd9fed11e7be56d82fc83>`() const;
		std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> :ref:`get_tensor_ptr<doxid-classov_1_1_input_3_01const_01_node_01_4_1a372dfcd2d7449c2da49bf147e5f586fd>`() const;
		bool :ref:`get_is_relevant_to_shapes<doxid-classov_1_1_input_3_01const_01_node_01_4_1a1aad9ed5d78aed50b481f76411b2fb61>`() const;
		bool :ref:`get_is_relevant_to_values<doxid-classov_1_1_input_3_01const_01_node_01_4_1a3c33e182d609bc673d3ab59588f87ff0>`() const;
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :ref:`get_rt_info<doxid-classov_1_1_input_3_01const_01_node_01_4_1a7b64fa6a736d41a427d62768d49c9913>`() const;
		bool :target:`operator ==<doxid-classov_1_1_input_3_01const_01_node_01_4_1a8ab7f65161deb46ebbcf874d1b92dfa9>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator !=<doxid-classov_1_1_input_3_01const_01_node_01_4_1a57411472d106e83a1dec423fdbc924f0>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator <<doxid-classov_1_1_input_3_01const_01_node_01_4_1ae4581056e2ac069733c9fd85d54e739d>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator ><doxid-classov_1_1_input_3_01const_01_node_01_4_1a665017c53121a3b01009d4e813a768e1>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator <=<doxid-classov_1_1_input_3_01const_01_node_01_4_1ab5a072e644fc285372dd88c52e9b68df>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
		bool :target:`operator >=<doxid-classov_1_1_input_3_01const_01_node_01_4_1a40c870fb7c22e7d7b6bdc7ed35e6be20>` (const :ref:`Input<doxid-classov_1_1_input>`& other) const;
	};
.. _details-classov_1_1_input_3_01const_01_node_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A handle for one of a node's inputs.

Construction
------------

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a4504abfb951572953884912aca9c19e8:
.. index:: pair: function; Input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Input(const :ref:`Node<doxid-classov_1_1_node>` \* node, size_t index)

Constructs a :ref:`Input <doxid-classov_1_1_input>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- Pointer to the node for the input handle.

	*
		- index

		- The index of the input.

Methods
-------

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a28a55a50200468bf017fcac3762494db:
.. index:: pair: function; get_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Node<doxid-classov_1_1_node>` \* get_node() const



.. rubric:: Returns:

A pointer to the node referenced by this input handle.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1adb311842616a8442e14de4eee346ea54:
.. index:: pair: function; get_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_index() const



.. rubric:: Returns:

The index of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a78d7975849240448426625091b707da7:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const



.. rubric:: Returns:

The element type of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a08e5472b398d5e0e164befa3b271415f:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_shape() const



.. rubric:: Returns:

The shape of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1aebec7b74f51d5eabb49cc569c7a723ff:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const



.. rubric:: Returns:

The partial shape of the input referred to by this input handle.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a11690a3ab4a5b33f0d8508ef278640d1:
.. index:: pair: function; get_source_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_source_output() const



.. rubric:: Returns:

A handle to the output that is connected to this input.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a2344e30bbefbd9fed11e7be56d82fc83:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& get_tensor() const



.. rubric:: Returns:

A reference to the tensor descriptor for this input.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a372dfcd2d7449c2da49bf147e5f586fd:
.. index:: pair: function; get_tensor_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> get_tensor_ptr() const



.. rubric:: Returns:

A shared pointer to the tensor descriptor for this input.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a1aad9ed5d78aed50b481f76411b2fb61:
.. index:: pair: function; get_is_relevant_to_shapes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_is_relevant_to_shapes() const



.. rubric:: Returns:

true if this input is relevant to its node's output shapes; else false.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a3c33e182d609bc673d3ab59588f87ff0:
.. index:: pair: function; get_is_relevant_to_values

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_is_relevant_to_values() const



.. rubric:: Returns:

true if this input is relevant to its node's output values; else false.

.. _doxid-classov_1_1_input_3_01const_01_node_01_4_1a7b64fa6a736d41a427d62768d49c9913:
.. index:: pair: function; get_rt_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& get_rt_info() const



.. rubric:: Returns:

The constant reference to runtime info map


.. index:: pair: class; ov::Input
.. _doxid-classov_1_1_input:

class ov::Input
^^^^^^^^^^^^^^^






