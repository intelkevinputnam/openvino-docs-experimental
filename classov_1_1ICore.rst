.. index:: pair: interface; ov::ICore
.. _doxid-classov_1_1_i_core:

interface ov::ICore
===================



Overview
~~~~~~~~

Minimal :ref:`ICore <doxid-classov_1_1_i_core>` interface to allow plugin to get information from :ref:`Core <doxid-classov_1_1_core>` Inference Engine class. :ref:`More...<details-classov_1_1_i_core>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_icore.hpp>
	
	template ICore
	{
		// methods
	
		virtual :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`ReadNetwork<doxid-classov_1_1_i_core_1a5f0faf1b6a977323cb0d46d35ecc8f46>`(
			const std::string& model,
			const :ref:`ie::Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`& weights,
			bool frontendMode = false
			) const = 0;
	
		virtual :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`ReadNetwork<doxid-classov_1_1_i_core_1ad53bbb6f37d8d4d9396e0e12530b1e3f>`(
			const std::string& modelPath,
			const std::string& binPath
			) const = 0;
	
		virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` :ref:`LoadNetwork<doxid-classov_1_1_i_core_1a0b013ba6ff1587ec9b7dff370077f5e6>`(
			const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config = {}
			) = 0;
	
		virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` :ref:`LoadNetwork<doxid-classov_1_1_i_core_1a6a647a1cd080df2f1a8756b3b6f51e41>`(
			const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const :ref:`ie::RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`& remoteCtx,
			const std::map<std::string, std::string>& config = {}
			) = 0;
	
		virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` :ref:`LoadNetwork<doxid-classov_1_1_i_core_1a07f3eb09465a18641302985b339ca14f>`(
			const std::string& modelPath,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config,
			const std::function<void(const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`&)>& val = nullptr
			) = 0;
	
		virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` :ref:`ImportNetwork<doxid-classov_1_1_i_core_1a6cb926f9aed1e2a7e9f35c2b0e77eaa8>`(
			std::istream& networkModel,
			const std::string& deviceName = {},
			const std::map<std::string, std::string>& config = {}
			) = 0;
	
		virtual :ref:`ie::QueryNetworkResult<doxid-struct_inference_engine_1_1_query_network_result>` :ref:`QueryNetwork<doxid-classov_1_1_i_core_1ab9c20906dedabdbd18c7a45e3487d6a8>`(
			const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::string& deviceName,
			const std::map<std::string, std::string>& config
			) const = 0;
	
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`GetMetric<doxid-classov_1_1_i_core_1aa95035fc229a7431dad1d5052ea45d1a>`(
			const std::string& deviceName,
			const std::string& name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& options = {}
			) const = 0;
	
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`GetConfig<doxid-classov_1_1_i_core_1ad81a6c06f7db4ba02e1ac578cc41d70d>`(const std::string& deviceName, const std::string& name) const = 0;
		virtual std::vector<std::string> :ref:`GetAvailableDevices<doxid-classov_1_1_i_core_1ac9c862c4fbc81f029a10ee4d7f0a7994>`() const = 0;
		virtual bool :ref:`DeviceSupportsImportExport<doxid-classov_1_1_i_core_1a16f5eff9ab6d614f827d4ff5fb82e0d1>`(const std::string& deviceName) const = 0;
	
		virtual :ref:`InferenceEngine::RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`CreateContext<doxid-classov_1_1_i_core_1a692ed66c1641a9c7568db934d8db123c>`(
			const std::string& deviceName,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`&
			) = 0;
	
		virtual std::map<std::string, std::string> :ref:`GetSupportedConfig<doxid-classov_1_1_i_core_1afad2f8b1e06b3e50226ce581ce969e63>`(
			const std::string& deviceName,
			const std::map<std::string, std::string>& config
			) = 0;
	
		virtual bool :target:`isNewAPI<doxid-classov_1_1_i_core_1a2334e44492a5fbd5ef2f075dc566425e>`() const = 0;
		virtual :ref:`ie::RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` :ref:`GetDefaultContext<doxid-classov_1_1_i_core_1ad37c6fd476b02576a7309f0786dd6f7d>`(const std::string& deviceName) = 0;
	
		virtual void :ref:`set_property<doxid-classov_1_1_i_core_1a5983f1846c1e69763501589883698f40>`(
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties
			) = 0;
	
		template <typename... Properties>
		util::EnableIfAllStringAny<void, Properties...> :ref:`set_property<doxid-classov_1_1_i_core_1aa7ddfc3561aa33b2c88cff174e75e6b6>`(
			const std::string& device_name,
			Properties&&... properties
			);
	
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`get_property<doxid-classov_1_1_i_core_1a13660120904cd1e2cc9e10c28cdf27a8>`(
			const std::string& device_name,
			const std::string& name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
			) const = 0;
	
		template <typename T, PropertyMutability M>
		T :ref:`get_property<doxid-classov_1_1_i_core_1a63eba165f36cdc80713aebda9eab15c1>`(
			const std::string& device_name,
			const :ref:`Property<doxid-classov_1_1_property>`<T, M>& property
			) const;
	
		template <typename T, PropertyMutability M>
		T :ref:`get_property<doxid-classov_1_1_i_core_1ac2bb45ef25a30e2a48a6309c61c81162>`(
			const std::string& device_name,
			const :ref:`Property<doxid-classov_1_1_property>`<T, M>& property,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
			) const;
	};
