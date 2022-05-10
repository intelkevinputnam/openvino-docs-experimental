.. index:: pair: class; ov::InferRequest
.. _doxid-classov_1_1_infer_request:

class ov::InferRequest
======================



Overview
~~~~~~~~

This is a class of infer request that can be run in asynchronous or synchronous manners. :ref:`More...<details-classov_1_1_infer_request>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <infer_request.hpp>
	
	class InferRequest
	{
	public:
		// construction
	
		:ref:`InferRequest<doxid-classov_1_1_infer_request_1aa993f40a8cf22469c07f4744a053b143>`();
		:ref:`InferRequest<doxid-classov_1_1_infer_request_1af14ae3f0f36c15ace1cd0e08dfed5e74>`(const InferRequest& other);
		:ref:`InferRequest<doxid-classov_1_1_infer_request_1a9726bdafae48afc327afc74f8514c8d1>`(InferRequest&& other);

		// methods
	
		InferRequest& :ref:`operator =<doxid-classov_1_1_infer_request_1a4e8744409d7073f8b564572fe8d569c4>` (const InferRequest& other);
		InferRequest& :ref:`operator =<doxid-classov_1_1_infer_request_1a741bf6de4c3bcf0544e735beeb1404e9>` (InferRequest&& other);
		void :ref:`set_tensor<doxid-classov_1_1_infer_request_1af54f126e7fb3b3a0343841dda8bcc368>`(const std::string& tensor_name, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		void :ref:`set_tensor<doxid-classov_1_1_infer_request_1acb0e8822dc4206740174bfdf95c2754b>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& port, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		void :ref:`set_tensor<doxid-classov_1_1_infer_request_1a51a945021f2559c18cdbfa0c8ce66cb4>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& port, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
	
		void :ref:`set_tensors<doxid-classov_1_1_infer_request_1a935a952c07cc7130a64614d0952db997>`(
			const std::string& tensor_name,
			const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors
			);
	
		void :ref:`set_tensors<doxid-classov_1_1_infer_request_1a28e18a17764134c47d26482d82ce9b65>`(
			const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& port,
			const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors
			);
	
		void :ref:`set_input_tensor<doxid-classov_1_1_infer_request_1a5ddca7af7faffa2c90fd600a3f84aa6e>`(size_t idx, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		void :ref:`set_input_tensor<doxid-classov_1_1_infer_request_1a5f3640729c5e9e197bad73dd3260573c>`(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		void :ref:`set_input_tensors<doxid-classov_1_1_infer_request_1af847095ee6e85141fb3ef35f1556d89c>`(const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors);
		void :ref:`set_input_tensors<doxid-classov_1_1_infer_request_1a5fef80b34aca795d8b426ad93c93fe0f>`(size_t idx, const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors);
		void :ref:`set_output_tensor<doxid-classov_1_1_infer_request_1a3e93efd003301c4de6b0181163e7d14d>`(size_t idx, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		void :ref:`set_output_tensor<doxid-classov_1_1_infer_request_1ab2844540aa73e122021882767656fbb2>`(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_tensor<doxid-classov_1_1_infer_request_1a75b8da7c6b00686bede600dddceaffc4>`(const std::string& tensor_name);
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_tensor<doxid-classov_1_1_infer_request_1ae95479408beb5d091037ef8221ba9940>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& port);
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_tensor<doxid-classov_1_1_infer_request_1ac30bcc9c86bdf2e89165c562f009e70a>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& port);
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_input_tensor<doxid-classov_1_1_infer_request_1a5f0bc1ab40de6a7a12136b4a4e6a8b54>`(size_t idx);
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_input_tensor<doxid-classov_1_1_infer_request_1a7e857e8a9f13114289db2cbfe831763c>`();
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_output_tensor<doxid-classov_1_1_infer_request_1a350159a8d967022db46633eed50d073a>`(size_t idx);
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_output_tensor<doxid-classov_1_1_infer_request_1a9bf7bf67c58858bda86ae01e83cd14c1>`();
		void :ref:`infer<doxid-classov_1_1_infer_request_1abcb7facc9f7c4b9226a1fd343e56958d>`();
		void :ref:`cancel<doxid-classov_1_1_infer_request_1aa100b080271f057ab5f98d1832af414d>`();
		std::vector<:ref:`ProfilingInfo<doxid-structov_1_1_profiling_info>`> :ref:`get_profiling_info<doxid-classov_1_1_infer_request_1af70dbbd38ffb928ce407a22bd781b6d5>`() const;
		void :ref:`start_async<doxid-classov_1_1_infer_request_1a5a05ae4352f804c865e11f5d68b983d5>`();
		void :ref:`wait<doxid-classov_1_1_infer_request_1ab0e0739da45789d816f8b5584a0b5691>`();
		bool :ref:`wait_for<doxid-classov_1_1_infer_request_1a94d6d52e03d2ad20310a1e0fdd807e9e>`(const std::chrono::milliseconds timeout);
		void :ref:`set_callback<doxid-classov_1_1_infer_request_1afba2a10162ab356728ec8901973e8f02>`(std::function<void(std::exception_ptr)> callback);
		std::vector<:ref:`VariableState<doxid-classov_1_1_variable_state>`> :ref:`query_state<doxid-classov_1_1_infer_request_1ac415100cc002db60b0afd871401345b5>`();
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`get_compiled_model<doxid-classov_1_1_infer_request_1ad295894c4d65d0e0dc260d4a6cf287eb>`();
		bool :ref:`operator !<doxid-classov_1_1_infer_request_1a4b10bba9b6b8331b4fce992c737668d2>` () const;
		:ref:`operator bool<doxid-classov_1_1_infer_request_1a324eb815c65cc72f4d2b534e950b0c34>` () const;
		bool :ref:`operator !=<doxid-classov_1_1_infer_request_1a659e8621129aa8aff0db2daace42a388>` (const InferRequest& other) const;
		bool :ref:`operator ==<doxid-classov_1_1_infer_request_1a2f0bdc369c5e54a4f1f49e85744b7ee6>` (const InferRequest& other) const;
	};
