.. index:: pair: interface; InferenceEngine::IInferencePlugin
.. _doxid-class_inference_engine_1_1_i_inference_plugin:

interface InferenceEngine::IInferencePlugin
===========================================

.. toctree::
	:hidden:

	VersionStore <classInferenceEngine_1_1IInferencePlugin_1_1VersionStore.rst>

Overview
~~~~~~~~

An API of plugin to be implemented by a plugin. :ref:`More...<details-class_inference_engine_1_1_i_inference_plugin>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iplugin_internal.hpp>
	
	template IInferencePlugin: public std::enable_shared_from_this< IInferencePlugin >
	{
		// typedefs
	
		typedef std::shared_ptr<IInferencePlugin> :ref:`Ptr<doxid-class_inference_engine_1_1_i_inference_plugin_1ac4c2f5b84dede594c46e52d3733feed1>`;

		// classes
	
		class :ref:`VersionStore<doxid-class_inference_engine_1_1_i_inference_plugin_1_1_version_store>`;

		// methods
	
		void :ref:`SetVersion<doxid-class_inference_engine_1_1_i_inference_plugin_1aa45dced3c8be311665eecf9e1ac4e3b4>`(const :ref:`Version<doxid-struct_inference_engine_1_1_version>`& version);
		const :ref:`Version<doxid-struct_inference_engine_1_1_version>`& :ref:`GetVersion<doxid-class_inference_engine_1_1_i_inference_plugin_1ab6ae8ccddf250a9d08e20befe0dffc34>`() const;
		virtual std::string :ref:`GetName<doxid-class_inference_engine_1_1_i_inference_plugin_1aa728b42400204d7fefe15e7ddd9f3e97>`() const;
		virtual void :ref:`SetName<doxid-class_inference_engine_1_1_i_inference_plugin_1a9e841aa308b07722d2989150567ae37e>`(const std::string& name);
	
		virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`LoadNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1a07baadb21491baef977c424e59ec466b>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::map<std::string, std::string>& config
			);
	
		virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`LoadNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1a1a62fb7ecb7b74b9619afb33004bd11a>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::map<std::string, std::string>& config,
			const std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`>& context
			);
	
		virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`LoadNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1ac5ece4e1c3f4c0de4c6e5e2146b291f3>`(
			const std::string& modelPath,
			const std::map<std::string, std::string>& config
			);
	
		virtual void :ref:`AddExtension<doxid-class_inference_engine_1_1_i_inference_plugin_1aaceab5daa3394c13789ba2dd498e1d26>`(const std::shared_ptr<:ref:`IExtension<doxid-class_inference_engine_1_1_i_extension>`>& extension);
		virtual void :ref:`SetConfig<doxid-class_inference_engine_1_1_i_inference_plugin_1a7504c94d1d6358515594dc6417b68255>`(const std::map<std::string, std::string>& config);
	
		virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-class_inference_engine_1_1_i_inference_plugin_1a958312c1e583dbd12433b5d47900838a>`(
			const std::string& name,
			const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& options
			) const;
	
		virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetMetric<doxid-class_inference_engine_1_1_i_inference_plugin_1a3144a2e4de4a30b82c177c8a28a8df1b>`(
			const std::string& name,
			const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& options
			) const;
	
		virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`CreateContext<doxid-class_inference_engine_1_1_i_inference_plugin_1a2f6982bff8d32e54fb9b5107f86d3d88>`(const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params);
		virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> :ref:`GetDefaultContext<doxid-class_inference_engine_1_1_i_inference_plugin_1aedc63ccd089b7414a8a3d8fc410f6d52>`(const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params);
	
		virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`ImportNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1ab17c290b8d9d53d65425caa299b955c6>`(
			const std::string& modelFileName,
			const std::map<std::string, std::string>& config
			);
	
		virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`ImportNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1a749679b57c27073d5492518ff5d94d09>`(
			std::istream& networkModel,
			const std::map<std::string, std::string>& config
			);
	
		virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> :ref:`ImportNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1ab47e243b1f237ed27c6dc7902f35f64b>`(
			std::istream& networkModel,
			const std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`>& context,
			const std::map<std::string, std::string>& config
			);
	
		virtual void :ref:`SetCore<doxid-class_inference_engine_1_1_i_inference_plugin_1a516c6524062c9bc2db8f289655b5a682>`(std::weak_ptr<:ref:`ov::ICore<doxid-classov_1_1_i_core>`> core);
		virtual std::shared_ptr<:ref:`ov::ICore<doxid-classov_1_1_i_core>`> :ref:`GetCore<doxid-class_inference_engine_1_1_i_inference_plugin_1a58aa880df716e3e6ebe3306fd53adc4d>`() const;
		const std::shared_ptr<:ref:`ExecutorManager<doxid-class_inference_engine_1_1_executor_manager>`>& :ref:`executorManager<doxid-class_inference_engine_1_1_i_inference_plugin_1a096054512c9cded97842333ed25f402d>`() const;
	
		virtual :ref:`QueryNetworkResult<doxid-struct_inference_engine_1_1_query_network_result>` :ref:`QueryNetwork<doxid-class_inference_engine_1_1_i_inference_plugin_1a38f25668aeda910ae35f9497fffa01f4>`(
			const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
			const std::map<std::string, std::string>& config
			) const;

	protected:
	};
.. _details-class_inference_engine_1_1_i_inference_plugin:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An API of plugin to be implemented by a plugin.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1ac4c2f5b84dede594c46e52d3733feed1:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<IInferencePlugin> Ptr

A shared pointer to :ref:`IInferencePlugin <doxid-class_inference_engine_1_1_i_inference_plugin>` interface.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1aa45dced3c8be311665eecf9e1ac4e3b4:
.. index:: pair: function; SetVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetVersion(const :ref:`Version<doxid-struct_inference_engine_1_1_version>`& version)

Sets a plugin version.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- version

		- A version to set

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1ab6ae8ccddf250a9d08e20befe0dffc34:
.. index:: pair: function; GetVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Version<doxid-struct_inference_engine_1_1_version>`& GetVersion() const

Gets a plugin version.



.. rubric:: Returns:

A const :ref:`InferenceEngine::Version <doxid-struct_inference_engine_1_1_version>` object

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1aa728b42400204d7fefe15e7ddd9f3e97:
.. index:: pair: function; GetName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string GetName() const

Provides a name of a plugin.



.. rubric:: Returns:

The name.

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a9e841aa308b07722d2989150567ae37e:
.. index:: pair: function; SetName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetName(const std::string& name)

Sets a name for a plugin.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- The name

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a07baadb21491baef977c424e59ec466b:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> LoadNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::map<std::string, std::string>& config
		)

