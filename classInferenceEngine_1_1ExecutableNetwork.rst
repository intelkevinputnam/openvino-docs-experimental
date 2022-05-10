.. index:: pair: class; InferenceEngine::ExecutableNetwork
.. _doxid-class_inference_engine_1_1_executable_network:

class InferenceEngine::ExecutableNetwork
========================================



Overview
~~~~~~~~

This is an interface of an executable network. :ref:`More...<details-class_inference_engine_1_1_executable_network>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_executable_network.hpp>
	
	class ExecutableNetwork
	{
	public:
		// construction
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network_1a9e074226bdcf46324f148a5aea44c82e>`();
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network_1a6cdac0283fd253a1d8b5443821999ddb>`(const ExecutableNetwork& other);
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network_1a9af30d9de119e514d19196dad920a8c9>`(ExecutableNetwork&& other);

		// methods
	
		ExecutableNetwork& :ref:`operator =<doxid-class_inference_engine_1_1_executable_network_1a096951ea87e7eec264c292c4ccff06c9>` (const ExecutableNetwork& other);
		ExecutableNetwork& :ref:`operator =<doxid-class_inference_engine_1_1_executable_network_1a3635142743ae4335a99c288d70b1414f>` (ExecutableNetwork&& other);
		:ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` :ref:`GetOutputsInfo<doxid-class_inference_engine_1_1_executable_network_1a02acc33e0b3feb52123f0d36a023d980>`() const;
		:ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` :ref:`GetInputsInfo<doxid-class_inference_engine_1_1_executable_network_1a89bd4c0b76013b8f2227e7c2930b57ba>`() const;
		:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request>` :ref:`CreateInferRequest<doxid-class_inference_engine_1_1_executable_network_1a5516b9b68b8fa0bcc72f19bc812ccf47>`();
		void :ref:`Export<doxid-class_inference_engine_1_1_executable_network_1aadc38371f9ebaabaf61a95ab646a50ae>`(const std::string& modelFileName);
		void :ref:`Export<doxid-class_inference_engine_1_1_executable_network_1af635c047bd8d67996940f14b3bd4dc95>`(std::ostream& networkModel);
		:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`GetExecGraphInfo<doxid-class_inference_engine_1_1_executable_network_1a00db8bf2706042fb616e0f6683c6a847>`();
		void :ref:`SetConfig<doxid-class_inference_engine_1_1_executable_network_1aa1ed6418b25be96a413c452ca8c1480a>`(const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config);
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-class_inference_engine_1_1_executable_network_1af43953e9d84965914d1ce50f90480145>`(const std::string& name) const;
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetMetric<doxid-class_inference_engine_1_1_executable_network_1a5b38590cad3a68144c679af5f5a6090d>`(const std::string& name) const;
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`GetContext<doxid-class_inference_engine_1_1_executable_network_1a42baa930646e435f5027425c23052d7d>`() const;
		bool :ref:`operator !<doxid-class_inference_engine_1_1_executable_network_1a77feb1084af838d71ce78ac001805fb2>` () const;
		:ref:`operator bool<doxid-class_inference_engine_1_1_executable_network_1a6494e4cb970c7f08701e6eb7530be21f>` () const;
		void :ref:`reset<doxid-class_inference_engine_1_1_executable_network_1a047641f157ef8745ba3a7d0017386af3>`(std::shared_ptr<:ref:`IExecutableNetwork<doxid-class_inference_engine_1_1_i_executable_network>`> newActual);
		:ref:`operator std::shared_ptr< IExecutableNetwork ><doxid-class_inference_engine_1_1_executable_network_1ab9899dca8b19f723bff911a581a3cce0>` ();
		:ref:`InferRequest::Ptr<doxid-class_inference_engine_1_1_infer_request_1aa725364c5565a1cbe4d0e9245a4cb055>` :ref:`CreateInferRequestPtr<doxid-class_inference_engine_1_1_executable_network_1a6579210c5507855ddf3306df28682e9c>`();
	};
.. _details-class_inference_engine_1_1_executable_network:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is an interface of an executable network.

Construction
------------

.. _doxid-class_inference_engine_1_1_executable_network_1a9e074226bdcf46324f148a5aea44c82e:
.. index:: pair: function; ExecutableNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ExecutableNetwork()

Default constructor.

.. _doxid-class_inference_engine_1_1_executable_network_1a6cdac0283fd253a1d8b5443821999ddb:
.. index:: pair: function; ExecutableNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ExecutableNetwork(const ExecutableNetwork& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object

.. _doxid-class_inference_engine_1_1_executable_network_1a9af30d9de119e514d19196dad920a8c9:
.. index:: pair: function; ExecutableNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ExecutableNetwork(ExecutableNetwork&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object

Methods
-------

.. _doxid-class_inference_engine_1_1_executable_network_1a096951ea87e7eec264c292c4ccff06c9:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ExecutableNetwork& operator = (const ExecutableNetwork& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-class_inference_engine_1_1_executable_network_1a3635142743ae4335a99c288d70b1414f:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ExecutableNetwork& operator = (ExecutableNetwork&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-class_inference_engine_1_1_executable_network_1a02acc33e0b3feb52123f0d36a023d980:
.. index:: pair: function; GetOutputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` GetOutputsInfo() const

