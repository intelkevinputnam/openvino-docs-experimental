.. index:: pair: struct; InferenceEngine::IStreamsExecutor::Config
.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config:

struct InferenceEngine::IStreamsExecutor::Config
================================================

.. toctree::
	:hidden:

	PreferredCoreType <enumInferenceEngine_1_1IStreamsExecutor_1_1Config_1_1PreferredCoreType.rst>

Overview
~~~~~~~~

Defines :ref:`IStreamsExecutor <doxid-class_inference_engine_1_1_i_streams_executor>` configuration. :ref:`More...<details-struct_inference_engine_1_1_i_streams_executor_1_1_config>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_istreams_executor.hpp>
	
	struct Config
	{
		// enums
	
		enum :ref:`PreferredCoreType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a522c480fde618152bec3c01ff470e84e>`;

		// fields
	
		std::string :ref:`_name<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1aef59325cbbe6a22cb667c88aa7c07c23>`;
		int :ref:`_streams<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a5dc259789f67b2f1af1461fc0cb8f033>` = 1;
		int :ref:`_threadsPerStream<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a8f544685992465ae279f6dbfe3ba6f1d>` = 0;
		:ref:`ThreadBindingType<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>` :ref:`_threadBindingType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a944fd72d6d1cbdb2a9a31499ea5d0b1c>` = ThreadBindingType::NONE;
		int :ref:`_threadBindingStep<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a05ba9a478614b69b151f1f276c730ba0>` = 1;
		int :ref:`_threadBindingOffset<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1ad463dfbd1548760f2ca19b9d9f52ff24>` = 0;
		int :ref:`_threads<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a4ad9d4c405e21ef198aecf92fc48e6c3>` = 0;
		enum :ref:`InferenceEngine::IStreamsExecutor::Config::PreferredCoreType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a522c480fde618152bec3c01ff470e84e>` :ref:`_threadPreferredCoreType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a478003234b78c6be420ec4e2073fc991>` =             PreferredCoreType::ANY;

		// construction
	
		:ref:`Config<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a49a38a03969d371ee5080fc1a83a0660>`(
			std::string name = "StreamsExecutor",
			int streams = 1,
			int threadsPerStream = 0,
			:ref:`ThreadBindingType<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>` threadBindingType = ThreadBindingType::NONE,
			int threadBindingStep = 1,
			int threadBindingOffset = 0,
			int threads = 0,
			:ref:`PreferredCoreType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a522c480fde618152bec3c01ff470e84e>` threadPreferredCoreType = PreferredCoreType::ANY
			);

		// methods
	
		std::vector<std::string> :ref:`SupportedKeys<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1af5194c42f86951299ba6a9ef334627ef>`() const;
		void :ref:`SetConfig<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a55b63d4d95c2c3f856b603dd128ea2b4>`(const std::string& key, const std::string& value);
		:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` :ref:`GetConfig<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a3fc899627d5a662b5920ca799d46299f>`(const std::string& key) const;
	
		static Config :ref:`MakeDefaultMultiThreaded<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1aa86ace5a369404be513fe5accb022dbb>`(
			const Config& initial,
			const bool fp_intesive = true
			);
	
		static int :ref:`GetDefaultNumStreams<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1ab86436e8439920f4781b7a9a38ea392c>`();
	};
.. _details-struct_inference_engine_1_1_i_streams_executor_1_1_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Defines :ref:`IStreamsExecutor <doxid-class_inference_engine_1_1_i_streams_executor>` configuration.

Fields
------

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1aef59325cbbe6a22cb667c88aa7c07c23:
.. index:: pair: variable; _name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string _name

Used by ``ITT`` to name executor threads.

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a5dc259789f67b2f1af1461fc0cb8f033:
.. index:: pair: variable; _streams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int _streams = 1

Number of streams.

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a8f544685992465ae279f6dbfe3ba6f1d:
.. index:: pair: variable; _threadsPerStream

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int _threadsPerStream = 0

