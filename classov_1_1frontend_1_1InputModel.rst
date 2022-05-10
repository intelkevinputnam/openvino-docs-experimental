.. index:: pair: class; ov::frontend::InputModel
.. _doxid-classov_1_1frontend_1_1_input_model:

class ov::frontend::InputModel
==============================



Overview
~~~~~~~~

:ref:`InputModel <doxid-classov_1_1frontend_1_1_input_model>` class represents an original, not yet converted model graph in a framework format given services to find places of interest in a graph or specialize/edit the model before conversion. :ref:`More...<details-classov_1_1frontend_1_1_input_model>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <input_model.hpp>
	
	class InputModel
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<InputModel> :target:`Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`;

		// construction
	
		:target:`InputModel<doxid-classov_1_1frontend_1_1_input_model_1a4216c3c441f112e3aa42a7af604a58ac>`();
		:target:`InputModel<doxid-classov_1_1frontend_1_1_input_model_1a9b2c2dc4b5bec9ce9678cd676df3e484>`(const InputModel&);
		:target:`InputModel<doxid-classov_1_1frontend_1_1_input_model_1ad9f0f41455cfe72067148aaa26cb6b6d>`(InputModel&&);

		// methods
	
		InputModel& :target:`operator =<doxid-classov_1_1frontend_1_1_input_model_1adfc3ae45d10a2360b824498ee30df698>` (const InputModel&);
		InputModel& :target:`operator =<doxid-classov_1_1frontend_1_1_input_model_1a07888cd215ff7fd0e0538c586cf12d4c>` (InputModel&&);
		virtual std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_inputs<doxid-classov_1_1frontend_1_1_input_model_1a8787a536ec05cb066ed39dbe76fad372>`() const;
		virtual std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_outputs<doxid-classov_1_1frontend_1_1_input_model_1aea0b7522ec209c80e1c20d78058cb971>`() const;
		virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_place_by_tensor_name<doxid-classov_1_1frontend_1_1_input_model_1ab4891521e5f8a8763275b9dbf47d247b>`(const std::string& tensor_name) const;
		virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_place_by_operation_name<doxid-classov_1_1frontend_1_1_input_model_1a69d44dbb9d8472c643ba8d7bfb53aed5>`(const std::string& operation_name) const;
	
		virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_place_by_operation_name_and_input_port<doxid-classov_1_1frontend_1_1_input_model_1a53f22ce59309db4c31d2d696c800f5cf>`(
			const std::string& operation_name,
			int input_port_index
			);
	
		virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_place_by_operation_name_and_output_port<doxid-classov_1_1frontend_1_1_input_model_1a4b42107215a7ebf72c96564b82108321>`(
			const std::string& operation_name,
			int output_port_index
			);
	
		virtual void :ref:`set_name_for_tensor<doxid-classov_1_1frontend_1_1_input_model_1abc71eed570eb5ea3f6259d822182672e>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& tensor,
			const std::string& new_name
			);
	
		virtual void :ref:`add_name_for_tensor<doxid-classov_1_1frontend_1_1_input_model_1a2a1a2c4de919bd77eebe29dcd73179bb>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& tensor,
			const std::string& new_name
			);
	
		virtual void :ref:`set_name_for_operation<doxid-classov_1_1frontend_1_1_input_model_1a6b94873fbe70a00b1d8377a45f78c44a>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& operation,
			const std::string& new_name
			);
	
		virtual void :ref:`free_name_for_tensor<doxid-classov_1_1frontend_1_1_input_model_1a4433a06e258ab68f9f8f4e5deb26ef0f>`(const std::string& name);
		virtual void :ref:`free_name_for_operation<doxid-classov_1_1frontend_1_1_input_model_1a984b79de660fbf371206b11a0a0952f4>`(const std::string& name);
	
		virtual void :ref:`set_name_for_dimension<doxid-classov_1_1frontend_1_1_input_model_1a538d7b19ad78d98f89d80b3d87a609ce>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
			size_t shape_dim_index,
			const std::string& dim_name
			);
	
		virtual void :ref:`cut_and_add_new_input<doxid-classov_1_1frontend_1_1_input_model_1a0f1520811acaf0bfbec00cea7724c677>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
			const std::string& new_name_optional = ""
			);
	
		virtual void :ref:`cut_and_add_new_output<doxid-classov_1_1frontend_1_1_input_model_1a8af9c9abef2707ca60aedf7e3e14b405>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
			const std::string& new_name_optional = ""
			);
	
		virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`add_output<doxid-classov_1_1frontend_1_1_input_model_1a84a0d7e02de3fb85c5f963bac49f74b8>`(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place);
		virtual void :ref:`remove_output<doxid-classov_1_1frontend_1_1_input_model_1a8c05cd0ebcd44ab14ecf1cce9859bea0>`(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place);
		virtual void :ref:`override_all_outputs<doxid-classov_1_1frontend_1_1_input_model_1a68891841c6d27680b88b5762583fccde>`(const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& outputs);
		virtual void :ref:`override_all_inputs<doxid-classov_1_1frontend_1_1_input_model_1ae59b801ce4b3e29ee01fb5f83e8e0512>`(const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& inputs);
	
		virtual void :ref:`extract_subgraph<doxid-classov_1_1frontend_1_1_input_model_1a48caa0b6656a24568ca401fb1866000a>`(
			const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& inputs,
			const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& outputs
			);
	
		virtual void :ref:`set_partial_shape<doxid-classov_1_1frontend_1_1_input_model_1a9313bb7159912aec55d918cc032bea9b>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
			const :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& shape
			);
	
		virtual :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>` :ref:`get_partial_shape<doxid-classov_1_1frontend_1_1_input_model_1a243aefe8e565ddbb05db762ea6062f56>`(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place) const;
	
		virtual void :ref:`set_element_type<doxid-classov_1_1frontend_1_1_input_model_1a774a9deaeecac23bbf68d1b630af840a>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
			const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type
			);
	
		virtual void :ref:`set_tensor_value<doxid-classov_1_1frontend_1_1_input_model_1ad12a9e5aa2faf8654fd08ce562056752>`(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place, const void \* value);
	
		virtual void :ref:`set_tensor_partial_value<doxid-classov_1_1frontend_1_1_input_model_1a60279a8fd46ea9bb8c5e7dc8752c2080>`(
			const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
			const void \* min_value,
			const void \* max_value
			);
	};
