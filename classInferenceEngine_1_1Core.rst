.. index:: pair: class; InferenceEngine::Core
.. _doxid-class_inference_engine_1_1_core:

class InferenceEngine::Core
===========================



Overview
~~~~~~~~

This class represents Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` entity. :ref:`More...<details-class_inference_engine_1_1_core>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_core.hpp>
	
	class Core
	{
	public:
		// construction
	
		:ref:`Core<doxid-class_inference_engine_1_1_core_1ab582cc865fc264fd798399ad34c4c490>`(const std::string& xmlConfigFile = {});

		// methods
	
		std::map<std::string, :ref:`Version<doxid-struct_inference_engine_1_1_version>`> :ref:`GetVersions<doxid-class_inference_engine_1_1_core_1a7c31b13da8f599e9aec93121da287d1c>`(const std::string& deviceName) const;
	
		:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`ReadNetwork<doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef>`(
			const std::string& modelPath,
			const std::string& binPath = {}
			) const;
	
		:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`ReadNetwork<doxid-class_inference_engine_1_1_core_1a251861e52a979d6e61848babae3673ef>`(const std::string& model, const :ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`& weights) const;
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`LoadNetwork<doxid-class_inference_engine_1_1_core_1a7b0b5ab0009abc572762422105b5c666>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::map<std::string, std::string>& config = {}
			);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`LoadNetwork<doxid-class_inference_engine_1_1_core_1a7ac4bd8bc351fae833aaa0db84fab738>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config = {}
			);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`LoadNetwork<doxid-class_inference_engine_1_1_core_1a6753da75547ffee37862c30c8f30f9e7>`(
			const std::string& modelPath,
			const std::map<std::string, std::string>& config = {}
			);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`LoadNetwork<doxid-class_inference_engine_1_1_core_1a58dfdb97a5a965688e0aa59dd2ffb476>`(
			const std::string& modelPath,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config = {}
			);
	
		void :ref:`AddExtension<doxid-class_inference_engine_1_1_core_1aac8284a60791abd6e50ddab0c695e38f>`(const :ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>`& extension);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`LoadNetwork<doxid-class_inference_engine_1_1_core_1aade061d5cccfab48d149ec989eb7e3f4>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` context,
			const std::map<std::string, std::string>& config = {}
			);
	
		void :ref:`AddExtension<doxid-class_inference_engine_1_1_core_1aa1ddb53f4160bf0735239f4aa0c12320>`(:ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>` extension, const std::string& deviceName);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`ImportNetwork<doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013>`(
			const std::string& modelFileName,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config = {}
			);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`ImportNetwork<doxid-class_inference_engine_1_1_core_1a0c4dc9377db2e03d016102d5beee0d7c>`(
			std::istream& networkModel,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config = {}
			);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`ImportNetwork<doxid-class_inference_engine_1_1_core_1a91273c76ba8495be1b73b03deeb9093f>`(std::istream& networkModel);
	
		:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` :ref:`ImportNetwork<doxid-class_inference_engine_1_1_core_1a81f8ced8acf4c0302fc242cc2618175d>`(
			std::istream& networkModel,
			const :ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`& context,
			const std::map<std::string, std::string>& config = {}
			);
	
		:ref:`QueryNetworkResult<doxid-struct_inference_engine_1_1_query_network_result>` :ref:`QueryNetwork<doxid-class_inference_engine_1_1_core_1a0852259214fd9faf2b46bb9720ec825a>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config = {}
			) const;
	
		void :ref:`SetConfig<doxid-class_inference_engine_1_1_core_1a34aa9ac6fb237b634d5bf08b288e88d4>`(
			const std::map<std::string, std::string>& config,
			const std::string& deviceName = {}
			);
	
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-class_inference_engine_1_1_core_1a415077386694f95b57e4cccb0d334a55>`(const std::string& deviceName, const std::string& name) const;
	
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetMetric<doxid-class_inference_engine_1_1_core_1a27b1476aa8095c237eeabacfce73b38e>`(
			const std::string& deviceName,
			const std::string& name,
			const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& options = {}
			) const;
	
		std::vector<std::string> :ref:`GetAvailableDevices<doxid-class_inference_engine_1_1_core_1acb212aa879e1234f51b845d2befae41c>`() const;
	
		void :ref:`RegisterPlugin<doxid-class_inference_engine_1_1_core_1a56acaf7ba719bae5d7d2992e6c5fe0f5>`(
			const std::string& pluginName,
			const std::string& deviceName
			);
	
		void :ref:`UnregisterPlugin<doxid-class_inference_engine_1_1_core_1a5bf42b2543fc4fb79af7c5da8b06209d>`(const std::string& deviceName);
		void :ref:`RegisterPlugins<doxid-class_inference_engine_1_1_core_1a6d5eb76c849a82d870a0a6f848641edd>`(const std::string& xmlConfigFile);
	
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`CreateContext<doxid-class_inference_engine_1_1_core_1afeaad400e079f7b24fe9106702215c7f>`(
			const std::string& deviceName,
			const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params
			);
	
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`GetDefaultContext<doxid-class_inference_engine_1_1_core_1a3f7e984891b16d3825d0184698562802>`(const std::string& deviceName);
	};