.. _details-classov_1_1_infer_request:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is a class of infer request that can be run in asynchronous or synchronous manners.

Construction
------------

.. _doxid-classov_1_1_infer_request_1aa993f40a8cf22469c07f4744a053b143:
.. index:: pair: function; InferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest()

Default constructor.

.. _doxid-classov_1_1_infer_request_1af14ae3f0f36c15ace1cd0e08dfed5e74:
.. index:: pair: function; InferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest(const InferRequest& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`InferRequest <doxid-classov_1_1_infer_request>` object.

.. _doxid-classov_1_1_infer_request_1a9726bdafae48afc327afc74f8514c8d1:
.. index:: pair: function; InferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest(InferRequest&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`InferRequest <doxid-classov_1_1_infer_request>` object.

Methods
-------

.. _doxid-classov_1_1_infer_request_1a4e8744409d7073f8b564572fe8d569c4:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest& operator = (const InferRequest& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`InferRequest <doxid-classov_1_1_infer_request>` object.



.. rubric:: Returns:

Reference to the current object.

.. _doxid-classov_1_1_infer_request_1a741bf6de4c3bcf0544e735beeb1404e9:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InferRequest& operator = (InferRequest&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`InferRequest <doxid-classov_1_1_infer_request>` object.



.. rubric:: Returns:

Reference to the current object.

.. _doxid-classov_1_1_infer_request_1af54f126e7fb3b3a0343841dda8bcc368:
.. index:: pair: function; set_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_tensor(const std::string& tensor_name, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an input/output tensor to infer on.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- Name of the input or output tensor.

	*
		- tensor

		- Reference to the tensor. The element_type and shape of the tensor must match the model's input/output element_type and size.

.. _doxid-classov_1_1_infer_request_1acb0e8822dc4206740174bfdf95c2754b:
.. index:: pair: function; set_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_tensor(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& port, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an input/output tensor to infer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- port

		- 
		  Port of the input or output tensor. Use the following methods to get the ports:
		  
		  * :ref:`ov::Model::input() <doxid-classov_1_1_model_1a9bf0166a1f9005222cb9a2f68a3b9a4c>`
		  
		  * :ref:`ov::Model::inputs() <doxid-classov_1_1_model_1a7121b50a2990b63eb6a73945f0cae089>`
		  
		  * :ref:`ov::Model::outputs() <doxid-classov_1_1_model_1a89c629856666f1064cf0418c432004f0>`
		  
		  * :ref:`ov::Model::outputs() <doxid-classov_1_1_model_1a89c629856666f1064cf0418c432004f0>`
		  
		  * :ref:`ov::CompiledModel::input() <doxid-classov_1_1_compiled_model_1a55f2867a43fb78829f9901c52f9ccea9>`
		  
		  * :ref:`ov::CompiledModel::inputs() <doxid-classov_1_1_compiled_model_1a39ec975bfc52054607b8800a6ee1fc2c>`
		  
		  * :ref:`ov::CompiledModel::outputs() <doxid-classov_1_1_compiled_model_1a0736f9b1443d5b564fc5b625e7aeb310>`
		  
		  * :ref:`ov::CompiledModel::outputs() <doxid-classov_1_1_compiled_model_1a0736f9b1443d5b564fc5b625e7aeb310>`

	*
		- tensor

		- Reference to a tensor. The element_type and shape of a tensor must match the model's input/output element_type and size.

.. _doxid-classov_1_1_infer_request_1a51a945021f2559c18cdbfa0c8ce66cb4:
.. index:: pair: function; set_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_tensor(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& port, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an input/output tensor to infer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- port

		- 
		  Port of the input or output tensor. Use the following methods to get the ports:
		  
		  * :ref:`ov::Model::input() <doxid-classov_1_1_model_1a9bf0166a1f9005222cb9a2f68a3b9a4c>`
		  
		  * :ref:`ov::Model::inputs() <doxid-classov_1_1_model_1a7121b50a2990b63eb6a73945f0cae089>`
		  
		  * :ref:`ov::Model::outputs() <doxid-classov_1_1_model_1a89c629856666f1064cf0418c432004f0>`
		  
		  * :ref:`ov::Model::outputs() <doxid-classov_1_1_model_1a89c629856666f1064cf0418c432004f0>`
		  
		  * :ref:`ov::CompiledModel::input() <doxid-classov_1_1_compiled_model_1a55f2867a43fb78829f9901c52f9ccea9>`
		  
		  * :ref:`ov::CompiledModel::inputs() <doxid-classov_1_1_compiled_model_1a39ec975bfc52054607b8800a6ee1fc2c>`
		  
		  * :ref:`ov::CompiledModel::outputs() <doxid-classov_1_1_compiled_model_1a0736f9b1443d5b564fc5b625e7aeb310>`
		  
		  * :ref:`ov::CompiledModel::outputs() <doxid-classov_1_1_compiled_model_1a0736f9b1443d5b564fc5b625e7aeb310>`

	*
		- tensor

		- Reference to a tensor. The element_type and shape of a tensor must match the model's input/output element_type and size.

.. _doxid-classov_1_1_infer_request_1a935a952c07cc7130a64614d0952db997:
.. index:: pair: function; set_tensors

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_tensors(
		const std::string& tensor_name,
		const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors
		)

Sets a batch of tensors for input data to infer by tensor name. :ref:`Model <doxid-classov_1_1_model>` input must have batch dimension, and the number of ``tensors`` must match the batch size. The current version supports setting tensors to model inputs only. If ``tensor_name`` is associated with output (or any other non-input node), an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- Name of the input tensor.

	*
		- tensors

		- :ref:`Input <doxid-classov_1_1_input>` tensors for batched infer request. The type of each tensor must match the model input element type and shape (except batch dimension). Total size of tensors must match the input size.

.. _doxid-classov_1_1_infer_request_1a28e18a17764134c47d26482d82ce9b65:
.. index:: pair: function; set_tensors

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_tensors(
		const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& port,
		const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors
		)

Sets a batch of tensors for input data to infer by input port. :ref:`Model <doxid-classov_1_1_model>` input must have batch dimension, and the number of ``tensors`` must match the batch size. The current version supports setting tensors to model inputs only. If ``port`` is associated with output (or any other non-input node), an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- port

		- Port of the input tensor.

	*
		- tensors

		- :ref:`Input <doxid-classov_1_1_input>` tensors for batched infer request. The type of each tensor must match the model input element type and shape (except batch dimension). Total size of tensors must match the input size.

.. _doxid-classov_1_1_infer_request_1a5ddca7af7faffa2c90fd600a3f84aa6e:
.. index:: pair: function; set_input_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_input_tensor(size_t idx, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an input tensor to infer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- idx

		- Index of the input tensor. If ``idx`` is greater than the number of model inputs, an exception is thrown.

	*
		- tensor

		- Reference to the tensor. The element_type and shape of the tensor must match the model's input/output element_type and size.

.. _doxid-classov_1_1_infer_request_1a5f3640729c5e9e197bad73dd3260573c:
.. index:: pair: function; set_input_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_input_tensor(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an input tensor to infer models with single input.

If model has several inputs, an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- Reference to the input tensor.

.. _doxid-classov_1_1_infer_request_1af847095ee6e85141fb3ef35f1556d89c:
.. index:: pair: function; set_input_tensors

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_input_tensors(const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors)

Sets a batch of tensors for single input data. :ref:`Model <doxid-classov_1_1_model>` input must have batch dimension, and the number of ``tensors`` must match the batch size.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensors

		- :ref:`Input <doxid-classov_1_1_input>` tensors for batched infer request. The type of each tensor must match the model input element type and shape (except batch dimension). Total size of tensors must match the input size.

.. _doxid-classov_1_1_infer_request_1a5fef80b34aca795d8b426ad93c93fe0f:
.. index:: pair: function; set_input_tensors

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_input_tensors(size_t idx, const std::vector<:ref:`Tensor<doxid-classov_1_1_tensor>`>& tensors)

Sets a batch of tensors for input data to infer by input name. :ref:`Model <doxid-classov_1_1_model>` input must have batch dimension, and number of ``tensors`` must match the batch size.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- idx

		- Name of the input tensor.

	*
		- tensors

		- :ref:`Input <doxid-classov_1_1_input>` tensors for batched infer request. The type of each tensor must match the model input element type and shape (except batch dimension). Total size of tensors must match the input size.

.. _doxid-classov_1_1_infer_request_1a3e93efd003301c4de6b0181163e7d14d:
.. index:: pair: function; set_output_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_output_tensor(size_t idx, const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an output tensor to infer.

Index of the input preserved accross :ref:`ov::Model <doxid-classov_1_1_model>`, :ref:`ov::CompiledModel <doxid-classov_1_1_compiled_model>`, and :ref:`ov::InferRequest <doxid-classov_1_1_infer_request>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- idx

		- Index of the output tensor.

	*
		- tensor

		- Reference to the output tensor. The type of the tensor must match the model output element type and shape.

.. _doxid-classov_1_1_infer_request_1ab2844540aa73e122021882767656fbb2:
.. index:: pair: function; set_output_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_output_tensor(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Sets an output tensor to infer models with single output.

If model has several outputs, an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- Reference to the output tensor.

.. _doxid-classov_1_1_infer_request_1a75b8da7c6b00686bede600dddceaffc4:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_tensor(const std::string& tensor_name)

Gets an input/output tensor for inference by tensor name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- Name of a tensor to get.



.. rubric:: Returns:

The tensor with name ``tensor_name``. If the tensor is not found, an exception is thrown.

.. _doxid-classov_1_1_infer_request_1ae95479408beb5d091037ef8221ba9940:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_tensor(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& port)

Gets an input/output tensor for inference.

If the tensor with the specified ``port`` is not found, an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- port

		- Port of the tensor to get.



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` for the port ``port``.

.. _doxid-classov_1_1_infer_request_1ac30bcc9c86bdf2e89165c562f009e70a:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_tensor(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& port)

Gets an input/output tensor for inference.

If the tensor with the specified ``port`` is not found, an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- port

		- Port of the tensor to get.



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` for the port ``port``.

.. _doxid-classov_1_1_infer_request_1a5f0bc1ab40de6a7a12136b4a4e6a8b54:
.. index:: pair: function; get_input_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_input_tensor(size_t idx)

Gets an input tensor for inference.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- idx

		- Index of the tensor to get.



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` with the input index ``idx``. If the tensor with the specified ``idx`` is not found, an exception is thrown.

.. _doxid-classov_1_1_infer_request_1a7e857e8a9f13114289db2cbfe831763c:
.. index:: pair: function; get_input_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_input_tensor()

Gets an input tensor for inference.



.. rubric:: Returns:

The input tensor for the model. If model has several inputs, an exception is thrown.

.. _doxid-classov_1_1_infer_request_1a350159a8d967022db46633eed50d073a:
.. index:: pair: function; get_output_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_output_tensor(size_t idx)

Gets an output tensor for inference.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- idx

		- Index of the tensor to get.



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` with the output index ``idx``. If the tensor with the specified ``idx`` is not found, an exception is thrown.

.. _doxid-classov_1_1_infer_request_1a9bf7bf67c58858bda86ae01e83cd14c1:
.. index:: pair: function; get_output_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_output_tensor()

Gets an output tensor for inference.



.. rubric:: Returns:

:ref:`Output <doxid-classov_1_1_output>` tensor for the model. If model has several outputs, an exception is thrown.

.. _doxid-classov_1_1_infer_request_1abcb7facc9f7c4b9226a1fd343e56958d:
.. index:: pair: function; infer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void infer()

Infers specified input(s) in synchronous mode.

It blocks all methods of :ref:`InferRequest <doxid-classov_1_1_infer_request>` while request is ongoing (running or waiting in a queue). Calling any method leads to throwning the :ref:`ov::Busy <doxid-classov_1_1_busy>` exception.

.. _doxid-classov_1_1_infer_request_1aa100b080271f057ab5f98d1832af414d:
.. index:: pair: function; cancel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void cancel()

Cancels inference request.

.. _doxid-classov_1_1_infer_request_1af70dbbd38ffb928ce407a22bd781b6d5:
.. index:: pair: function; get_profiling_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ProfilingInfo<doxid-structov_1_1_profiling_info>`> get_profiling_info() const

Queries performance measures per layer to identify the most time consuming operation.

Not all plugins provide meaningful data.



.. rubric:: Returns:

Vector of profiling information for operations in a model.

.. _doxid-classov_1_1_infer_request_1a5a05ae4352f804c865e11f5d68b983d5:
.. index:: pair: function; start_async

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void start_async()

Starts inference of specified input(s) in asynchronous mode.

It returns immediately. Inference starts also immediately. Calling any method while the request in a running state leads to throwning the :ref:`ov::Busy <doxid-classov_1_1_busy>` exception.

.. _doxid-classov_1_1_infer_request_1ab0e0739da45789d816f8b5584a0b5691:
.. index:: pair: function; wait

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void wait()

Waits for the result to become available. Blocks until the result becomes available.

.. _doxid-classov_1_1_infer_request_1a94d6d52e03d2ad20310a1e0fdd807e9e:
.. index:: pair: function; wait_for

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool wait_for(const std::chrono::milliseconds timeout)

Waits for the result to become available. Blocks until the specified timeout has elapsed or the result becomes available, whichever comes first.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- timeout

		- Maximum duration, in milliseconds, to block for.



.. rubric:: Returns:

True if inference request is ready and false, otherwise.

.. _doxid-classov_1_1_infer_request_1afba2a10162ab356728ec8901973e8f02:
.. index:: pair: function; set_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_callback(std::function<void(std::exception_ptr)> callback)

Sets a callback std::function that is called on success or failure of an asynchronous request.

Do not capture strong references to OpenVINO runtime objects into callback. Following objects should not be captured like:

* :ref:`ov::InferRequest <doxid-classov_1_1_infer_request>`

* ov::ExecutableNetwork

* :ref:`ov::Core <doxid-classov_1_1_core>` As specified objects implement shared reference concept do not capture this objects by value. It can lead to memory leaks or undefined behaviour! Try to use weak references or pointers.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- callback

		- callback object which will be called on when inference finish.

.. _doxid-classov_1_1_infer_request_1ac415100cc002db60b0afd871401345b5:
.. index:: pair: function; query_state

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`VariableState<doxid-classov_1_1_variable_state>`> query_state()

Gets state control interface for the given infer request.

State control essential for recurrent models.



.. rubric:: Returns:

Vector of Variable State objects.

.. _doxid-classov_1_1_infer_request_1ad295894c4d65d0e0dc260d4a6cf287eb:
.. index:: pair: function; get_compiled_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` get_compiled_model()

Returns a compiled model that creates this inference request.



.. rubric:: Returns:

Compiled model object.

.. _doxid-classov_1_1_infer_request_1a4b10bba9b6b8331b4fce992c737668d2:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Checks if the current :ref:`InferRequest <doxid-classov_1_1_infer_request>` object is not initialized.



.. rubric:: Returns:

True if the current :ref:`InferRequest <doxid-classov_1_1_infer_request>` object is not initialized; false, otherwise.

.. _doxid-classov_1_1_infer_request_1a324eb815c65cc72f4d2b534e950b0c34:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Checks if the current :ref:`InferRequest <doxid-classov_1_1_infer_request>` object is initialized.



.. rubric:: Returns:

True if the current :ref:`InferRequest <doxid-classov_1_1_infer_request>` object is initialized; false, otherwise.

.. _doxid-classov_1_1_infer_request_1a659e8621129aa8aff0db2daace42a388:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const InferRequest& other) const

Compares whether this request wraps the same impl underneath.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another inference request.



.. rubric:: Returns:

True if the current :ref:`InferRequest <doxid-classov_1_1_infer_request>` object does not wrap the same impl as the operator's arg.

.. _doxid-classov_1_1_infer_request_1a2f0bdc369c5e54a4f1f49e85744b7ee6:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const InferRequest& other) const

Compares whether this request wraps the same impl underneath.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another inference request.



.. rubric:: Returns:

True if the current :ref:`InferRequest <doxid-classov_1_1_infer_request>` object wraps the same impl as the operator's arg.