.. _details-classov_1_1frontend_1_1_input_model:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`InputModel <doxid-classov_1_1frontend_1_1_input_model>` class represents an original, not yet converted model graph in a framework format given services to find places of interest in a graph or specialize/edit the model before conversion.

Class methods are divided into several groups: searching for places, naming and annotation, topology editing, setting tensor properties.

Editing requests may affect ability to convert the original model to OV :ref:`Model <doxid-classov_1_1_model>`. Aim to provide these editing capabilities is to unlock conversion for models that are not natively supported "as-is" because of undefined shapes, types or operations.

Specific front-end implementation is supposed to have a lazy implementation for all methods, not doing a complete load of a model without an explicit method call. For example, the list of all inputs are not pre-fetched by :ref:`InputModel <doxid-classov_1_1frontend_1_1_input_model>` derived class instance creation, but only when get_inputs method is called. But it is not an obligation, the most convenient way should be chosen depending on the framework model representation.

All editing requests affect the model representation that is held behind the scene successive method calls observe a new graph structure.

Methods
-------

.. _doxid-classov_1_1frontend_1_1_input_model_1a8787a536ec05cb066ed39dbe76fad372:
.. index:: pair: function; get_inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_inputs() const

Returns all inputs for a model An input is a place in a graph where data is supposed to flow inside graph from outside. It can be a tensor, port, operation; which kind of place can be an output is FW dependent. Usually framework models have a dedicated artifact to code model input, it can be a tensor without producer, that writes to it in ONNX, or a special operation like Placeholder in TensorFlow.



.. rubric:: Returns:

A vector of input place references

.. _doxid-classov_1_1frontend_1_1_input_model_1aea0b7522ec209c80e1c20d78058cb971:
.. index:: pair: function; get_outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_outputs() const

Returns all output for a model An output is a terminal place in a graph where data escapes the flow. It can be a tensor, port, operation; which kind of place can be an output is FW dependent. In comparison to a graph input, the output is less formally defined thing and determination of initial list of outputs may include some conventions defined by a frontend itself, not a framework. For example, all output ports without consumers may be considered as outputs.



.. rubric:: Returns:

A vector of output place references

