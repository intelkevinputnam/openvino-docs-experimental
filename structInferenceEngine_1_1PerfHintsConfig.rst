.. index:: pair: struct; InferenceEngine::PerfHintsConfig
.. _doxid-struct_inference_engine_1_1_perf_hints_config:

struct InferenceEngine::PerfHintsConfig
=======================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_performance_hints.hpp>
	
	struct PerfHintsConfig
	{
		// fields
	
		std::string :target:`ovPerfHint<doxid-struct_inference_engine_1_1_perf_hints_config_1a3a885bcc11b65684d9a450979951ef3d>` = "";
		int :target:`ovPerfHintNumRequests<doxid-struct_inference_engine_1_1_perf_hints_config_1a24c2dbe718a161292c1a29e4ef16682f>` = 0;

		// methods
	
		void :ref:`SetConfig<doxid-struct_inference_engine_1_1_perf_hints_config_1a8afe92e60333055a4c8586a73e271432>`(const std::string& key, const std::string& value);
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-struct_inference_engine_1_1_perf_hints_config_1af6e60126cd0853fc713df268030bdeec>`(const std::string& key);
		static std::vector<std::string> :ref:`SupportedKeys<doxid-struct_inference_engine_1_1_perf_hints_config_1aa653d0612ffad334006df8de99c810ba>`();
		static void :ref:`CheckConfigAndValue<doxid-struct_inference_engine_1_1_perf_hints_config_1af74a6a67c55a8640108bdeaea7fd53b4>`(std::pair<const std::string, const std::string&> kvp);
		static std::string :ref:`CheckPerformanceHintValue<doxid-struct_inference_engine_1_1_perf_hints_config_1a7eb2432f230a4b3244fcf9d4e1f7d803>`(const std::string& val);
		static int :ref:`CheckPerformanceHintRequestValue<doxid-struct_inference_engine_1_1_perf_hints_config_1af31081518a716102c3fed56141faa505>`(const std::string& val);
	};
.. _details-struct_inference_engine_1_1_perf_hints_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-struct_inference_engine_1_1_perf_hints_config_1a8afe92e60333055a4c8586a73e271432:
.. index:: pair: function; SetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void SetConfig(const std::string& key, const std::string& value)

Parses configuration key/value pair.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- key

		- configuration key

	*
		- value

		- configuration values

.. _doxid-struct_inference_engine_1_1_perf_hints_config_1af6e60126cd0853fc713df268030bdeec:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetConfig(const std::string& key)

Return configuration value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- key

		- configuration key



.. rubric:: Returns:

configuration value wrapped into Parameter

.. _doxid-struct_inference_engine_1_1_perf_hints_config_1aa653d0612ffad334006df8de99c810ba:
.. index:: pair: function; SupportedKeys

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::vector<std::string> SupportedKeys()

Supported Configuration keys.



.. rubric:: Returns:

vector of supported configuration keys

.. _doxid-struct_inference_engine_1_1_perf_hints_config_1af74a6a67c55a8640108bdeaea7fd53b4:
.. index:: pair: function; CheckConfigAndValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void CheckConfigAndValue(std::pair<const std::string, const std::string&> kvp)

Checks configuration key and value, otherwise throws.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- configuration

		- key + value



.. rubric:: Returns:

void

.. _doxid-struct_inference_engine_1_1_perf_hints_config_1a7eb2432f230a4b3244fcf9d4e1f7d803:
.. index:: pair: function; CheckPerformanceHintValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::string CheckPerformanceHintValue(const std::string& val)

Returns configuration value if it is valid, otherwise throws.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- configuration

		- value



.. rubric:: Returns:

configuration value

.. _doxid-struct_inference_engine_1_1_perf_hints_config_1af31081518a716102c3fed56141faa505:
.. index:: pair: function; CheckPerformanceHintRequestValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static int CheckPerformanceHintRequestValue(const std::string& val)

Returns configuration value if it is valid, otherwise throws.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- configuration

		- value as string



.. rubric:: Returns:

configuration value as number


