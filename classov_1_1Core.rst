.. index:: pair: class; ov::Core
.. _doxid-classov_1_1_core:

class ov::Core
==============



Overview
~~~~~~~~

This class represents an OpenVINO runtime :ref:`Core <doxid-classov_1_1_core>` entity.

User applications can create several :ref:`Core <doxid-classov_1_1_core>` class instances, but in this case the underlying plugins are created multiple times and not shared between several :ref:`Core <doxid-classov_1_1_core>` instances. The recommended way is to have a single :ref:`Core <doxid-classov_1_1_core>` instance per application. :ref:`More...<details-classov_1_1_core>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <core.hpp>
	
	class Core
	{
	public:
		// construction
	
		:ref:`Core<doxid-classov_1_1_core_1a0d036ec76a3c9fb851d25983a5cf8b65>`(const std::string& xml_config_file = {});

		// methods
	
		std::map<std::string, :ref:`Version<doxid-structov_1_1_version>`> :ref:`get_versions<doxid-classov_1_1_core_1a29caa73859531e56017a8b85a7ea7c22>`(const std::string& device_name) const;
	
		std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> :ref:`read_model<doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`(
			const std::string& model_path,
			const std::string& bin_path = {}
			) const;
	
		std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> :ref:`read_model<doxid-classov_1_1_core_1ae03920734b7f7c2011a69212a4fed802>`(
			const std::string& model,
			const :ref:`Tensor<doxid-classov_1_1_tensor>`& weights
			) const;
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`compile_model<doxid-classov_1_1_core_1a46555f0803e8c29524626be08e7f5c5a>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`compile_model<doxid-classov_1_1_core_1a00c10d82856a356ae61a05eae9aecf7f>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			Properties&&... properties
			);
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`compile_model<doxid-classov_1_1_core_1aa76b45a674acf63b901c805ee8f2ce94>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`compile_model<doxid-classov_1_1_core_1a4c34bf8e08e71dfc99f7cc05ffd8c53f>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const std::string& device_name,
			Properties&&... properties
			);
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`compile_model<doxid-classov_1_1_core_1a65ca9ef050647290741641d2e6e7caf3>`(
			const std::string& model_path,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`compile_model<doxid-classov_1_1_core_1a1234fffb379c06e0956f91e83991fec3>`(
			const std::string& model_path,
			Properties&&... properties
			);
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`compile_model<doxid-classov_1_1_core_1af619069271ccc7b10f8873427ba31404>`(
			const std::string& model_path,
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`compile_model<doxid-classov_1_1_core_1aa53b76d5b7a0905ee2585fe313a60666>`(
			const std::string& model_path,
			const std::string& device_name,
			Properties&&... properties
			);
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`compile_model<doxid-classov_1_1_core_1abfc3448baa2338c93d856235cda319d1>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`compile_model<doxid-classov_1_1_core_1a3524c699eb9bb670816728b7898e4f77>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
			Properties&&... properties
			);
	
		void :ref:`add_extension<doxid-classov_1_1_core_1a68d0dea1cbcd42a67bea32780e32acea>`(const std::shared_ptr<:ref:`InferenceEngine::IExtension<doxid-class_inference_engine_1_1_i_extension>`>& extension);
		void :ref:`add_extension<doxid-classov_1_1_core_1adb5929d85ce33c029794f0dbbb23340f>`(const std::string& library_path);
		void :ref:`add_extension<doxid-classov_1_1_core_1a31767e933913bd6a8379174a6d345a2e>`(const std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>& extension);
		void :ref:`add_extension<doxid-classov_1_1_core_1a77eb6bc41ba7e0174765c7ecd51764dd>`(const std::vector<std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>>& extensions);
	
		template <
			class T,
			typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
			>
		void :ref:`add_extension<doxid-classov_1_1_core_1a085742dfdd3180fecb6eae4dc4876059>`(const T& extension);
	
		template <
			class T,
			class... Targs,
			typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
			>
		void :ref:`add_extension<doxid-classov_1_1_core_1afd1c7fb8fced33c76d4b9cb53c9c21af>`(
			const T& extension,
			Targs... args
			);
	
		template <
			class T,
			typename std::enable_if<std::is_base_of<ov::op::Op, T>::value, bool>::type = true
			>
		void :ref:`add_extension<doxid-classov_1_1_core_1abdaf09c199b3479b0a75b7bd86a7a7a5>`();
	
		template <
			class T,
			class... Targs,
			typename std::enable_if<std::is_base_of<ov::op::Op, T>::value&&sizeof...(Targs), bool>::type = true
			>
		void :ref:`add_extension<doxid-classov_1_1_core_1ab285ce1bd2a4f739b8b6bae782eb1dfd>`();
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`import_model<doxid-classov_1_1_core_1a0d2853511bd7ba60cb591f4685b91884>`(
			std::istream& model_stream,
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`import_model<doxid-classov_1_1_core_1a5acc88fb26e9b2bc2fa796b3ea82f9c7>`(
			std::istream& model_stream,
			const std::string& device_name,
			Properties&&... properties
			);
	
		:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` :ref:`import_model<doxid-classov_1_1_core_1a319a7979bd731f3ad7e8aa4cf209727e>`(
			std::istream& model_stream,
			const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> :ref:`import_model<doxid-classov_1_1_core_1adde2adadfa0a523a078667b4f52046c6>`(
			std::istream& model_stream,
			const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
			Properties&&... properties
			);
	
		:ref:`SupportedOpsMap<doxid-group__ov__runtime__cpp__api_1gae52f095f7ed180ae11f2a8bca5dfc16b>` :ref:`query_model<doxid-classov_1_1_core_1acdf8e64824fe4cf147c3b52ab32c1aab>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
			) const;
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`SupportedOpsMap<doxid-group__ov__runtime__cpp__api_1gae52f095f7ed180ae11f2a8bca5dfc16b>`, Properties...> :ref:`query_model<doxid-classov_1_1_core_1a5bee7e3a9b5ee0866add542ee17807a7>`(
			const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
			const std::string& device_name,
			Properties&&... properties
			) const;
	
		void :ref:`set_property<doxid-classov_1_1_core_1aa953cb0a1601dbc9a34ef6ba82b8476e>`(const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<void, Properties...> :ref:`set_property<doxid-classov_1_1_core_1a3e7164e5c6865ffb458c0bcc976df6a2>`(Properties&&... properties);
	
		void :ref:`set_property<doxid-classov_1_1_core_1a14cba2136b972ee34478dd11633293a2>`(const std::string& device_name, const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<void, Properties...> :ref:`set_property<doxid-classov_1_1_core_1abd2ef5e757bb7b5ef5a075740992e731>`(
			const std::string& device_name,
			Properties&&... properties
			);
	
		:ref:`Any<doxid-classov_1_1_any>` :ref:`get_property<doxid-classov_1_1_core_1a4fb9fc7375d04f744a27a9588cbcff1a>`(const std::string& device_name, const std::string& name) const;
	
		:ref:`Any<doxid-classov_1_1_any>` :ref:`get_property<doxid-classov_1_1_core_1a448a6115a7a9eea4e0c028f9fffd37e9>`(
			const std::string& device_name,
			const std::string& name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
			) const;
	
		template <typename T, PropertyMutability M>
		T :ref:`get_property<doxid-classov_1_1_core_1a7e8abe0a1d9b4b9046b6eefb47be1abb>`(
			const std::string& deviceName,
			const :ref:`ov::Property<doxid-classov_1_1_property>`<T, M>& property
			) const;
	
		template <typename T, PropertyMutability M>
		T :ref:`get_property<doxid-classov_1_1_core_1a3267437192896805958f2d6ccfd66429>`(
			const std::string& deviceName,
			const :ref:`ov::Property<doxid-classov_1_1_property>`<T, M>& property,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
			) const;
	
		template <typename T, PropertyMutability M, typename... Args>
		util::EnableIfAllStringAny<T, Args...> :ref:`get_property<doxid-classov_1_1_core_1a018a070d2c512b247b75cf6de945e679>`(
			const std::string& deviceName,
			const :ref:`ov::Property<doxid-classov_1_1_property>`<T, M>& property,
			Args&&... args
			) const;
	
		std::vector<std::string> :ref:`get_available_devices<doxid-classov_1_1_core_1ac4efa134a1f874cffa38c7f48f222e3a>`() const;
	
		void :ref:`register_plugin<doxid-classov_1_1_core_1a079dcf7620d97d26d1fb2b763ca38025>`(
			const std::string& plugin_name,
			const std::string& device_name
			);
	
		void :ref:`unload_plugin<doxid-classov_1_1_core_1a8ec07372698dbbe9640d15ad5da48ff2>`(const std::string& device_name);
		void :ref:`register_plugins<doxid-classov_1_1_core_1a6876f03b2e99b7ff2a78d8416dfe29ea>`(const std::string& xml_config_file);
	
		:ref:`RemoteContext<doxid-classov_1_1_remote_context>` :ref:`create_context<doxid-classov_1_1_core_1ab9a3eef07c3471037070242f8da2fb01>`(
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& remote_properties
			);
	
		template <typename... Properties>
		util::EnableIfAllStringAny<:ref:`RemoteContext<doxid-classov_1_1_remote_context>`, Properties...> :ref:`create_context<doxid-classov_1_1_core_1a6d80f484c89161cc3b179979134cf8ab>`(
			const std::string& device_name,
			Properties&&... remote_properties
			);
	
		:ref:`RemoteContext<doxid-classov_1_1_remote_context>` :ref:`get_default_context<doxid-classov_1_1_core_1a0ae465fb50e92fa63054c2d0acfd25ae>`(const std::string& device_name);
	};
.. _details-classov_1_1_core:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an OpenVINO runtime :ref:`Core <doxid-classov_1_1_core>` entity.

User applications can create several :ref:`Core <doxid-classov_1_1_core>` class instances, but in this case the underlying plugins are created multiple times and not shared between several :ref:`Core <doxid-classov_1_1_core>` instances. The recommended way is to have a single :ref:`Core <doxid-classov_1_1_core>` instance per application.

Construction
------------

.. _doxid-classov_1_1_core_1a0d036ec76a3c9fb851d25983a5cf8b65:
.. index:: pair: function; Core

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Core(const std::string& xml_config_file = {})

Constructs an OpenVINO :ref:`Core <doxid-classov_1_1_core>` instance with devices and their plugins description.

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

.. _doxid-classov_1_1_core_1a29caa73859531e56017a8b85a7ea7c22:
.. index:: pair: function; get_versions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, :ref:`Version<doxid-structov_1_1_version>`> get_versions(const std::string& device_name) const

Returns device plugins version information. Device name can be complex and identify multiple devices at once like ``HETERO:CPU,GPU``; in this case, std::map contains multiple entries, each per device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Device name to identify a plugin.



.. rubric:: Returns:

A vector of versions.

.. _doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1:
.. index:: pair: function; read_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> read_model(
		const std::string& model_path,
		const std::string& bin_path = {}
		) const

Reads models from IR/ONNX/PDPD formats.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model_path

		- Path to a model.

	*
		- bin_path

		- 
		  Path to a data file. For IR format (\*.bin):
		  
		  * if path is empty, will try to read a bin file with the same name as xml and
		  
		  * if the bin file with the same name is not found, will load IR without weights. For ONNX format (\*.onnx):
		  
		  * the bin_path parameter is not used. For PDPD format (\*.pdmodel)
		  
		  * the bin_path parameter is not used.



.. rubric:: Returns:

A model.

.. _doxid-classov_1_1_core_1ae03920734b7f7c2011a69212a4fed802:
.. index:: pair: function; read_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> read_model(
		const std::string& model,
		const :ref:`Tensor<doxid-classov_1_1_tensor>`& weights
		) const

Reads models from IR/ONNX/PDPD formats.

Created model object shares the weights with the ``weights`` object. Thus, do not create ``weights`` on temporary data that can be freed later, since the model constant data will point to an invalid memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- String with a model in IR/ONNX/PDPD format.

	*
		- weights

		- Shared pointer to a constant tensor with weights. Reading ONNX/PDPD models does not support loading weights from the ``weights`` tensors.



.. rubric:: Returns:

A model.

.. _doxid-classov_1_1_core_1a46555f0803e8c29524626be08e7f5c5a:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` compile_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Creates and loads a compiled model from a source model to the default OpenVINO device selected by the AUTO plugin.

Users can create as many compiled models as they need and use them simultaneously (up to the limitation of the hardware resources).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object acquired from :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1a00c10d82856a356ae61a05eae9aecf7f:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> compile_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		Properties&&... properties
		)