.. _doxid-classov_1_1frontend_1_1_input_model_1ab4891521e5f8a8763275b9dbf47d247b:
.. index:: pair: function; get_place_by_tensor_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_place_by_tensor_name(const std::string& tensor_name) const

Returns a tensor place by a tensor name following framework conventions, or nullptr if a tensor with this name doesn't exist.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- Name of tensor



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` place corresponding to specified tensor name or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_input_model_1a69d44dbb9d8472c643ba8d7bfb53aed5:
.. index:: pair: function; get_place_by_operation_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_place_by_operation_name(const std::string& operation_name) const

Returns an operation place by an operation name following framework conventions, or nullptr if an operation with this name doesn't exist.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- operation_name

		- Name of operation



.. rubric:: Returns:

:ref:`Place <doxid-classov_1_1frontend_1_1_place>` representing operation or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_input_model_1a53f22ce59309db4c31d2d696c800f5cf:
.. index:: pair: function; get_place_by_operation_name_and_input_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_place_by_operation_name_and_input_port(
		const std::string& operation_name,
		int input_port_index
		)

Returns an input port place by operation name and appropriate port index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- operation_name

		- Name of operation

	*
		- input_port_index

		- Index of input port for this operation



.. rubric:: Returns:

:ref:`Place <doxid-classov_1_1frontend_1_1_place>` representing input port of operation or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_input_model_1a4b42107215a7ebf72c96564b82108321:
.. index:: pair: function; get_place_by_operation_name_and_output_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_place_by_operation_name_and_output_port(
		const std::string& operation_name,
		int output_port_index
		)

Returns an output port place by operation name and appropriate port index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- operation_name

		- Name of operation

	*
		- output_port_index

		- Index of output port for this operation



.. rubric:: Returns:

:ref:`Place <doxid-classov_1_1frontend_1_1_place>` representing output port of operation or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_input_model_1abc71eed570eb5ea3f6259d822182672e:
.. index:: pair: function; set_name_for_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_name_for_tensor(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& tensor,
		const std::string& new_name
		)

Sets name for tensor. Overwrites existing names of this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- :ref:`Tensor <doxid-classov_1_1_tensor>` place

	*
		- new_name

		- New name for this tensor

.. _doxid-classov_1_1frontend_1_1_input_model_1a2a1a2c4de919bd77eebe29dcd73179bb:
.. index:: pair: function; add_name_for_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void add_name_for_tensor(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& tensor,
		const std::string& new_name
		)

Adds new name for tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- :ref:`Tensor <doxid-classov_1_1_tensor>` place

	*
		- new_name

		- New name to be added to this place

.. _doxid-classov_1_1frontend_1_1_input_model_1a6b94873fbe70a00b1d8377a45f78c44a:
.. index:: pair: function; set_name_for_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_name_for_operation(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& operation,
		const std::string& new_name
		)

Sets name for operation. Overwrites existing names of this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- operation

		- Operation place

	*
		- new_name

		- New name for this operation

.. _doxid-classov_1_1frontend_1_1_input_model_1a4433a06e258ab68f9f8f4e5deb26ef0f:
.. index:: pair: function; free_name_for_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void free_name_for_tensor(const std::string& name)

Unassign specified name from tensor place(s)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of tensor

.. _doxid-classov_1_1frontend_1_1_input_model_1a984b79de660fbf371206b11a0a0952f4:
.. index:: pair: function; free_name_for_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void free_name_for_operation(const std::string& name)

Unassign specified name from operation place(s)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of operation

.. _doxid-classov_1_1frontend_1_1_input_model_1a538d7b19ad78d98f89d80b3d87a609ce:
.. index:: pair: function; set_name_for_dimension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_name_for_dimension(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
		size_t shape_dim_index,
		const std::string& dim_name
		)

Set name for a particular dimension of a place (e.g. batch dimension)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Model <doxid-classov_1_1_model>` 's place

	*
		- shape_dim_index

		- :ref:`Dimension <doxid-classov_1_1_dimension>` index

	*
		- dim_name

		- Name to assign on this dimension

.. _doxid-classov_1_1frontend_1_1_input_model_1a0f1520811acaf0bfbec00cea7724c677:
.. index:: pair: function; cut_and_add_new_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void cut_and_add_new_input(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
		const std::string& new_name_optional = ""
		)

Cut immediately before this place and assign this place as new input; prune all nodes that don't contribute to any output.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- New place to be assigned as input

	*
		- new_name_optional

		- Optional new name assigned to this input place