Number of threads per stream that executes ``ie_parallel`` calls.

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a944fd72d6d1cbdb2a9a31499ea5d0b1c:
.. index:: pair: variable; _threadBindingType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ThreadBindingType<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>` _threadBindingType = ThreadBindingType::NONE

Thread binding to hardware resource type. No binding by default

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a05ba9a478614b69b151f1f276c730ba0:
.. index:: pair: variable; _threadBindingStep

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int _threadBindingStep = 1

In case of :ref:`CORES <doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872ac31f62d8f7987f4816c5fbfffb26429f>` binding offset type thread binded to cores with defined step

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1ad463dfbd1548760f2ca19b9d9f52ff24:
.. index:: pair: variable; _threadBindingOffset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int _threadBindingOffset = 0

In case of :ref:`CORES <doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872ac31f62d8f7987f4816c5fbfffb26429f>` binding offset type thread binded to cores starting from offset

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a4ad9d4c405e21ef198aecf92fc48e6c3:
.. index:: pair: variable; _threads

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int _threads = 0

Number of threads distributed between streams. Reserved. Should not be used.

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a478003234b78c6be420ec4e2073fc991:
.. index:: pair: variable; _threadPreferredCoreType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	enum :ref:`InferenceEngine::IStreamsExecutor::Config::PreferredCoreType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a522c480fde618152bec3c01ff470e84e>` _threadPreferredCoreType =             PreferredCoreType::ANY

In case of :ref:`HYBRID_AWARE <doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872a1a7a5d64f7a66531b134c7caf524ad81>` hints the TBB to affinitize.

Construction
------------

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a49a38a03969d371ee5080fc1a83a0660:
.. index:: pair: function; Config

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Config(
		std::string name = "StreamsExecutor",
		int streams = 1,
		int threadsPerStream = 0,
		:ref:`ThreadBindingType<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>` threadBindingType = ThreadBindingType::NONE,
		int threadBindingStep = 1,
		int threadBindingOffset = 0,
		int threads = 0,
		:ref:`PreferredCoreType<doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a522c480fde618152bec3c01ff470e84e>` threadPreferredCoreType = PreferredCoreType::ANY
		)

A constructor with arguments.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- The executor name

	*
		- streams

		- Number of streams.

	*
		- threadsPerStream

		- Number of threads per stream that executes ``ie_parallel`` calls.

	*
		- threadBindingType

		- 

	*
		- threadBindingStep

		- 

	*
		- threadBindingOffset

		- 

	*
		- threads

		- 

	*
		- threadPreferBigCores

		-

Methods
-------

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1af5194c42f86951299ba6a9ef334627ef:
.. index:: pair: function; SupportedKeys

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> SupportedKeys() const

Supported Configuration keys.



.. rubric:: Returns:

vector of supported configuration keys

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a55b63d4d95c2c3f856b603dd128ea2b4:
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

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1a3fc899627d5a662b5920ca799d46299f:
.. index:: pair: function; GetConfig

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Parameter<doxid-namespace_inference_engine_1aff2231f886c9f8fc9c226fd343026789>` GetConfig(const std::string& key) const

Return configuration value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- key

		- configuration key



.. rubric:: Returns:

configuration value wrapped into Parameter

.. _doxid-struct_inference_engine_1_1_i_streams_executor_1_1_config_1aa86ace5a369404be513fe5accb022dbb:
.. index:: pair: function; MakeDefaultMultiThreaded

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static Config MakeDefaultMultiThreaded(
		const Config& initial,
		const bool fp_intesive = true
		)

Create appropriate multithreaded configuration filing unconfigured values from initial configuration using hardware properties.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- initial

		- Inital configuration

	*
		- fp_intesive

		- additional hint for the the (Hybrid) core-types selection logic whether the executor should be configured for floating point intensive work (as opposite to int8 intensive)



.. rubric:: Returns:

configured values