.. _details-class_inference_engine_1_1_core:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` entity.

It can throw exceptions safely for the application, where it is properly handled.

Construction
------------

.. _doxid-class_inference_engine_1_1_core_1ab582cc865fc264fd798399ad34c4c490:
.. index:: pair: function; Core

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Core(const std::string& xmlConfigFile = {})

Constructs an OpenVINO :ref:`Core <doxid-class_inference_engine_1_1_core>` instance with devices and their plugins description.

There are two ways how to configure device plugins:

#. (default) Use XML configuration file in case of dynamic libraries build;

#. Use strictly defined configuration in case of static libraries build.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xml_config_file

		- 
		  Path to the .xml file with plugins to load from. If the XML configuration file is not specified, default OpenVINO Runtime plugins are loaded from:
		  
		  #. (dynamic build) default ``plugins.xml`` file located in the same folder as OpenVINO runtime shared library;
		  
		  #. (static build) statically defined configuration. In this case path to the .xml file is ignored.

Methods
-------

.. _doxid-class_inference_engine_1_1_core_1a7c31b13da8f599e9aec93121da287d1c:
.. index:: pair: function; GetVersions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, :ref:`Version<doxid-struct_inference_engine_1_1_version>`> GetVersions(const std::string& deviceName) const

Returns plugins version information.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- Device name to identify plugin



.. rubric:: Returns:

A vector of versions

.. _doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef:
.. index:: pair: function; ReadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` ReadNetwork(
		const std::string& modelPath,
		const std::string& binPath = {}
		) const

Reads models from IR and ONNX formats.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelPath

		- path to model

	*
		- binPath

		- 
		  path to data file For IR format (\*.bin):
		  
		  * if path is empty, will try to read bin file with the same name as xml and
		  
		  * if bin file with the same name was not found, will load IR without weights. For ONNX format (\*.onnx):
		  
		  * binPath parameter is not used.



.. rubric:: Returns:

:ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>`

.. _doxid-class_inference_engine_1_1_core_1a251861e52a979d6e61848babae3673ef:
.. index:: pair: function; ReadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` ReadNetwork(const std::string& model, const :ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`& weights) const

Reads models from IR and ONNX formats.

Created :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` object shares the weights with ``weights`` object. So, do not create ``weights`` on temporary data which can be later freed, since the network constant data becomes to point to invalid memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- string with model in IR or ONNX format

	*
		- weights

		- shared pointer to constant blob with weights Reading ONNX models doesn't support loading weights from data blobs. If you are using an ONNX model with external data files, please use the ``:ref:`InferenceEngine::Core::ReadNetwork(const std::string& model, const Blob::CPtr& weights) const <doxid-class_inference_engine_1_1_core_1a251861e52a979d6e61848babae3673ef>``` function overload which takes a filesystem path to the model. For ONNX case the second parameter should contain empty blob.



.. rubric:: Returns:

:ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>`

.. _doxid-class_inference_engine_1_1_core_1a7b0b5ab0009abc572762422105b5c666:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` LoadNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::map<std::string, std::string>& config = {}
		)

Creates an executable network from a network object and uses AUTO plugin as the default device to load executable network.

Users can create as many networks as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- :ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` object acquired from :ref:`Core::ReadNetwork <doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef>`

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a7ac4bd8bc351fae833aaa0db84fab738:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` LoadNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config = {}
		)

Creates an executable network from a network object.

