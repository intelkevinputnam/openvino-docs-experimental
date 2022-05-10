.. index:: pair: class; ov::CompiledModel
.. _doxid-classov_1_1_compiled_model:

class ov::CompiledModel
=======================



Overview
~~~~~~~~

This class represents a compiled model.

A model is compiled by a specific device by applying multiple optimization transformations, then mapping to compute kernels. :ref:`More...<details-classov_1_1_compiled_model>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <compiled_model.hpp>
	
	class CompiledModel
	{
	public:
		// methods
	
		std::shared_ptr<const :ref:`Model<doxid-classov_1_1_model>`> :ref:`get_runtime_model<doxid-classov_1_1_compiled_model_1aeb5d50ac029051980ced06bc6a1d33c7>`() const;
		std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>> :ref:`inputs<doxid-classov_1_1_compiled_model_1a39ec975bfc52054607b8800a6ee1fc2c>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_compiled_model_1a55f2867a43fb78829f9901c52f9ccea9>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_compiled_model_1aaff39ee2df6b73e51931ce8e604aa527>`(size_t i) const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_compiled_model_1a9d981d7b280d0db06d7798a5556af8ab>`(const std::string& tensor_name) const;
		std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>> :ref:`outputs<doxid-classov_1_1_compiled_model_1a0736f9b1443d5b564fc5b625e7aeb310>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_compiled_model_1a7ce36eb31153cc2ca623e1a3e33eed5f>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_compiled_model_1acdbddae0b26a4122c4ad3c8d25a41fc7>`(size_t i) const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_compiled_model_1a152e39465e6759a4c55d2d0433cbd3d2>`(const std::string& tensor_name) const;
		:ref:`InferRequest<doxid-classov_1_1_infer_request>` :ref:`create_infer_request<doxid-classov_1_1_compiled_model_1ae3633c0eb5173ed776446fba32b95953>`();
		void :ref:`export_model<doxid-classov_1_1_compiled_model_1ac9978b1d741c47286cba4eeb109effe4>`(std::ostream& model_stream);
		void :ref:`set_property<doxid-classov_1_1_compiled_model_1a9beec68aa25d6535e26fae5df00aaba0>`(const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<void, Properties...> :ref:`set_property<doxid-classov_1_1_compiled_model_1af701d1a8b3c834fe86aa80d1ab4a1758>`(Properties&&... properties);
	
		:ref:`Any<doxid-classov_1_1_any>` :ref:`get_property<doxid-classov_1_1_compiled_model_1a109d701ffe8b5de096961c7c98ff0bed>`(const std::string& name) const;
	
		template <typename T, PropertyMutability mutability>
		T :ref:`get_property<doxid-classov_1_1_compiled_model_1ab614111ae47c1776aa80f882d58234de>`(const :ref:`ov::Property<doxid-classov_1_1_property>`<T, mutability>& property) const;
	
		:ref:`RemoteContext<doxid-classov_1_1_remote_context>` :ref:`get_context<doxid-classov_1_1_compiled_model_1a22c5537d4c7182072d327077c386b01a>`() const;
		bool :ref:`operator !<doxid-classov_1_1_compiled_model_1a8ec0d4b4217e2b1c13f566377c21542f>` () const;
		:ref:`operator bool<doxid-classov_1_1_compiled_model_1a1e1856f4ceea9f49b7cdf5371514c145>` () const;
	};
.. _details-classov_1_1_compiled_model:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents a compiled model.

A model is compiled by a specific device by applying multiple optimization transformations, then mapping to compute kernels.

Methods
-------

.. _doxid-classov_1_1_compiled_model_1aeb5d50ac029051980ced06bc6a1d33c7:
.. index:: pair: function; get_runtime_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<const :ref:`Model<doxid-classov_1_1_model>`> get_runtime_model() const

Gets runtime model information from a device. This object represents an internal device-specific model that is optimized for a particular accelerator. It contains device-specific nodes, runtime information and can be used only to understand how the source model is optimized and which kernels, element types, and layouts are selected for optimal inference.



.. rubric:: Returns:

A model containing Executable Graph Info.

.. _doxid-classov_1_1_compiled_model_1a39ec975bfc52054607b8800a6ee1fc2c:
.. index:: pair: function; inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>> inputs() const

Gets all inputs of a compiled model. Inputs are represented as a vector of outputs of the :ref:`ov::op::v0::Parameter <doxid-classov_1_1op_1_1v0_1_1_parameter>` operations. They contain information about input tensors such as tensor shape, names, and element type.



.. rubric:: Returns:

std::vector of model inputs.

.. _doxid-classov_1_1_compiled_model_1a55f2867a43fb78829f9901c52f9ccea9:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> input() const

Gets a single input of a compiled model. The input is represented as an output of the :ref:`ov::op::v0::Parameter <doxid-classov_1_1op_1_1v0_1_1_parameter>` operation. The input contains information about input tensor such as tensor shape, names, and element type.

If a model has more than one input, this method throws :ref:`ov::Exception <doxid-classov_1_1_exception>`.



.. rubric:: Returns:

Compiled model input.

.. _doxid-classov_1_1_compiled_model_1aaff39ee2df6b73e51931ce8e604aa527:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> input(size_t i) const

Gets input of a compiled model identified by ``i``. The input contains information about input tensor such as tensor shape, names, and element type.

The method throws :ref:`ov::Exception <doxid-classov_1_1_exception>` if input with the specified index ``i`` is not found.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- i

		- Index of input.



.. rubric:: Returns:

Compiled model input.

.. _doxid-classov_1_1_compiled_model_1a9d981d7b280d0db06d7798a5556af8ab:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> input(const std::string& tensor_name) const

Gets input of a compiled model identified by ``tensor_name``. The input contains information about input tensor such as tensor shape, names, and element type.

The method throws :ref:`ov::Exception <doxid-classov_1_1_exception>` if input with the specified tensor name ``tensor_name`` is not found.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- The input tensor name.



.. rubric:: Returns:

Compiled model input.

.. _doxid-classov_1_1_compiled_model_1a0736f9b1443d5b564fc5b625e7aeb310:
.. index:: pair: function; outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>> outputs() const

Get all outputs of a compiled model. Outputs are represented as a vector of output from the :ref:`ov::op::v0::Result <doxid-classov_1_1op_1_1v0_1_1_result>` operations. Outputs contain information about output tensors such as tensor shape, names, and element type.



.. rubric:: Returns:

std::vector of model outputs.

.. _doxid-classov_1_1_compiled_model_1a7ce36eb31153cc2ca623e1a3e33eed5f:
.. index:: pair: function; output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> output() const

Gets a single output of a compiled model. The output is represented as an output from the :ref:`ov::op::v0::Result <doxid-classov_1_1op_1_1v0_1_1_result>` operation. The output contains information about output tensor such as tensor shape, names, and element type.

If a model has more than one output, this method throws :ref:`ov::Exception <doxid-classov_1_1_exception>`.



.. rubric:: Returns:

Compiled model output.

.. _doxid-classov_1_1_compiled_model_1acdbddae0b26a4122c4ad3c8d25a41fc7:
.. index:: pair: function; output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> output(size_t i) const

Gets output of a compiled model identified by ``index``. The output contains information about output tensor such as tensor shape, names, and element type.

The method throws :ref:`ov::Exception <doxid-classov_1_1_exception>` if output with the specified index ``index`` is not found.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- i

		- Index of input.



.. rubric:: Returns:

Compiled model output.

.. _doxid-classov_1_1_compiled_model_1a152e39465e6759a4c55d2d0433cbd3d2:
.. index:: pair: function; output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> output(const std::string& tensor_name) const

Gets output of a compiled model identified by ``tensor_name``. The output contains information about output tensor such as tensor shape, names, and element type.

The method throws :ref:`ov::Exception <doxid-classov_1_1_exception>` if output with the specified tensor name ``tensor_name`` is not found.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- :ref:`Output <doxid-classov_1_1_output>` tensor name.



.. rubric:: Returns:

Compiled model output.

.. _doxid-classov_1_1_compiled_model_1ae3633c0eb5173ed776446fba32b95953:
.. index:: pair: function; create_infer_request

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferRequest<doxid-classov_1_1_infer_request>` create_infer_request()