Gets the Executable network output :ref:`Data <doxid-class_inference_engine_1_1_data>` node information.

The received info is stored in the given :ref:`InferenceEngine::ConstOutputsDataMap <doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` node. This method need to be called to find output names for using them later when calling :ref:`InferenceEngine::InferRequest::GetBlob <doxid-class_inference_engine_1_1_infer_request_1a9601a4cda3f309181af34feedf1b914c>` or :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`



.. rubric:: Returns:

A collection that contains string as key, and const :ref:`Data <doxid-class_inference_engine_1_1_data>` smart pointer as value

.. _doxid-class_inference_engine_1_1_executable_network_1a89bd4c0b76013b8f2227e7c2930b57ba:
.. index:: pair: function; GetInputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` GetInputsInfo() const

Gets the executable network input :ref:`Data <doxid-class_inference_engine_1_1_data>` node information.

The received info is stored in the given :ref:`InferenceEngine::ConstInputsDataMap <doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` object. This method need to be called to find out input names for using them later when calling :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`



.. rubric:: Returns:

A collection that contains string as key, and const :ref:`InputInfo <doxid-class_inference_engine_1_1_input_info>` smart pointer as value

.. _doxid-class_inference_engine_1_1_executable_network_1a5516b9b68b8fa0bcc72f19bc812ccf47:
.. index:: pair: function; CreateInferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferRequest<doxid-class_inference_engine_1_1_infer_request>` CreateInferRequest()

Creates an inference request object used to infer the network.

The created request has allocated input and output blobs (that can be changed later).



.. rubric:: Returns:

:ref:`InferRequest <doxid-class_inference_engine_1_1_infer_request>` object

.. _doxid-class_inference_engine_1_1_executable_network_1aadc38371f9ebaabaf61a95ab646a50ae:
.. index:: pair: function; Export

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void Export(const std::string& modelFileName)

Exports the current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelFileName

		- Full path to the location of the exported file



.. rubric:: See also:

:ref:`Core::ImportNetwork <doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013>`

.. _doxid-class_inference_engine_1_1_executable_network_1af635c047bd8d67996940f14b3bd4dc95:
.. index:: pair: function; Export

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void Export(std::ostream& networkModel)

Exports the current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- Network model output stream



.. rubric:: See also:

:ref:`Core::ImportNetwork <doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013>`