Users can create as many networks as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- :ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` object acquired from :ref:`Core::ReadNetwork <doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef>`

	*
		- deviceName

		- Name of device to load network to

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a6753da75547ffee37862c30c8f30f9e7:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` LoadNetwork(
		const std::string& modelPath,
		const std::map<std::string, std::string>& config = {}
		)

Reads model and creates an executable network from IR or ONNX file and uses AUTO plugin as the default device to load executable network.

This can be more efficient than using ReadNetwork + LoadNetwork(CNNNetwork) flow especially for cases when caching is enabled and cached model is available



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelPath

		- path to model

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation/



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a58dfdb97a5a965688e0aa59dd2ffb476:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` LoadNetwork(
		const std::string& modelPath,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config = {}
		)

Reads model and creates an executable network from IR or ONNX file.

This can be more efficient than using ReadNetwork + LoadNetwork(CNNNetwork) flow especially for cases when caching is enabled and cached model is available



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelPath

		- path to model

	*
		- deviceName

		- Name of device to load network to

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation/



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1aac8284a60791abd6e50ddab0c695e38f:
.. index:: pair: function; AddExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void AddExtension(const :ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>`& extension)

Registers extension.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- Pointer to already loaded extension

.. _doxid-class_inference_engine_1_1_core_1aade061d5cccfab48d149ec989eb7e3f4:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` LoadNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` context,
		const std::map<std::string, std::string>& config = {}
		)

Creates an executable network from a network object within a specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- :ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` object acquired from :ref:`Core::ReadNetwork <doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef>`

	*
		- context

		- Pointer to :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation



.. rubric:: Returns:

An executable network object

.. _doxid-class_inference_engine_1_1_core_1aa1ddb53f4160bf0735239f4aa0c12320:
.. index:: pair: function; AddExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void AddExtension(:ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>` extension, const std::string& deviceName)

Registers extension for the specified plugin.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- Pointer to already loaded extension

	*
		- deviceName

		- Device name to identify plugin to add an executable extension

.. _doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` ImportNetwork(
		const std::string& modelFileName,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config = {}
		)

Creates an executable network from a previously exported network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelFileName

		- Path to the location of the exported file

	*
		- deviceName

		- Name of device load executable network on

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation\*



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a0c4dc9377db2e03d016102d5beee0d7c:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` ImportNetwork(
		std::istream& networkModel,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config = {}
		)

Creates an executable network from a previously exported network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- network model stream

	*
		- deviceName

		- Name of device load executable network on

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation\*



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a91273c76ba8495be1b73b03deeb9093f:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` ImportNetwork(std::istream& networkModel)

Creates an executable network from a previously exported network.

Deprecated Use :ref:`Core::ImportNetwork <doxid-class_inference_engine_1_1_core_1af5dd52e92164a99ce9ed90f78b14d013>` with explicit device name



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- network model stream



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a81f8ced8acf4c0302fc242cc2618175d:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ExecutableNetwork<doxid-class_inference_engine_1_1_executable_network>` ImportNetwork(
		std::istream& networkModel,
		const :ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`& context,
		const std::map<std::string, std::string>& config = {}
		)

Creates an executable network from a previously exported network within a specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- Network model stream

	*
		- context

		- Pointer to :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation



.. rubric:: Returns:

An executable network reference

.. _doxid-class_inference_engine_1_1_core_1a0852259214fd9faf2b46bb9720ec825a:
.. index:: pair: function; QueryNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QueryNetworkResult<doxid-struct_inference_engine_1_1_query_network_result>` QueryNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config = {}
		) const

Query device if it supports specified network with specified configuration.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- A name of a device to query

	*
		- network

		- Network object to query

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value)



.. rubric:: Returns:

An object containing a map of pairs a layer name -> a device name supporting this layer.

.. _doxid-class_inference_engine_1_1_core_1a34aa9ac6fb237b634d5bf08b288e88d4:
.. index:: pair: function; SetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetConfig(
		const std::map<std::string, std::string>& config,
		const std::string& deviceName = {}
		)

Sets configuration for device, acceptable keys can be found in ``ie_plugin_config.hpp``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- An optional name of a device. If device name is not specified, the config is set for all the registered devices.

	*
		- config

		- Map of pairs: (config parameter name, config parameter value)