.. _details-classov_1_1_i_core:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimal :ref:`ICore <doxid-classov_1_1_i_core>` interface to allow plugin to get information from :ref:`Core <doxid-classov_1_1_core>` Inference Engine class.

Methods
-------

.. _doxid-classov_1_1_i_core_1a5f0faf1b6a977323cb0d46d35ecc8f46:
.. index:: pair: function; ReadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` ReadNetwork(
		const std::string& model,
		const :ref:`ie::Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`& weights,
		bool frontendMode = false
		) const = 0

Reads IR xml and bin (with the same name) files.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- string with IR

	*
		- weights

		- shared pointer to constant blob with weights

	*
		- frontendMode

		- read network without post-processing or other transformations



.. rubric:: Returns:

CNNNetwork

.. _doxid-classov_1_1_i_core_1ad53bbb6f37d8d4d9396e0e12530b1e3f:
.. index:: pair: function; ReadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` ReadNetwork(
		const std::string& modelPath,
		const std::string& binPath
		) const = 0

Reads IR xml and bin files.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelPath

		- path to IR file

	*
		- binPath

		- path to bin file, if path is empty, will try to read bin file with the same name as xml and if bin file with the same name was not found, will load IR without weights.



.. rubric:: Returns:

CNNNetwork

.. _doxid-classov_1_1_i_core_1a0b013ba6ff1587ec9b7dff370077f5e6:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` LoadNetwork(
		const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config = {}
		) = 0

Creates an executable network from a network object.

Users can create as many networks as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- CNNNetwork object acquired from Core::ReadNetwork

	*
		- deviceName

		- Name of device to load network to

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation



.. rubric:: Returns:

An executable network reference

.. _doxid-classov_1_1_i_core_1a6a647a1cd080df2f1a8756b3b6f51e41:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` LoadNetwork(
		const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const :ref:`ie::RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`& remoteCtx,
		const std::map<std::string, std::string>& config = {}
		) = 0

Creates an executable network from a network object.

Users can create as many networks as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- CNNNetwork object acquired from Core::ReadNetwork

	*
		- remoteCtx

		- "Remote" (non-CPU) accelerator device-specific execution context to use

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation



.. rubric:: Returns:

An executable network reference

.. _doxid-classov_1_1_i_core_1a07f3eb09465a18641302985b339ca14f:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` LoadNetwork(
		const std::string& modelPath,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config,
		const std::function<void(const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`&)>& val = nullptr
		) = 0

Creates an executable network from a model file.

Users can create as many networks as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelPath

		- Path to model

	*
		- deviceName

		- Name of device to load network to

	*
		- config

		- Optional map of pairs: (config parameter name, config parameter value) relevant only for this load operation

	*
		- val

		- Optional callback to perform validation of loaded CNNNetwork, if ReadNetwork is triggered



.. rubric:: Returns:

An executable network reference

.. _doxid-classov_1_1_i_core_1a6cb926f9aed1e2a7e9f35c2b0e77eaa8:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::SoExecutableNetworkInternal<doxid-namespace_inference_engine_1a2c034db0766cc19f90fcaa1670424efa>` ImportNetwork(
		std::istream& networkModel,
		const std::string& deviceName = {},
		const std::map<std::string, std::string>& config = {}
		) = 0

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

.. _doxid-classov_1_1_i_core_1ab9c20906dedabdbd18c7a45e3487d6a8:
.. index:: pair: function; QueryNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::QueryNetworkResult<doxid-struct_inference_engine_1_1_query_network_result>` QueryNetwork(
		const :ref:`ie::CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::string& deviceName,
		const std::map<std::string, std::string>& config
		) const = 0

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

.. _doxid-classov_1_1_i_core_1aa95035fc229a7431dad1d5052ea45d1a:
.. index:: pair: function; GetMetric

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Any<doxid-classov_1_1_any>` GetMetric(
		const std::string& deviceName,
		const std::string& name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& options = {}
		) const = 0

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



.. rubric:: Returns:

Metric value corresponding to metric key.

.. _doxid-classov_1_1_i_core_1ad81a6c06f7db4ba02e1ac578cc41d70d:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Any<doxid-classov_1_1_any>` GetConfig(const std::string& deviceName, const std::string& name) const = 0

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

.. _doxid-classov_1_1_i_core_1ac9c862c4fbc81f029a10ee4d7f0a7994:
.. index:: pair: function; GetAvailableDevices

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::string> GetAvailableDevices() const = 0

Returns devices available for neural networks inference.



.. rubric:: Returns:

A vector of devices. The devices are returned as { CPU, GPU.0, GPU.1, MYRIAD } If there more than one device of specific type, they are enumerated with .# suffix.

.. _doxid-classov_1_1_i_core_1a16f5eff9ab6d614f827d4ff5fb82e0d1:
.. index:: pair: function; DeviceSupportsImportExport

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool DeviceSupportsImportExport(const std::string& deviceName) const = 0

Checks whether device supports Export & Import functionality of network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- - A name of a device to get a metric value.



.. rubric:: Returns:

True if device has IMPORT_EXPORT_SUPPORT metric in SUPPORTED_METRICS and this metric returns 'true', False otherwise.

.. _doxid-classov_1_1_i_core_1a692ed66c1641a9c7568db934d8db123c:
.. index:: pair: function; CreateContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`InferenceEngine::RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` CreateContext(
		const std::string& deviceName,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`&
		) = 0

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

