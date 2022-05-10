.. index:: pair: group; Plugin base classes
.. _doxid-group__ie__dev__api__plugin__api:

Plugin base classes
===================

.. toctree::
	:hidden:

	PluginConfigInternalParams <namespaceInferenceEngine_1_1PluginConfigInternalParams.rst>
	ICore <classov_1_1ICore.rst>
	IInferencePlugin <classInferenceEngine_1_1IInferencePlugin.rst>

Overview
~~~~~~~~

A set of base and helper classes to implement a plugin class. :ref:`More...<details-group__ie__dev__api__plugin__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`InferenceEngine::PluginConfigInternalParams<doxid-namespace_inference_engine_1_1_plugin_config_internal_params>`;

	// templates

	template :ref:`ov::ICore<doxid-classov_1_1_i_core>`;
	template :ref:`InferenceEngine::IInferencePlugin<doxid-class_inference_engine_1_1_i_inference_plugin>`;

	// macros

	#define :ref:`CONFIG_KEY_INTERNAL<doxid-group__ie__dev__api__plugin__api_1ga467101d10535ee20c68d110957c75334>`(name)
	#define :ref:`CONFIG_VALUE_INTERNAL<doxid-group__ie__dev__api__plugin__api_1ga698a6c9b92df3c0cd02d89c17b07d8c3>`(name)
	#define :ref:`IE_CREATE_PLUGIN<doxid-group__ie__dev__api__plugin__api_1ga99b18089a6c2b980a7b68538886041ae>`
	#define :ref:`IE_DEFINE_PLUGIN_CREATE_FUNCTION<doxid-group__ie__dev__api__plugin__api_1ga06b197cbe37f59f94b15a7d861e17d4e>`(PluginType, version, ...)

.. _details-group__ie__dev__api__plugin__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A set of base and helper classes to implement a plugin class.

Macros
------

.. _doxid-group__ie__dev__api__plugin__api_1ga467101d10535ee20c68d110957c75334:
.. index:: pair: define; CONFIG_KEY_INTERNAL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define CONFIG_KEY_INTERNAL(name)

Shortcut for defining internal configuration keys.

.. _doxid-group__ie__dev__api__plugin__api_1ga698a6c9b92df3c0cd02d89c17b07d8c3:
.. index:: pair: define; CONFIG_VALUE_INTERNAL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define CONFIG_VALUE_INTERNAL(name)

Shortcut for defining internal configuration values.

.. _doxid-group__ie__dev__api__plugin__api_1ga99b18089a6c2b980a7b68538886041ae:
.. index:: pair: define; IE_CREATE_PLUGIN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_CREATE_PLUGIN

Defines a name of a function creating plugin instance.

.. _doxid-group__ie__dev__api__plugin__api_1ga06b197cbe37f59f94b15a7d861e17d4e:
.. index:: pair: define; IE_DEFINE_PLUGIN_CREATE_FUNCTION

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_DEFINE_PLUGIN_CREATE_FUNCTION(PluginType, version, ...)

Defines the exported ``IE_CREATE_PLUGIN`` function which is used to create a plugin instance.