.. _doxid-class_inference_engine_1_1_core_1a415077386694f95b57e4cccb0d334a55:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetConfig(const std::string& deviceName, const std::string& name) const

Gets configuration dedicated to device behaviour.

The method is targeted to extract information which can be set via SetConfig method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- - A name of a device to get a configuration value.

	*
		- name

		- - config key.



.. rubric:: Returns:

Value of config corresponding to config key.

.. _doxid-class_inference_engine_1_1_core_1a27b1476aa8095c237eeabacfce73b38e:
.. index:: pair: function; GetMetric

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetMetric(
		const std::string& deviceName,
		const std::string& name,
		const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& options = {}
		) const

Gets general runtime metric for dedicated hardware.

The method is needed to request common device properties which are executable network agnostic. It can be device name, temperature, other devices-specific values.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- - A name of a device to get a metric value.

	*
		- name

		- - metric name to request.

	*
		- options

		- - optional parameters to get a metric value



.. rubric:: Returns:

Metric value corresponding to metric key.

.. _doxid-class_inference_engine_1_1_core_1acb212aa879e1234f51b845d2befae41c:
.. index:: pair: function; GetAvailableDevices

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> GetAvailableDevices() const

Returns devices available for neural networks inference.



.. rubric:: Returns:

A vector of devices. The devices are returned as { CPU, GPU.0, GPU.1, MYRIAD } If there more than one device of specific type, they are enumerated with .# suffix.

.. _doxid-class_inference_engine_1_1_core_1a56acaf7ba719bae5d7d2992e6c5fe0f5:
.. index:: pair: function; RegisterPlugin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void RegisterPlugin(
		const std::string& pluginName,
		const std::string& deviceName
		)

Register new device and plugin which implement this device inside Inference Engine.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pluginName

		- A name of plugin. Depending on platform pluginName is wrapped with shared library suffix and prefix to identify library full name

	*
		- deviceName

		- A device name to register plugin for. If device name is not specified, then it's taken from plugin itself.

.. _doxid-class_inference_engine_1_1_core_1a5bf42b2543fc4fb79af7c5da8b06209d:
.. index:: pair: function; UnregisterPlugin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void UnregisterPlugin(const std::string& deviceName)

Unloads previously loaded plugin with a specified name from Inference Engine The method is needed to remove plugin instance and free its resources. If plugin for a specified device has not been created before, the method throws an exception.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- Device name identifying plugin to remove from Inference Engine

.. _doxid-class_inference_engine_1_1_core_1a6d5eb76c849a82d870a0a6f848641edd:
.. index:: pair: function; RegisterPlugins

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void RegisterPlugins(const std::string& xmlConfigFile)

Registers plugin to Inference Engine :ref:`Core <doxid-class_inference_engine_1_1_core>` instance using XML configuration file with plugins description.

XML file has the following structure:

.. ref-code-block:: cpp

	<ie>
	    <plugins>
	        <plugin name="" location="">
	            <extensions>
	                <extension location=""/>
	            </extensions>
	            <properties>
	                <property key="" value=""/>
	            </properties>
	        </plugin>
	    </plugins>
	</ie>

* ``name`` identifies name of device enabled by plugin

* ``location`` specifies absolute path to dynamic library with plugin. A path can also be relative to inference engine shared library. It allows to have common config for different systems with different configurations.

* Properties are set to plugin via the ``SetConfig`` method.

* Extensions are set to plugin via the ``AddExtension`` method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlConfigFile

		- A path to .xml file with plugins to register.

.. _doxid-class_inference_engine_1_1_core_1afeaad400e079f7b24fe9106702215c7f:
.. index:: pair: function; CreateContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` CreateContext(
		const std::string& deviceName,
		const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params
		)

Create a new shared context object on specified accelerator device using specified plugin-specific low level device API parameters (device handle, pointer, etc.)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- Name of a device to create new shared context on.

	*
		- params

		- Map of device-specific shared context parameters.



.. rubric:: Returns:

A shared pointer to a created remote context.

.. _doxid-class_inference_engine_1_1_core_1a3f7e984891b16d3825d0184698562802:
.. index:: pair: function; GetDefaultContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` GetDefaultContext(const std::string& deviceName)

Get a pointer to default(plugin-supplied) shared context object for specified accelerator device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- - A name of a device to get create shared context from.



.. rubric:: Returns:

A shared pointer to a default remote context.