.. _doxid-classov_1_1_i_core_1afad2f8b1e06b3e50226ce581ce969e63:
.. index:: pair: function; GetSupportedConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, std::string> GetSupportedConfig(
		const std::string& deviceName,
		const std::map<std::string, std::string>& config
		) = 0

Get only configs that are suppored by device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- Name of a device

	*
		- config

		- Map of configs that can contains configs that are not supported by device



.. rubric:: Returns:

map of configs that are supported by device

.. _doxid-classov_1_1_i_core_1ad37c6fd476b02576a7309f0786dd6f7d:
.. index:: pair: function; GetDefaultContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ie::RemoteContext::Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>` GetDefaultContext(const std::string& deviceName) = 0

Get a pointer to default shared context object for the specified device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- deviceName

		- - A name of a device to get create shared context from.



.. rubric:: Returns:

A shared pointer to a default remote context.

.. _doxid-classov_1_1_i_core_1a5983f1846c1e69763501589883698f40:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_property(
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties
		) = 0

Sets properties for a device, acceptable keys can be found in ``openvino/runtime/properties.hpp``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Name of a device.

	*
		- properties

		- Map of pairs: (property name, property value).

.. _doxid-classov_1_1_i_core_1aa7ddfc3561aa33b2c88cff174e75e6b6:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<void, Properties...> set_property(
		const std::string& device_name,
		Properties&&... properties
		)

Sets properties for a device, acceptable keys can be found in ``openvino/runtime/properties.hpp``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`Any <doxid-classov_1_1_any>`>`` types.

	*
		- device_name

		- Name of a device.

	*
		- properties

		- Optional pack of pairs: (property name, property value).

.. _doxid-classov_1_1_i_core_1a13660120904cd1e2cc9e10c28cdf27a8:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Any<doxid-classov_1_1_any>` get_property(
		const std::string& device_name,
		const std::string& name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
		) const = 0

Gets properties related to device behaviour.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Name of a device to get a property value.

	*
		- name

		- :ref:`Property <doxid-classov_1_1_property>` name.

	*
		- arguments

		- Additional arguments to get a property.



.. rubric:: Returns:

Value of a property corresponding to the property name.

.. _doxid-classov_1_1_i_core_1a63eba165f36cdc80713aebda9eab15c1:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, PropertyMutability M>
	T get_property(
		const std::string& device_name,
		const :ref:`Property<doxid-classov_1_1_property>`<T, M>& property
		) const

Gets properties related to device behaviour.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type of a returned value.

	*
		- M

		- :ref:`Property <doxid-classov_1_1_property>` mutability.

	*
		- deviceName

		- Name of a device to get a property value.

	*
		- property

		- :ref:`Property <doxid-classov_1_1_property>` object.



.. rubric:: Returns:

:ref:`Property <doxid-classov_1_1_property>` value.

.. _doxid-classov_1_1_i_core_1ac2bb45ef25a30e2a48a6309c61c81162:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, PropertyMutability M>
	T get_property(
		const std::string& device_name,
		const :ref:`Property<doxid-classov_1_1_property>`<T, M>& property,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
		) const

Gets properties related to device behaviour.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type of a returned value.

	*
		- M

		- :ref:`Property <doxid-classov_1_1_property>` mutability.

	*
		- deviceName

		- Name of a device to get a property value.

	*
		- property

		- :ref:`Property <doxid-classov_1_1_property>` object.

	*
		- arguments

		- Additional arguments to get a property.



.. rubric:: Returns:

:ref:`Property <doxid-classov_1_1_property>` value.