Creates an executable network from an pares network object, users can create as many networks as they need and use them simultaneously (up to the limitation of the HW resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- A network object acquired from :ref:`InferenceEngine::Core::ReadNetwork <doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef>`

	*
		- config

		- A string-string map of config parameters relevant only for this load operation



.. rubric:: Returns:

Created Executable Network object

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a1a62fb7ecb7b74b9619afb33004bd11a:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> LoadNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::map<std::string, std::string>& config,
		const std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`>& context
		)

Creates an executable network from network object, on specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- A network object acquired from :ref:`InferenceEngine::Core::ReadNetwork <doxid-class_inference_engine_1_1_core_1ac716dda382aefd09264b60ea40def3ef>`

	*
		- config

		- string-string map of config parameters relevant only for this load operation

	*
		- context

		- A pointer to plugin context derived from :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` class used to execute the network



.. rubric:: Returns:

Created Executable Network object

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1ac5ece4e1c3f4c0de4c6e5e2146b291f3:
.. index:: pair: function; LoadNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> LoadNetwork(
		const std::string& modelPath,
		const std::map<std::string, std::string>& config
		)

Creates an executable network from model file path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelPath

		- A path to model

	*
		- config

		- A string-string map of config parameters relevant only for this load operation



.. rubric:: Returns:

Created Executable Network object

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1aaceab5daa3394c13789ba2dd498e1d26:
.. index:: pair: function; AddExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void AddExtension(const std::shared_ptr<:ref:`IExtension<doxid-class_inference_engine_1_1_i_extension>`>& extension)

Registers extension within plugin.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- - pointer to already loaded extension

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a7504c94d1d6358515594dc6417b68255:
.. index:: pair: function; SetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetConfig(const std::map<std::string, std::string>& config)

Sets configuration for plugin, acceptable keys can be found in ``ie_plugin_config.hpp``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- config

		- string-string map of config parameters

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a958312c1e583dbd12433b5d47900838a:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetConfig(
		const std::string& name,
		const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& options
		) const

Gets configuration dedicated to plugin behaviour.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - value of config corresponding to config key

	*
		- options

		- - configuration details for config



.. rubric:: Returns:

Value of config corresponding to config key

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a3144a2e4de4a30b82c177c8a28a8df1b:
.. index:: pair: function; GetMetric

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetMetric(
		const std::string& name,
		const std::map<std::string, :ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>`>& options
		) const

Gets general runtime metric for dedicated hardware.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- - metric name to request

	*
		- options

		- - configuration details for metric



.. rubric:: Returns:

Metric value corresponding to metric key

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a2f6982bff8d32e54fb9b5107f86d3d88:
.. index:: pair: function; CreateContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> CreateContext(const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params)

Creates a remote context instance based on a map of parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- params

		- The map of parameters



.. rubric:: Returns:

A remote context object

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1aedc63ccd089b7414a8a3d8fc410f6d52:
.. index:: pair: function; GetDefaultContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`> GetDefaultContext(const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params)

Provides a default remote context instance if supported by a plugin.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- params

		- The map of parameters



.. rubric:: Returns:

The default context.

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1ab17c290b8d9d53d65425caa299b955c6:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> ImportNetwork(
		const std::string& modelFileName,
		const std::map<std::string, std::string>& config
		)

Creates an executable network from an previously exported network.

Deprecated Use :ref:`ImportNetwork(std::istream& networkModel, const std::map\<std::string, std::string>& config) <doxid-class_inference_engine_1_1_i_inference_plugin_1a749679b57c27073d5492518ff5d94d09>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- modelFileName

		- - path to the location of the exported file

	*
		- config

		- A string -> string map of parameters



.. rubric:: Returns:

An Executable network

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a749679b57c27073d5492518ff5d94d09:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> ImportNetwork(
		std::istream& networkModel,
		const std::map<std::string, std::string>& config
		)

Creates an executable network from an previously exported network using plugin implementation and removes Inference Engine magic and plugin name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- Reference to network model output stream

	*
		- config

		- A string -> string map of parameters



.. rubric:: Returns:

An Executable network

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1ab47e243b1f237ed27c6dc7902f35f64b:
.. index:: pair: function; ImportNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`IExecutableNetworkInternal<doxid-class_inference_engine_1_1_i_executable_network_internal>`> ImportNetwork(
		std::istream& networkModel,
		const std::shared_ptr<:ref:`RemoteContext<doxid-class_inference_engine_1_1_remote_context>`>& context,
		const std::map<std::string, std::string>& config
		)

Creates an executable network from an previously exported network using plugin implementation and removes Inference Engine magic and plugin name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- networkModel

		- Reference to network model output stream

	*
		- context

		- A pointer to plugin context derived from :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` class used to execute the network

	*
		- config

		- A string -> string map of parameters



.. rubric:: Returns:

An Executable network

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a516c6524062c9bc2db8f289655b5a682:
.. index:: pair: function; SetCore

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void SetCore(std::weak_ptr<:ref:`ov::ICore<doxid-classov_1_1_i_core>`> core)

Sets pointer to ICore interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- core

		- Pointer to :ref:`Core <doxid-class_inference_engine_1_1_core>` interface

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a58aa880df716e3e6ebe3306fd53adc4d:
.. index:: pair: function; GetCore

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`ov::ICore<doxid-classov_1_1_i_core>`> GetCore() const

Gets reference to ICore interface.



.. rubric:: Returns:

Reference to ICore interface

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a096054512c9cded97842333ed25f402d:
.. index:: pair: function; executorManager

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::shared_ptr<:ref:`ExecutorManager<doxid-class_inference_engine_1_1_executor_manager>`>& executorManager() const

Gets reference to tasks execution manager.



.. rubric:: Returns:

Reference to :ref:`ExecutorManager <doxid-class_inference_engine_1_1_executor_manager>` interface

.. _doxid-class_inference_engine_1_1_i_inference_plugin_1a38f25668aeda910ae35f9497fffa01f4:
.. index:: pair: function; QueryNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QueryNetworkResult<doxid-struct_inference_engine_1_1_query_network_result>` QueryNetwork(
		const :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& network,
		const std::map<std::string, std::string>& config
		) const

Queries a plugin about supported layers in network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- The network object to query

	*
		- config

		- The map of configuration parameters



.. rubric:: Returns:

The result of query operator containing supported layers map