Creates and loads a compiled model from a source model to the default OpenVINO device selected by AUTO plugin.

Users can create as many compiled models as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object acquired from :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation



.. rubric:: Returns:

A compiled model

.. _doxid-classov_1_1_core_1aa76b45a674acf63b901c805ee8f2ce94:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` compile_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Creates a compiled model from a source model object.

Users can create as many compiled models as they need and use them simultaneously (up to the limitation of the hardware resources).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object acquired from :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`.

	*
		- device_name

		- Name of a device to load a model to.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1a4c34bf8e08e71dfc99f7cc05ffd8c53f:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> compile_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const std::string& device_name,
		Properties&&... properties
		)

Creates a compiled model from a source model object.

Users can create as many compiled models as they need and use them simultaneously (up to the limitation of the hardware resources)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object acquired from :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`

	*
		- device_name

		- Name of device to load model to

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation



.. rubric:: Returns:

A compiled model

.. _doxid-classov_1_1_core_1a65ca9ef050647290741641d2e6e7caf3:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` compile_model(
		const std::string& model_path,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Reads and loads a compiled model from the IR/ONNX/PDPD file to the default OpenVINO device selected by the AUTO plugin.

This can be more efficient than using the :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>` + Core::compile_model(model_in_memory_object) flow, especially for cases when caching is enabled and a cached model is available.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model_path

		- Path to a model.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1a1234fffb379c06e0956f91e83991fec3:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> compile_model(
		const std::string& model_path,
		Properties&&... properties
		)

Reads and loads a compiled model from IR / ONNX / PDPD file to the default OpenVINI device selected by AUTO plugin.

This can be more efficient than using read_model + compile_model(Model) flow especially for cases when caching is enabled and cached model is available



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types

	*
		- model_path

		- path to model

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation



.. rubric:: Returns:

A compiled model

.. _doxid-classov_1_1_core_1af619069271ccc7b10f8873427ba31404:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` compile_model(
		const std::string& model_path,
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Reads a model and creates a compiled model from the IR/ONNX/PDPD file.

This can be more efficient than using the :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>` + Core::compile_model(model_in_memory_object) flow, especially for cases when caching is enabled and a cached model is available.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model_path

		- Path to a model.

	*
		- device_name

		- Name of a device to load a model to.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1aa53b76d5b7a0905ee2585fe313a60666:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> compile_model(
		const std::string& model_path,
		const std::string& device_name,
		Properties&&... properties
		)

Reads a model and creates a compiled model from the IR/ONNX/PDPD file.

This can be more efficient than using read_model + compile_model(Model) flow especially for cases when caching is enabled and cached model is available.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be a pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- model_path

		- Path to a model.

	*
		- device_name

		- Name of a device to load a model to.

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1abfc3448baa2338c93d856235cda319d1:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` compile_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Creates a compiled model from a source model within a specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object acquired from :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`.

	*
		- context

		- A reference to a :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model object.

.. _doxid-classov_1_1_core_1a3524c699eb9bb670816728b7898e4f77:
.. index:: pair: function; compile_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> compile_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
		Properties&&... properties
		)

Creates a compiled model from a source model within a specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object acquired from :ref:`Core::read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`

	*
		- context

		- Pointer to :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation



.. rubric:: Returns:

A compiled model object

.. _doxid-classov_1_1_core_1a68d0dea1cbcd42a67bea32780e32acea:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_extension(const std::shared_ptr<:ref:`InferenceEngine::IExtension<doxid-class_inference_engine_1_1_i_extension>`>& extension)

Registers OpenVINO 1.0 extension to a :ref:`Core <doxid-classov_1_1_core>` object.

Deprecated This method is deprecated. Please use other :ref:`Core::add_extension <doxid-classov_1_1_core_1a68d0dea1cbcd42a67bea32780e32acea>` methods.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- Pointer to the already loaded extension.

.. _doxid-classov_1_1_core_1adb5929d85ce33c029794f0dbbb23340f:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_extension(const std::string& library_path)

Registers an extension to a :ref:`Core <doxid-classov_1_1_core>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- library_path

		- Path to the library with :ref:`ov::Extension <doxid-classov_1_1_extension>`.

.. _doxid-classov_1_1_core_1a31767e933913bd6a8379174a6d345a2e:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_extension(const std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>& extension)

Registers an extension to a :ref:`Core <doxid-classov_1_1_core>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- Pointer to the extension.

.. _doxid-classov_1_1_core_1a77eb6bc41ba7e0174765c7ecd51764dd:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_extension(const std::vector<std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>>& extensions)

Registers extensions to a :ref:`Core <doxid-classov_1_1_core>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extensions

		- Vector of loaded extensions.

.. _doxid-classov_1_1_core_1a085742dfdd3180fecb6eae4dc4876059:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
		>
	void add_extension(const T& extension)

Registers an extension to a :ref:`Core <doxid-classov_1_1_core>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- :ref:`Extension <doxid-classov_1_1_extension>` class that is inherited from the :ref:`ov::Extension <doxid-classov_1_1_extension>` class.

.. _doxid-classov_1_1_core_1afd1c7fb8fced33c76d4b9cb53c9c21af:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		class... Targs,
		typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
		>
	void add_extension(
		const T& extension,
		Targs... args
		)

Registers extensions to a :ref:`Core <doxid-classov_1_1_core>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- :ref:`Extension <doxid-classov_1_1_extension>` class that is inherited from the :ref:`ov::Extension <doxid-classov_1_1_extension>` class.

	*
		- args

		- A list of extensions.

.. _doxid-classov_1_1_core_1abdaf09c199b3479b0a75b7bd86a7a7a5:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<std::is_base_of<ov::op::Op, T>::value, bool>::type = true
		>
	void add_extension()

Registers a custom operation inherited from :ref:`ov::op::Op <doxid-classov_1_1op_1_1_op>`.

.. _doxid-classov_1_1_core_1ab285ce1bd2a4f739b8b6bae782eb1dfd:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		class... Targs,
		typename std::enable_if<std::is_base_of<ov::op::Op, T>::value&&sizeof...(Targs), bool>::type = true
		>
	void add_extension()

Registers custom operations inherited from :ref:`ov::op::Op <doxid-classov_1_1op_1_1_op>`.

.. _doxid-classov_1_1_core_1a0d2853511bd7ba60cb591f4685b91884:
.. index:: pair: function; import_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` import_model(
		std::istream& model_stream,
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Imports a compiled model from the previously exported one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model_stream

		- std::istream input stream containing a model previously exported using the :ref:`ov::CompiledModel::export_model <doxid-classov_1_1_compiled_model_1ac9978b1d741c47286cba4eeb109effe4>` method.

	*
		- device_name

		- Name of a device to import a compiled model for. Note, if ``device_name`` device was not used to compile the original mode, an exception is thrown.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1a5acc88fb26e9b2bc2fa796b3ea82f9c7:
.. index:: pair: function; import_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> import_model(
		std::istream& model_stream,
		const std::string& device_name,
		Properties&&... properties
		)

Imports a compiled model from the previously exported one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- model_stream

		- :ref:`Model <doxid-classov_1_1_model>` stream.

	*
		- device_name

		- Name of a device to import a compiled model for. Note, if ``device_name`` device was not used to compile the original mode, an exception is thrown.

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1a319a7979bd731f3ad7e8aa4cf209727e:
.. index:: pair: function; import_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CompiledModel<doxid-classov_1_1_compiled_model>` import_model(
		std::istream& model_stream,
		const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		)

Imports a compiled model from the previously exported one with the specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model_stream

		- std::istream input stream containing a model previously exported from :ref:`ov::CompiledModel::export_model <doxid-classov_1_1_compiled_model_1ac9978b1d741c47286cba4eeb109effe4>`

	*
		- context

		- A reference to a :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object. Note, if the device from ``context`` was not used to compile the original mode, an exception is thrown.

	*
		- properties

		- Optional map of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1adde2adadfa0a523a078667b4f52046c6:
.. index:: pair: function; import_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`CompiledModel<doxid-classov_1_1_compiled_model>`, Properties...> import_model(
		std::istream& model_stream,
		const :ref:`RemoteContext<doxid-classov_1_1_remote_context>`& context,
		Properties&&... properties
		)

Imports a compiled model from the previously exported one with the specified remote context.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- model_stream

		- :ref:`Model <doxid-classov_1_1_model>` stream.

	*
		- context

		- Pointer to a :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object.

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this load operation.



.. rubric:: Returns:

A compiled model.

.. _doxid-classov_1_1_core_1acdf8e64824fe4cf147c3b52ab32c1aab:
.. index:: pair: function; query_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`SupportedOpsMap<doxid-group__ov__runtime__cpp__api_1gae52f095f7ed180ae11f2a8bca5dfc16b>` query_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties = {}
		) const

Query device if it supports the specified model with specified properties.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Name of a device to query.

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object to query.

	*
		- properties

		- Optional map of pairs: (property name, property value).



.. rubric:: Returns:

An object containing a map of pairs an operation name -> a device name supporting this operation.

.. _doxid-classov_1_1_core_1a5bee7e3a9b5ee0866add542ee17807a7:
.. index:: pair: function; query_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`SupportedOpsMap<doxid-group__ov__runtime__cpp__api_1gae52f095f7ed180ae11f2a8bca5dfc16b>`, Properties...> query_model(
		const std::shared_ptr<const :ref:`ov::Model<doxid-classov_1_1_model>`>& model,
		const std::string& device_name,
		Properties&&... properties
		) const

Queries a device if it supports the specified model with specified properties.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- device_name

		- Name of a device to query.

	*
		- model

		- :ref:`Model <doxid-classov_1_1_model>` object to query.

	*
		- properties

		- Optional pack of pairs: (property name, property value) relevant only for this query operation.



.. rubric:: Returns:

An object containing a map of pairs an operation name -> a device name supporting this operation.

.. _doxid-classov_1_1_core_1aa953cb0a1601dbc9a34ef6ba82b8476e:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_property(const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties)

Sets properties for all the registered devices, acceptable keys can be found in ``openvino/runtime/properties.hpp``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- properties

		- Map of pairs: (property name, property value).

.. _doxid-classov_1_1_core_1a3e7164e5c6865ffb458c0bcc976df6a2:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<void, Properties...> set_property(Properties&&... properties)

Sets properties for all the registered devices, acceptable keys can be found in ``openvino/runtime/properties.hpp``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be a pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- properties

		- Optional pack of pairs: property name, property value.

.. _doxid-classov_1_1_core_1a14cba2136b972ee34478dd11633293a2:
.. index:: pair: function; set_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_property(const std::string& device_name, const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& properties)

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

.. _doxid-classov_1_1_core_1abd2ef5e757bb7b5ef5a075740992e731:
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

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types.

	*
		- device_name

		- Name of a device.

	*
		- properties

		- Optional pack of pairs: (property name, property value).

.. _doxid-classov_1_1_core_1a4fb9fc7375d04f744a27a9588cbcff1a:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Any<doxid-classov_1_1_any>` get_property(const std::string& device_name, const std::string& name) const

Gets properties related to device behaviour.

The method extracts information that can be set via the set_property method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Name of a device to get a property value.

	*
		- name

		- :ref:`Property <doxid-classov_1_1_property>` name.



.. rubric:: Returns:

Value of a property corresponding to the property name.

.. _doxid-classov_1_1_core_1a448a6115a7a9eea4e0c028f9fffd37e9:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Any<doxid-classov_1_1_any>` get_property(
		const std::string& device_name,
		const std::string& name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
		) const

Gets properties related to device behaviour.

The method extracts information that can be set via the set_property method.



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

.. _doxid-classov_1_1_core_1a7e8abe0a1d9b4b9046b6eefb47be1abb:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, PropertyMutability M>
	T get_property(
		const std::string& deviceName,
		const :ref:`ov::Property<doxid-classov_1_1_property>`<T, M>& property
		) const

Gets properties related to device behaviour.

The method is needed to request common device or system properties. It can be device name, temperature, and other devices-specific values.



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

.. _doxid-classov_1_1_core_1a3267437192896805958f2d6ccfd66429:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, PropertyMutability M>
	T get_property(
		const std::string& deviceName,
		const :ref:`ov::Property<doxid-classov_1_1_property>`<T, M>& property,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& arguments
		) const

Gets properties related to device behaviour.

The method is needed to request common device or system properties. It can be device name, temperature, other devices-specific values.



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

.. _doxid-classov_1_1_core_1a018a070d2c512b247b75cf6de945e679:
.. index:: pair: function; get_property

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, PropertyMutability M, typename... Args>
	util::EnableIfAllStringAny<T, Args...> get_property(
		const std::string& deviceName,
		const :ref:`ov::Property<doxid-classov_1_1_property>`<T, M>& property,
		Args&&... args
		) const

Gets properties related to device behaviour.

The method is needed to request common device or system properties. It can be device name, temperature, other devices-specific values.



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
		- Args

		- Set of additional arguments ended with property object variable.

	*
		- deviceName

		- Name of a device to get a property value.

	*
		- property

		- :ref:`Property <doxid-classov_1_1_property>` object.

	*
		- args

		- Optional pack of pairs: (argument name, argument value) ended with property object.



.. rubric:: Returns:

:ref:`Property <doxid-classov_1_1_property>` value.

.. _doxid-classov_1_1_core_1ac4efa134a1f874cffa38c7f48f222e3a:
.. index:: pair: function; get_available_devices

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> get_available_devices() const

Returns devices available for inference. :ref:`Core <doxid-classov_1_1_core>` objects go over all registered plugins and ask about available devices.



.. rubric:: Returns:

A vector of devices. The devices are returned as { CPU, GPU.0, GPU.1, MYRIAD }. If there is more than one device of a specific type, they are enumerated with the .# suffix. Such enumerated device can later be used as a device name in all :ref:`Core <doxid-classov_1_1_core>` methods like :ref:`Core::compile_model <doxid-classov_1_1_core_1a46555f0803e8c29524626be08e7f5c5a>`, :ref:`Core::query_model <doxid-classov_1_1_core_1acdf8e64824fe4cf147c3b52ab32c1aab>`, :ref:`Core::set_property <doxid-classov_1_1_core_1aa953cb0a1601dbc9a34ef6ba82b8476e>` and so on.

.. _doxid-classov_1_1_core_1a079dcf7620d97d26d1fb2b763ca38025:
.. index:: pair: function; register_plugin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void register_plugin(
		const std::string& plugin_name,
		const std::string& device_name
		)

Register a new device and plugin that enables this device inside OpenVINO Runtime.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- plugin_name

		- 
		  Name of a plugin. Depending on platform, ``plugin_name`` is wrapped with shared library suffix and prefix to identify library full name. For example, on Linux platform, plugin name specified as ``plugin_name`` will be wrapped as ``libplugin_name.so``. Plugin search algorithm:
		  
		  * If plugin is located in the same directory as OpenVINO runtime library, it will be used.
		  
		  * If no, plugin is tried to be loaded from paths pointed by PATH/LD_LIBRARY_PATH/DYLD_LIBRARY_PATH environment variables depending on the platform.

	*
		- device_name

		- Device name to register a plugin for.

.. _doxid-classov_1_1_core_1a8ec07372698dbbe9640d15ad5da48ff2:
.. index:: pair: function; unload_plugin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void unload_plugin(const std::string& device_name)

Unloads the previously loaded plugin identified by ``device_name`` from OpenVINO Runtime. The method is needed to remove loaded plugin instance and free its resources. If plugin for a specified device has not been created before, the method throws an exception.

This method does not remove plugin from the plugins known to OpenVINO :ref:`Core <doxid-classov_1_1_core>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Device name identifying plugin to remove from OpenVINO Runtime.

.. _doxid-classov_1_1_core_1a6876f03b2e99b7ff2a78d8416dfe29ea:
.. index:: pair: function; register_plugins

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void register_plugins(const std::string& xml_config_file)

Registers a device plugin to the OpenVINO Runtime :ref:`Core <doxid-classov_1_1_core>` instance using an XML configuration file with plugins description.

The XML file has the following structure:

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

* ``name`` identifies name of a device enabled by a plugin.

* ``location`` specifies absolute path to dynamic library with a plugin. The path can also be relative to inference engine shared library. It allows having common config for different systems with different configurations.

* ``properties`` are set to a plugin via the :ref:`ov::Core::set_property <doxid-classov_1_1_core_1aa953cb0a1601dbc9a34ef6ba82b8476e>` method.

* ``extensions`` are set to a plugin via the :ref:`ov::Core::add_extension <doxid-classov_1_1_core_1a68d0dea1cbcd42a67bea32780e32acea>` method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xml_config_file

		- A path to .xml file with plugins to register.

.. _doxid-classov_1_1_core_1ab9a3eef07c3471037070242f8da2fb01:
.. index:: pair: function; create_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteContext<doxid-classov_1_1_remote_context>` create_context(
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& remote_properties
		)

Creates a new remote shared context object on the specified accelerator device using specified plugin-specific low-level device API parameters (device handle, pointer, context, etc.).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Name of a device to create a new shared context on.

	*
		- remote_properties

		- Map of device-specific shared context remote properties.



.. rubric:: Returns:

Reference to a created remote context.

.. _doxid-classov_1_1_core_1a6d80f484c89161cc3b179979134cf8ab:
.. index:: pair: function; create_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<:ref:`RemoteContext<doxid-classov_1_1_remote_context>`, Properties...> create_context(
		const std::string& device_name,
		Properties&&... remote_properties
		)

Creates a new shared context object on specified accelerator device using specified plugin-specific low level device API properties (device handle, pointer, etc.)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Properties

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types

	*
		- device_name

		- Name of a device to create new shared context on.

	*
		- remote_properties

		- Pack of device-specific shared context remote properties.



.. rubric:: Returns:

A shared pointer to a created remote context.

.. _doxid-classov_1_1_core_1a0ae465fb50e92fa63054c2d0acfd25ae:
.. index:: pair: function; get_default_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteContext<doxid-classov_1_1_remote_context>` get_default_context(const std::string& device_name)

Gets a pointer to default (plugin-supplied) shared context object for the specified accelerator device.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- Name of a device to get a default shared context from.



.. rubric:: Returns:

Reference to a default remote context.