Creates an inference request object used to infer the compiled model. The created request has allocated input and output tensors (which can be changed later).



.. rubric:: Returns:

:ref:`InferRequest <doxid-classov_1_1_infer_request>` object

.. _doxid-classov_1_1_compiled_model_1ac9978b1d741c47286cba4eeb109effe4:
.. index:: pair: function; export_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void export_model(std::ostream& model_stream)

Exports the current compiled model to an output stream ``std::ostream``. The exported model can also be imported via the :ref:`ov::Core::import_model <doxid-classov_1_1_core_1a0d2853511bd7ba60cb591f4685b91884>` method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model_stream

		- :ref:`Output <doxid-classov_1_1_output>` stream to store the model to.



.. rubric:: See also:

:ref:`ov::Core::import_model <doxid-classov_1_1_core_1a0d2853511bd7ba60cb591f4685b91884>`

.. _doxid-classov_1_1_compiled_model_1a9beec68aa25d6535e26fae5df00aaba0:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_property(const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties)

Sets properties for the current compiled model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- properties

		- Map of pairs: (property name, property value).

.. _doxid-classov_1_1_compiled_model_1af701d1a8b3c834fe86aa80d1ab4a1758:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<void, Properties...> set_property(Properties&&... properties)

Sets properties for the current compiled model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- properties

		- Optional pack of pairs: (property name, property value).

