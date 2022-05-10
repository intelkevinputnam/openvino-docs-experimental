.. index:: pair: class; ov::descriptor::Input
.. _doxid-classov_1_1descriptor_1_1_input:

class ov::descriptor::Input
===========================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <input.hpp>
	
	class Input
	{
	public:
		// construction
	
		:ref:`Input<doxid-classov_1_1descriptor_1_1_input_1a94604cf9c53e81a0da44d7c7360cc3f4>`(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index, :ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& output);
		:ref:`Input<doxid-classov_1_1descriptor_1_1_input_1a44e3aac76e00079140d79f393d87dd0e>`(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index);
		:target:`Input<doxid-classov_1_1descriptor_1_1_input_1ae1d7c75973e6356cd3a04b90f7cbf0f6>`(const Input&);
		:target:`Input<doxid-classov_1_1descriptor_1_1_input_1a37e98382353a7e8236b6d603da5df05f>`(Input&&);

		// methods
	
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_node<doxid-classov_1_1descriptor_1_1_input_1a995e60669699bb7031a2b402a7658c85>`() const;
		:ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_raw_pointer_node<doxid-classov_1_1descriptor_1_1_input_1aab55609315c31b60c6cf9bb4772d7223>`() const;
		size_t :ref:`get_index<doxid-classov_1_1descriptor_1_1_input_1acf18e7fdbdb6e5def9e314425042a822>`() const;
		const :ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& :ref:`get_output<doxid-classov_1_1descriptor_1_1_input_1a59e33ca1c31b770120db8b3787c8fbf3>`() const;
		:ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& :ref:`get_output<doxid-classov_1_1descriptor_1_1_input_1af443ddc0d6d3efcb005b08bf22e27209>`();
		bool :ref:`has_output<doxid-classov_1_1descriptor_1_1_input_1a6c3375dc52ed354a1a1b327e1576c138>`() const;
		const :ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_tensor<doxid-classov_1_1descriptor_1_1_input_1ae6a5ac5ec8566ccd62d47172b2228d71>`() const;
		:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_tensor<doxid-classov_1_1descriptor_1_1_input_1a624a5f6b405936f0cba73e698d573211>`();
		:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1descriptor_1_1_input_1a3f06bb3f3b9a11d9c792aab933cb12be>`();
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1descriptor_1_1_input_1acaeca3b825bddedd0bc6a16b7e8fffb5>`() const;
		void :ref:`replace_output<doxid-classov_1_1descriptor_1_1_input_1a3fb843f0249d223e3259c04896c0f0af>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node, size_t i);
		void :ref:`replace_output<doxid-classov_1_1descriptor_1_1_input_1a69b301c3909afb29227f25324803df1d>`(:ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& output);
		void :ref:`remove_output<doxid-classov_1_1descriptor_1_1_input_1a2a3b18d3cf06cb379dcfc7d2c6d25c7a>`();
		bool :ref:`get_is_relevant_to_shape<doxid-classov_1_1descriptor_1_1_input_1a4b40f725b59a89cfea72f519a13770ef>`() const;
		bool :ref:`get_is_relevant_to_value<doxid-classov_1_1descriptor_1_1_input_1a8823ce58f1210af8325e6b6687906881>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1descriptor_1_1_input_1a694e54a5751393a0db11219da16eba7c>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classov_1_1descriptor_1_1_input_1a5f10a48ac18b42495d8702a187266685>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1descriptor_1_1_input_1a414eb243cad92dd55806d5e409daacab>`() const;
		Input& :target:`operator =<doxid-classov_1_1descriptor_1_1_input_1a133d8716e23521cb5bba5d7185674af1>` (const Input&);
	};
.. _details-classov_1_1descriptor_1_1_input:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Construction
------------

.. _doxid-classov_1_1descriptor_1_1_input_1a94604cf9c53e81a0da44d7c7360cc3f4:
.. index:: pair: function; Input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Input(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index, :ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& output)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node that owns this input

	*
		- index

		- The position of this tensor in all input tensors

	*
		- output

		- The output that supplies a value for this input

.. _doxid-classov_1_1descriptor_1_1_input_1a44e3aac76e00079140d79f393d87dd0e:
.. index:: pair: function; Input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Input(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index)

Create an :ref:`Input <doxid-classov_1_1descriptor_1_1_input>` that is not connected to an output.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node that owns this input

	*
		- index

		- The position of this tensor in all input tensors

Methods
-------

.. _doxid-classov_1_1descriptor_1_1_input_1a995e60669699bb7031a2b402a7658c85:
.. index:: pair: function; get_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> get_node() const



.. rubric:: Returns:

the node that this is an input of

.. _doxid-classov_1_1descriptor_1_1_input_1aab55609315c31b60c6cf9bb4772d7223:
.. index:: pair: function; get_raw_pointer_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Node<doxid-classov_1_1_node>` \* get_raw_pointer_node() const



.. rubric:: Returns:

the raw pointer to the node that this is an input of

.. _doxid-classov_1_1descriptor_1_1_input_1acf18e7fdbdb6e5def9e314425042a822:
.. index:: pair: function; get_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_index() const



.. rubric:: Returns:

the position within all supplied tensors of this input

.. _doxid-classov_1_1descriptor_1_1_input_1a59e33ca1c31b770120db8b3787c8fbf3:
.. index:: pair: function; get_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& get_output() const



.. rubric:: Returns:

the connected output

.. _doxid-classov_1_1descriptor_1_1_input_1af443ddc0d6d3efcb005b08bf22e27209:
.. index:: pair: function; get_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& get_output()



.. rubric:: Returns:

the connected output

.. _doxid-classov_1_1descriptor_1_1_input_1a6c3375dc52ed354a1a1b327e1576c138:
.. index:: pair: function; has_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has_output() const



.. rubric:: Returns:

true if an output is connected to the input.

.. _doxid-classov_1_1descriptor_1_1_input_1ae6a5ac5ec8566ccd62d47172b2228d71:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& get_tensor() const



.. rubric:: Returns:

the tensor of the connected output

.. _doxid-classov_1_1descriptor_1_1_input_1a624a5f6b405936f0cba73e698d573211:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& get_tensor()



.. rubric:: Returns:

the tensor of the connected output

.. _doxid-classov_1_1descriptor_1_1_input_1a3fb843f0249d223e3259c04896c0f0af:
.. index:: pair: function; replace_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void replace_output(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node, size_t i)

Replace the current output that supplies a value for this input with output i of node.

.. _doxid-classov_1_1descriptor_1_1_input_1a69b301c3909afb29227f25324803df1d:
.. index:: pair: function; replace_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void replace_output(:ref:`Output<doxid-classov_1_1descriptor_1_1_output>`& output)

Replace the current output that supplies a value for this input with output.

.. _doxid-classov_1_1descriptor_1_1_input_1a2a3b18d3cf06cb379dcfc7d2c6d25c7a:
.. index:: pair: function; remove_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_output()

Remove the output from this input. The node will not be valid until another output is supplied.

.. _doxid-classov_1_1descriptor_1_1_input_1a4b40f725b59a89cfea72f519a13770ef:
.. index:: pair: function; get_is_relevant_to_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_is_relevant_to_shape() const

See :ref:`Node::set_input_is_relevant_to_shape <doxid-classov_1_1_node_1ae2eb8e3082bce5888e14163ed422d135>` for more details.



.. rubric:: Returns:

true if the value of this input is relevant to the output shapes of the corresponding node. (Usually this is false.)

.. _doxid-classov_1_1descriptor_1_1_input_1a8823ce58f1210af8325e6b6687906881:
.. index:: pair: function; get_is_relevant_to_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_is_relevant_to_value() const

See :ref:`Node::set_input_is_relevant_to_value <doxid-classov_1_1_node_1aa01ce25f87af4a741476d7857968f4be>` for more details.



.. rubric:: Returns:

true if the value of this input is relevant to the output value of the corresponding node. (Usually this is true.)

.. _doxid-classov_1_1descriptor_1_1_input_1a694e54a5751393a0db11219da16eba7c:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_shape() const



.. rubric:: Returns:

the shape of the connected output

.. _doxid-classov_1_1descriptor_1_1_input_1a5f10a48ac18b42495d8702a187266685:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const



.. rubric:: Returns:

the partial shape of the connected output

.. _doxid-classov_1_1descriptor_1_1_input_1a414eb243cad92dd55806d5e409daacab:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const



.. rubric:: Returns:

the element type of the connected output


