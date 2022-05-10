.. index:: pair: class; InferenceEngine::IExecutableNetwork
.. _doxid-class_inference_engine_1_1_i_executable_network:

class InferenceEngine::IExecutableNetwork
=========================================



Overview
~~~~~~~~

This is an interface of an executable network. :ref:`More...<details-class_inference_engine_1_1_i_executable_network>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iexecutable_network.hpp>
	
	class IExecutableNetwork: public std::enable_shared_from_this< IExecutableNetwork >
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<IExecutableNetwork> :ref:`Ptr<doxid-class_inference_engine_1_1_i_executable_network_1ac04ef0e735335e1e62f6cfcaec533ad2>`;

		// methods
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetOutputsInfo<doxid-class_inference_engine_1_1_i_executable_network_1a478fb61c5b8aba1891be9be22e4dd0c2>`(
			:ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>`& out,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetInputsInfo<doxid-class_inference_engine_1_1_i_executable_network_1aaa7989a24ce6aeb0f4cf1ca52dbc59fe>`(
			:ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>`& inputs,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`CreateInferRequest<doxid-class_inference_engine_1_1_i_executable_network_1a27caaa0ed26c441a4994d53477f9dddc>`(
			:ref:`IInferRequest::Ptr<doxid-class_inference_engine_1_1_i_infer_request_1a3a97a4462a185eed9e86c1f0f0261ab3>`& req,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Export<doxid-class_inference_engine_1_1_i_executable_network_1acb387ffedbcb00e7ddda41828b63d58c>`(
			const std::string& modelFileName,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`Export<doxid-class_inference_engine_1_1_i_executable_network_1a437948e1677395dfe29a72704eac55f3>`(std::ostream& networkModel, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetExecGraphInfo<doxid-class_inference_engine_1_1_i_executable_network_1a761c2a454d46b66ed6538ed9ab42d85a>`(
			:ref:`ICNNNetwork::Ptr<doxid-class_inference_engine_1_1_i_c_n_n_network_1a05b6f650d23e571e03da46a3a89db633>`& graphPtr,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`SetConfig<doxid-class_inference_engine_1_1_i_executable_network_1ab0960afa5470727239d334fa1de5d04e>`(
			const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetConfig<doxid-class_inference_engine_1_1_i_executable_network_1ad0c289951019aef4a7950d58517c2c13>`(
			const std::string& name,
			:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`& result,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetMetric<doxid-class_inference_engine_1_1_i_executable_network_1a6ea9d412e4a520c82a4c92edf113f485>`(
			const std::string& name,
			:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`& result,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`GetContext<doxid-class_inference_engine_1_1_i_executable_network_1a4d3a5de698e62a8c6b43a92d237e1678>`(
			:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`& pContext,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;

	protected:
	};
.. _details-class_inference_engine_1_1_i_executable_network:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is an interface of an executable network.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_executable_network_1ac04ef0e735335e1e62f6cfcaec533ad2:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IExecutableNetwork> Ptr

A smart pointer to the current :ref:`IExecutableNetwork <doxid-class_inference_engine_1_1_i_executable_network>` object.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_executable_network_1a478fb61c5b8aba1891be9be22e4dd0c2:
.. index:: pair: function; GetOutputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetOutputsInfo(
		:ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>`& out,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Gets the Executable network output :ref:`Data <doxid-class_inference_engine_1_1_data>` node information.

The received info is stored in the given :ref:`InferenceEngine::ConstOutputsDataMap <doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` node. This method need to be called to find output names for using them later when calling :ref:`InferenceEngine::InferRequest::GetBlob <doxid-class_inference_engine_1_1_infer_request_1a9601a4cda3f309181af34feedf1b914c>` or :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- out

		- Reference to the :ref:`InferenceEngine::ConstOutputsDataMap <doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` object

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_executable_network_1aaa7989a24ce6aeb0f4cf1ca52dbc59fe:
.. index:: pair: function; GetInputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetInputsInfo(
		:ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>`& inputs,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Gets the executable network input :ref:`Data <doxid-class_inference_engine_1_1_data>` node information.

The received info is stored in the given :ref:`InferenceEngine::ConstInputsDataMap <doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` object. This method need to be called to find out input names for using them later when calling :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- Reference to :ref:`InferenceEngine::ConstInputsDataMap <doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` object.

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_executable_network_1a27caaa0ed26c441a4994d53477f9dddc:
.. index:: pair: function; CreateInferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` CreateInferRequest(
		:ref:`IInferRequest::Ptr<doxid-class_inference_engine_1_1_i_infer_request_1a3a97a4462a185eed9e86c1f0f0261ab3>`& req,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Creates an inference request object used to infer the network.

The created request has allocated input and output blobs (that can be changed later).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- req

		- Shared pointer to the created request object

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_executable_network_1acb387ffedbcb00e7ddda41828b63d58c:
.. index:: pair: function; Export

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Export(
		const std::string& modelFileName,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Exports the current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelFileName

		- Full path to the location of the exported file

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success



.. rubric:: See also:

:ref:`Core::ImportNetwork <doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013>`

.. _doxid-class_inference_engine_1_1_i_executable_network_1a437948e1677395dfe29a72704eac55f3:
.. index:: pair: function; Export

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` Export(std::ostream& networkModel, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Exports the current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- Network model output stream

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success



.. rubric:: See also:

:ref:`Core::ImportNetwork <doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013>`

.. _doxid-class_inference_engine_1_1_i_executable_network_1a761c2a454d46b66ed6538ed9ab42d85a:
.. index:: pair: function; GetExecGraphInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetExecGraphInfo(
		:ref:`ICNNNetwork::Ptr<doxid-class_inference_engine_1_1_i_c_n_n_network_1a05b6f650d23e571e03da46a3a89db633>`& graphPtr,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Get executable graph information from a device.

Deprecated Use :ref:`InferenceEngine::ExecutableNetwork::GetExecGraphInfo <doxid-class_inference_engine_1_1_executable_network_1a00db8bf2706042fb616e0f6683c6a847>` instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- graphPtr

		- network ptr to store executable graph information

	*
		- resp

		- Optional: pointer to an already allocated object to contain information in case of failure



.. rubric:: Returns:

Status code of the operation: :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` (0) for success

.. _doxid-class_inference_engine_1_1_i_executable_network_1ab0960afa5470727239d334fa1de5d04e:
.. index:: pair: function; SetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` SetConfig(
		const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Sets configuration for current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- config

		- Map of pairs: (config parameter name, config parameter value)

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

code of the operation. :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` if succeeded

.. _doxid-class_inference_engine_1_1_i_executable_network_1ad0c289951019aef4a7950d58517c2c13:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetConfig(
		const std::string& name,
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`& result,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Gets configuration for current executable network.

The method is responsible to extract information which affects executable network execution. The list of supported configuration values can be extracted via :ref:`ExecutableNetwork::GetMetric <doxid-class_inference_engine_1_1_executable_network_1a5b38590cad3a68144c679af5f5a6090d>` with the SUPPORTED_CONFIG_KEYS key, but some of these keys cannot be changed dymanically, e.g. DEVICE_ID cannot changed if an executable network has already been compiled for particular device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- config key, can be found in ``ie_plugin_config.hpp``

	*
		- result

		- value of config corresponding to config key

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

code of the operation. :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` if succeeded

.. _doxid-class_inference_engine_1_1_i_executable_network_1a6ea9d412e4a520c82a4c92edf113f485:
.. index:: pair: function; GetMetric

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetMetric(
		const std::string& name,
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`& result,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Gets general runtime metric for an executable network.

It can be network name, actual device ID on which executable network is running or all other properties which cannot be changed dynamically.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- metric name to request

	*
		- result

		- metric value corresponding to metric key

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

code of the operation. :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` if succeeded

.. _doxid-class_inference_engine_1_1_i_executable_network_1a4d3a5de698e62a8c6b43a92d237e1678:
.. index:: pair: function; GetContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` GetContext(
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`& pContext,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Gets shared context used to create an executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pContext

		- Reference to a pointer that will receive resulting shared context object ptr

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

code of the operation. :ref:`InferenceEngine::OK <doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>` if succeeded