.. _doxid-classov_1_1_compiled_model_1a109d701ffe8b5de096961c7c98ff0bed:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Any<doxid-classov_1_1_any>` get_property(const std::string& name) const

Gets properties for current compiled model.

The method is responsible for extracting information that affects compiled model inference. The list of supported configuration values can be extracted via :ref:`CompiledModel::get_property <doxid-classov_1_1_compiled_model_1a109d701ffe8b5de096961c7c98ff0bed>` with the :ref:`ov::supported_properties <doxid-group__ov__runtime__cpp__prop__api_1ga097f1274f26f3f4e1aa4fc3928748592>` key, but some of these keys cannot be changed dynamically, for example, :ref:`ov::device::id <doxid-group__ov__runtime__cpp__prop__api_1ga433b8ea52e99c2b1fa8b26453485d75d>` cannot be changed if a compiled model has already been compiled for a particular device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- :ref:`Property <doxid-classov_1_1_property>` key, can be found in ``openvino/runtime/properties.hpp``.



.. rubric:: Returns:

:ref:`Property <doxid-classov_1_1_property>` value.

.. _doxid-classov_1_1_compiled_model_1ab614111ae47c1776aa80f882d58234de:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, PropertyMutability mutability>
	T get_property(const :ref:`ov::Property<doxid-classov_1_1_property>`<T, mutability>& property) const

Gets properties related to device behaviour.

The method extracts information that can be set via the set_property method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type of a returned value.

	*
		- property

		- :ref:`Property <doxid-classov_1_1_property>` object.



.. rubric:: Returns:

Value of property.

.. _doxid-classov_1_1_compiled_model_1a22c5537d4c7182072d327077c386b01a:
.. index:: pair: function; get_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteContext<doxid-classov_1_1_remote_context>` get_context() const

Returns pointer to device-specific shared context on a remote accelerator device that was used to create this :ref:`CompiledModel <doxid-classov_1_1_compiled_model>`.



.. rubric:: Returns:

A context.

.. _doxid-classov_1_1_compiled_model_1a8ec0d4b4217e2b1c13f566377c21542f:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Checks if the current :ref:`CompiledModel <doxid-classov_1_1_compiled_model>` object is not initialized.



.. rubric:: Returns:

``true`` if the current :ref:`CompiledModel <doxid-classov_1_1_compiled_model>` object is not initialized; ``false``, otherwise.

.. _doxid-classov_1_1_compiled_model_1a1e1856f4ceea9f49b7cdf5371514c145:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Checks if the current :ref:`CompiledModel <doxid-classov_1_1_compiled_model>` object is initialized.



.. rubric:: Returns:

``true`` if the current :ref:`CompiledModel <doxid-classov_1_1_compiled_model>` object is initialized; ``false``, otherwise.