.. _doxid-class_inference_engine_1_1_executable_network_1a00db8bf2706042fb616e0f6683c6a847:
.. index:: pair: function; GetExecGraphInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` GetExecGraphInfo()

Get executable graph information from a device.

Wraps :ref:`IExecutableNetwork::GetExecGraphInfo <doxid-class_inference_engine_1_1_i_executable_network_1a761c2a454d46b66ed6538ed9ab42d85a>`.



.. rubric:: Returns:

CNNetwork containing Executable Graph Info

.. _doxid-class_inference_engine_1_1_executable_network_1aa1ed6418b25be96a413c452ca8c1480a:
.. index:: pair: function; SetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetConfig(const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config)

Sets configuration for current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- config

		- Map of pairs: (config parameter name, config parameter value)

.. _doxid-class_inference_engine_1_1_executable_network_1af43953e9d84965914d1ce50f90480145:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetConfig(const std::string& name) const

Gets configuration for current executable network.

The method is responsible to extract information which affects executable network execution. The list of supported configuration values can be extracted via :ref:`ExecutableNetwork::GetMetric <doxid-class_inference_engine_1_1_executable_network_1a5b38590cad3a68144c679af5f5a6090d>` with the SUPPORTED_CONFIG_KEYS key, but some of these keys cannot be changed dynamically, e.g. DEVICE_ID cannot changed if an executable network has already been compiled for particular device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- config key, can be found in ``ie_plugin_config.hpp``



.. rubric:: Returns:

Configuration parameter value

.. _doxid-class_inference_engine_1_1_executable_network_1a5b38590cad3a68144c679af5f5a6090d:
.. index:: pair: function; GetMetric

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetMetric(const std::string& name) const

Gets general runtime metric for an executable network.

It can be network name, actual device ID on which executable network is running or all other properties which cannot be changed dynamically.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- metric name to request



.. rubric:: Returns:

Metric parameter value

.. _doxid-class_inference_engine_1_1_executable_network_1a42baa930646e435f5027425c23052d7d:
.. index:: pair: function; GetContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` GetContext() const

Returns pointer to plugin-specific shared context on remote accelerator device that was used to create this :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>`.



.. rubric:: Returns:

A context

.. _doxid-class_inference_engine_1_1_executable_network_1a77feb1084af838d71ce78ac001805fb2:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Checks if current :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object is not initialized.



.. rubric:: Returns:

true if current :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object is not initialized, false - otherwise

.. _doxid-class_inference_engine_1_1_executable_network_1a6494e4cb970c7f08701e6eb7530be21f:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Checks if current :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object is initialized.



.. rubric:: Returns:

true if current :ref:`ExecutableNetwork <doxid-class_inference_engine_1_1_executable_network>` object is initialized, false - otherwise

.. _doxid-class_inference_engine_1_1_executable_network_1a047641f157ef8745ba3a7d0017386af3:
.. index:: pair: function; reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reset(std::shared_ptr<:ref:`IExecutableNetwork<doxid-class_inference_engine_1_1_i_executable_network>`> newActual)

reset owned object to new pointer.

Deprecated The method Will be removed

Essential for cases when simultaneously loaded networks not expected.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- newActual

		- actual pointed object

.. _doxid-class_inference_engine_1_1_executable_network_1ab9899dca8b19f723bff911a581a3cce0:
.. index:: pair: function; operator std::shared_ptr< IExecutableNetwork >

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator std::shared_ptr< IExecutableNetwork > ()

cast operator is used when this wrapper initialized by LoadNetwork

Deprecated Will be removed. Use operator bool



.. rubric:: Returns:

A shared pointer to :ref:`IExecutableNetwork <doxid-class_inference_engine_1_1_i_executable_network>` interface.

.. _doxid-class_inference_engine_1_1_executable_network_1a6579210c5507855ddf3306df28682e9c:
.. index:: pair: function; CreateInferRequestPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferRequest::Ptr<doxid-class_inference_engine_1_1_infer_request_1aa725364c5565a1cbe4d0e9245a4cb055>` CreateInferRequestPtr()

Creates an inference request object used to infer the network.

Deprecated Use :ref:`ExecutableNetwork::CreateInferRequest <doxid-class_inference_engine_1_1_executable_network_1a5516b9b68b8fa0bcc72f19bc812ccf47>`

Wraps :ref:`IExecutableNetwork::CreateInferRequest <doxid-class_inference_engine_1_1_i_executable_network_1a27caaa0ed26c441a4994d53477f9dddc>`.



.. rubric:: Returns:

shared pointer on :ref:`InferenceEngine::InferRequest <doxid-class_inference_engine_1_1_infer_request>` object