.. _doxid-classov_1_1frontend_1_1_input_model_1a8af9c9abef2707ca60aedf7e3e14b405:
.. index:: pair: function; cut_and_add_new_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void cut_and_add_new_output(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
		const std::string& new_name_optional = ""
		)

Cut immediately after this place and assign this place as new output; prune all nodes that don't contribute to any output.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- New place to be assigned as output

	*
		- new_name_optional

		- Optional new name assigned to this output place

.. _doxid-classov_1_1frontend_1_1_input_model_1a84a0d7e02de3fb85c5f963bac49f74b8:
.. index:: pair: function; add_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` add_output(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place)

Assign this place as new output or add necessary nodes to represent a new output.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- Anchor point to add an output



.. rubric:: Returns:

new output place, may be the same as a given place

.. _doxid-classov_1_1frontend_1_1_input_model_1a8c05cd0ebcd44ab14ecf1cce9859bea0:
.. index:: pair: function; remove_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void remove_output(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place)

Removes any sinks directly attached to this place with all inbound data flow if it is not required by any other output.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Model <doxid-classov_1_1_model>` place

.. _doxid-classov_1_1frontend_1_1_input_model_1a68891841c6d27680b88b5762583fccde:
.. index:: pair: function; override_all_outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void override_all_outputs(const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& outputs)

Replaces all existing outputs with new ones removing all data flow that is not required for new outputs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outputs

		- Vector with places that will become new outputs; may intersect existing outputs.

	*
		- outputs

		- Array of new output places

.. _doxid-classov_1_1frontend_1_1_input_model_1ae59b801ce4b3e29ee01fb5f83e8e0512:
.. index:: pair: function; override_all_inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void override_all_inputs(const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& inputs)

Modifies the graph to use new inputs instead of existing ones. New inputs should completely satisfy all existing outputs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- Array of new input places

.. _doxid-classov_1_1frontend_1_1_input_model_1a48caa0b6656a24568ca401fb1866000a:
.. index:: pair: function; extract_subgraph

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void extract_subgraph(
		const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& inputs,
		const std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`>& outputs
		)

Leaves only subgraph that are defined by new inputs and new outputs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- Array of new input places

	*
		- outputs

		- Array of new output places

.. _doxid-classov_1_1frontend_1_1_input_model_1a9313bb7159912aec55d918cc032bea9b:
.. index:: pair: function; set_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_partial_shape(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
		const :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& shape
		)

Defines all possible shape that may be used for this place; place should be uniquely refer to some data. This partial shape will be converted to corresponding shape of results OV nodes and will define shape inference when the model is converted to OV.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Model <doxid-classov_1_1_model>` place

	*
		- shape

		- Partial shape for this place

.. _doxid-classov_1_1frontend_1_1_input_model_1a243aefe8e565ddbb05db762ea6062f56:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>` get_partial_shape(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place) const

Returns current partial shape used for this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Model <doxid-classov_1_1_model>` place



.. rubric:: Returns:

Partial shape for this place

.. _doxid-classov_1_1frontend_1_1_input_model_1a774a9deaeecac23bbf68d1b630af840a:
.. index:: pair: function; set_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_element_type(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
		const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type
		)

Sets new element type for a place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Model <doxid-classov_1_1_model>` place

	*
		- type

		- New element type

.. _doxid-classov_1_1frontend_1_1_input_model_1ad12a9e5aa2faf8654fd08ce562056752:
.. index:: pair: function; set_tensor_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_tensor_value(const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place, const void \* value)

Freezes a tensor with statically defined value or replace existing value for already constant node or tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Tensor <doxid-classov_1_1_tensor>` place

	*
		- value

		- Value for tensor place representing a memory buffer

.. _doxid-classov_1_1frontend_1_1_input_model_1a60279a8fd46ea9bb8c5e7dc8752c2080:
.. index:: pair: function; set_tensor_partial_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_tensor_partial_value(
		const :ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& place,
		const void \* min_value,
		const void \* max_value
		)

Defines partial value (lower bound and upper bound) for a tensor place TODO: more details for min_value and max_value format; who defines shape?



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- place

		- :ref:`Tensor <doxid-classov_1_1_tensor>` place

	*
		- min_value

		- Lower bound of partial value for tensor place

	*
		- max_value

		- Upper bound of partial value for tensor place


