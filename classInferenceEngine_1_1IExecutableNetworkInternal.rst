.. index:: pair: interface; InferenceEngine::IExecutableNetworkInternal
.. _doxid-class_inference_engine_1_1_i_executable_network_internal:

interface InferenceEngine::IExecutableNetworkInternal
=====================================================



Overview
~~~~~~~~

An internal API of executable network to be implemented by plugin,. :ref:`More...<details-class_inference_engine_1_1_i_executable_network_internal>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iexecutable_network_internal.hpp>
	
	template IExecutableNetworkInternal: public std::enable_shared_from_this< IExecutableNetworkInternal >
	{
		// typedefs
	
		typedef std::shared_ptr<IExecutableNetworkInternal> :ref:`Ptr<doxid-class_inference_engine_1_1_i_executable_network_internal_1a264e3e04130a2e44d0b257ae63c9feae>`;

		// methods
	
		virtual void :ref:`setNetworkInputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a516604bd1cedd1072d82eb82170aed18>`(const :ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& networkInputs);
		virtual void :ref:`setNetworkOutputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a6b795c8f85fe7acc1819e230bce6e4da>`(const :ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& networkOutputs);
		virtual void :ref:`setInputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a9417aa5772082d01cee2b19185835ad1>`(const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& params);
		virtual const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`getInputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1af02e0a16bf01c39514b005edd9743d7a>`() const;
		virtual void :ref:`setOutputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1ae529d59d4e19a45f60ea03af93e32fb9>`(const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& results);
		virtual const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`getOutputs<doxid-class_inference_engine_1_1_i_executable_network_internal_1a153bdd4f0da982ada15e257e2fd8d620>`() const;
		virtual :ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` :ref:`GetOutputsInfo<doxid-class_inference_engine_1_1_i_executable_network_internal_1ac6fbce66b52b33bb62709803b25f2a6e>`() const;
		virtual :ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` :ref:`GetInputsInfo<doxid-class_inference_engine_1_1_i_executable_network_internal_1a1529cab4d8385e21ef394b817f8c2230>`() const;
		virtual std::shared_ptr<:ref:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal>`> :ref:`CreateInferRequest<doxid-class_inference_engine_1_1_i_executable_network_internal_1ab5d5797a7ef239eeb20d1c3eadf1bd73>`();
		virtual void :ref:`Export<doxid-class_inference_engine_1_1_i_executable_network_internal_1a057bca9b0f955c03190bdf77635e9516>`(const std::string& modelFileName);
		virtual void :ref:`Export<doxid-class_inference_engine_1_1_i_executable_network_internal_1a2b5e212158cd5bf3a2f903cd405fdd3d>`(std::ostream& networkModel);
		virtual std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`GetExecGraphInfo<doxid-class_inference_engine_1_1_i_executable_network_internal_1aeb29d9f35b340496272f785d7be4f097>`();
		virtual void :ref:`SetPointerToPlugin<doxid-class_inference_engine_1_1_i_executable_network_internal_1a13df5cff9daf69a68365509ad11a5b1f>`(const std::shared_ptr<:ref:`IInferencePlugin<doxid-class_inference_engine_1_1_i_inference_plugin>`>& plugin);
		virtual void :ref:`SetConfig<doxid-class_inference_engine_1_1_i_executable_network_internal_1a66bc34d51b798322d29ec1b1a8332faa>`(const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config);
		virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-class_inference_engine_1_1_i_executable_network_internal_1aab6b3c29e3fec7400548b0af1808a772>`(const std::string& name) const;
		virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetMetric<doxid-class_inference_engine_1_1_i_executable_network_internal_1abff44a61825a0da77a4a329225431708>`(const std::string& name) const;
		virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`GetContext<doxid-class_inference_engine_1_1_i_executable_network_internal_1a3a14f4c13bf0ba5470278d762cefc356>`() const;

	protected:
	};

	// direct descendants

	class :ref:`ExecutableNetworkThreadSafeDefault<doxid-class_inference_engine_1_1_executable_network_thread_safe_default>`;
.. _details-class_inference_engine_1_1_i_executable_network_internal:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An internal API of executable network to be implemented by plugin,.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a264e3e04130a2e44d0b257ae63c9feae:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IExecutableNetworkInternal> Ptr

A shared pointer to :ref:`IExecutableNetworkInternal <doxid-class_inference_engine_1_1_i_executable_network_internal>` interface.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a516604bd1cedd1072d82eb82170aed18:
.. index:: pair: function; setNetworkInputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setNetworkInputs(const :ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& networkInputs)

Sets the network inputs info.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkInputs

		- The network inputs info

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a6b795c8f85fe7acc1819e230bce6e4da:
.. index:: pair: function; setNetworkOutputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setNetworkOutputs(const :ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& networkOutputs)

Sets the network outputs data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkOutputs

		- The network outputs

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a9417aa5772082d01cee2b19185835ad1:
.. index:: pair: function; setInputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setInputs(const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& params)

Sets the network parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- params

		- The network parameters

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1af02e0a16bf01c39514b005edd9743d7a:
.. index:: pair: function; getInputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& getInputs() const

Returns the network parameters.

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1ae529d59d4e19a45f60ea03af93e32fb9:
.. index:: pair: function; setOutputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setOutputs(const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& results)

Sets the network results.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- results

		- The network results

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a153bdd4f0da982ada15e257e2fd8d620:
.. index:: pair: function; getOutputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::vector<std::shared_ptr<const :ref:`ov::Node<doxid-classov_1_1_node>`>>& getOutputs() const

Returns the network results.

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1ac6fbce66b52b33bb62709803b25f2a6e:
.. index:: pair: function; GetOutputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ConstOutputsDataMap<doxid-namespace_inference_engine_1a226d61fcc2c0bb77b4e4351871e1936d>` GetOutputsInfo() const

Gets the Executable network output :ref:`Data <doxid-class_inference_engine_1_1_data>` node information. The received info is stored in the given :ref:`Data <doxid-class_inference_engine_1_1_data>` node.



.. rubric:: Returns:

out Reference to the ConstOutputsDataMap object

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a1529cab4d8385e21ef394b817f8c2230:
.. index:: pair: function; GetInputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ConstInputsDataMap<doxid-namespace_inference_engine_1a3f61af4b68481a688f550b63a19909d5>` GetInputsInfo() const

Gets the Executable network input :ref:`Data <doxid-class_inference_engine_1_1_data>` node information. The received info is stored in the given InputsDataMap object.



.. rubric:: Returns:

inputs Reference to ConstInputsDataMap object.

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1ab5d5797a7ef239eeb20d1c3eadf1bd73:
.. index:: pair: function; CreateInferRequest

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IInferRequestInternal<doxid-class_inference_engine_1_1_i_infer_request_internal>`> CreateInferRequest()

Create an inference request object used to infer the network Note: the returned request will have allocated input and output blobs (that can be changed later)



.. rubric:: Returns:

shared_ptr for the created request

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a057bca9b0f955c03190bdf77635e9516:
.. index:: pair: function; Export

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Export(const std::string& modelFileName)

Export the current created executable network so it can be used later in the Import() main API.

Deprecated Use :ref:`IExecutableNetworkInternal::Export(std::ostream& networkModel) <doxid-class_inference_engine_1_1_i_executable_network_internal_1a2b5e212158cd5bf3a2f903cd405fdd3d>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelFileName

		- - path to the location of the exported file

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a2b5e212158cd5bf3a2f903cd405fdd3d:
.. index:: pair: function; Export

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Export(std::ostream& networkModel)

Export the current created executable network so it can be used later in the Import() main API.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- - Reference to network model output stream

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1aeb29d9f35b340496272f785d7be4f097:
.. index:: pair: function; GetExecGraphInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> GetExecGraphInfo()

Get executable graph information from a device.



.. rubric:: Returns:

A network object to store executable graph information

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a13df5cff9daf69a68365509ad11a5b1f:
.. index:: pair: function; SetPointerToPlugin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetPointerToPlugin(const std::shared_ptr<:ref:`IInferencePlugin<doxid-class_inference_engine_1_1_i_inference_plugin>`>& plugin)

Sets the pointer to plugin internal.

Needed to correctly handle ownership between objects.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- plugin

		- The plugin

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a66bc34d51b798322d29ec1b1a8332faa:
.. index:: pair: function; SetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetConfig(const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& config)

Sets configuration for current executable network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- config

		- Map of pairs: (config parameter name, config parameter value)

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1aab6b3c29e3fec7400548b0af1808a772:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetConfig(const std::string& name) const

Gets configuration dedicated to plugin behaviour.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- A config key, can be found in ``ie_plugin_config.hpp``



.. rubric:: Returns:

A value of config corresponding to config key

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1abff44a61825a0da77a4a329225431708:
.. index:: pair: function; GetMetric

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetMetric(const std::string& name) const

Gets general runtime metric for dedicated hardware.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- A metric name to request



.. rubric:: Returns:

A metric value corresponding to metric key

.. _doxid-class_inference_engine_1_1_i_executable_network_internal_1a3a14f4c13bf0ba5470278d762cefc356:
.. index:: pair: function; GetContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> GetContext() const

Gets the remote context.



.. rubric:: Returns:

A reference to a context


