.. index:: pair: namespace; InferenceEngine::PluginConfigParams
.. _doxid-namespace_inference_engine_1_1_plugin_config_params:

namespace InferenceEngine::PluginConfigParams
=============================================



Overview
~~~~~~~~

Generic plugin configuration. :ref:`More...<details-namespace_inference_engine_1_1_plugin_config_params>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace PluginConfigParams {

	// global variables

	static constexpr auto :ref:`KEY_MODEL_PRIORITY<doxid-namespace_inference_engine_1_1_plugin_config_params_1afc54f5b44baa3209fb0002919b6d8341>` = "MODEL_PRIORITY";
	static constexpr auto :target:`MODEL_PRIORITY_HIGH<doxid-namespace_inference_engine_1_1_plugin_config_params_1afc340e8616e3d54c0a62fa4f22bea9bc>` = "MODEL_PRIORITY_HIGH";
	static constexpr auto :target:`MODEL_PRIORITY_MED<doxid-namespace_inference_engine_1_1_plugin_config_params_1a5972b589d2ace262369e966016d1ee87>` = "MODEL_PRIORITY_MED";
	static constexpr auto :target:`MODEL_PRIORITY_LOW<doxid-namespace_inference_engine_1_1_plugin_config_params_1abc13346d1b43d32caf0df821ac8b1d93>` = "MODEL_PRIORITY_LOW";
	static constexpr auto :ref:`KEY_PERFORMANCE_HINT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a62ae1b72a60eb8b54045f5cfa82048d3>` = "PERFORMANCE_HINT";
	static constexpr auto :target:`LATENCY<doxid-namespace_inference_engine_1_1_plugin_config_params_1a9a13ab89c9451a5d72a3cfeb53f5d74a>` = "LATENCY";
	static constexpr auto :target:`THROUGHPUT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a0902fd7a7ca168b6a188daf4b75db92f>` = "THROUGHPUT";
	static constexpr auto :target:`CUMULATIVE_THROUGHPUT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a30b03e3689d9824507ba404b71cb2d48>` = "CUMULATIVE_THROUGHPUT";
	static constexpr auto :ref:`KEY_PERFORMANCE_HINT_NUM_REQUESTS<doxid-namespace_inference_engine_1_1_plugin_config_params_1af396a7cb36e02d0a51a11f5d4c6cc85c>` = "PERFORMANCE_HINT_NUM_REQUESTS";
	static constexpr auto :ref:`KEY_ALLOW_AUTO_BATCHING<doxid-namespace_inference_engine_1_1_plugin_config_params_1a7fecce127f588c812ce5ca925b81ec07>` = "ALLOW_AUTO_BATCHING";
	static constexpr auto :ref:`YES<doxid-namespace_inference_engine_1_1_plugin_config_params_1a42d48631fa3332ded8c776513e897bf3>` = "YES";
	static constexpr auto :target:`NO<doxid-namespace_inference_engine_1_1_plugin_config_params_1a3ceab5fe6f519a82b92c7a3794561c5f>` = "NO";
	static constexpr auto :ref:`KEY_AUTO_BATCH_DEVICE_CONFIG<doxid-namespace_inference_engine_1_1_plugin_config_params_1a698874939203a09d306958261807690d>` = "AUTO_BATCH_DEVICE_CONFIG";
	static constexpr auto :ref:`KEY_AUTO_BATCH_TIMEOUT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a50dbf909c0f72673a4de8dcee99d7f42>` = "AUTO_BATCH_TIMEOUT";
	static constexpr auto :ref:`KEY_CPU_THREADS_NUM<doxid-namespace_inference_engine_1_1_plugin_config_params_1afd027d0800ad52c8658bb0098848d5ad>` = "CPU_THREADS_NUM";
	static constexpr auto :ref:`KEY_CPU_BIND_THREAD<doxid-namespace_inference_engine_1_1_plugin_config_params_1a1264fc1aa7f58c908e884eb8fbaff8b2>` = "CPU_BIND_THREAD";
	static constexpr auto :target:`NUMA<doxid-namespace_inference_engine_1_1_plugin_config_params_1a5d5f2e4ab8ae11d7fe9a718cad499615>` = "NUMA";
	static constexpr auto :target:`HYBRID_AWARE<doxid-namespace_inference_engine_1_1_plugin_config_params_1a9696ef14ba31df6345323cecfe2a4a81>` = "HYBRID_AWARE";
	static constexpr auto :ref:`KEY_CPU_THROUGHPUT_STREAMS<doxid-namespace_inference_engine_1_1_plugin_config_params_1ae04df28b5ac394e398297e432f3c7b6e>` = "CPU_THROUGHPUT_STREAMS";
	static constexpr auto :target:`CPU_THROUGHPUT_NUMA<doxid-namespace_inference_engine_1_1_plugin_config_params_1a4f5f53765f721693c02480f6f6f23f69>` = "CPU_THROUGHPUT_NUMA";
	static constexpr auto :target:`CPU_THROUGHPUT_AUTO<doxid-namespace_inference_engine_1_1_plugin_config_params_1a4cd7a5a13a764191ddb7d6fe101662ac>` = "CPU_THROUGHPUT_AUTO";
	static constexpr auto :ref:`KEY_PERF_COUNT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a06e7d1c7f8905f0915d73eba49fa1bed>` = "PERF_COUNT";
	static constexpr auto :ref:`KEY_DYN_BATCH_LIMIT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a66d52f19002274e481440b0c3a2d12e3>` = "DYN_BATCH_LIMIT";
	static constexpr auto :ref:`KEY_DYN_BATCH_ENABLED<doxid-namespace_inference_engine_1_1_plugin_config_params_1a7640912dbc0cb75c3396371760048f19>` = "DYN_BATCH_ENABLED";
	static constexpr auto :ref:`KEY_CONFIG_FILE<doxid-namespace_inference_engine_1_1_plugin_config_params_1a8b8c53f571862c6c394c67f3a66e7db2>` = "CONFIG_FILE";
	static constexpr auto :ref:`KEY_LOG_LEVEL<doxid-namespace_inference_engine_1_1_plugin_config_params_1a0ad8e81ea6681cb216494f308f353a1b>` = "LOG_LEVEL";
	static constexpr auto :target:`LOG_NONE<doxid-namespace_inference_engine_1_1_plugin_config_params_1ae1b4cc88b88790c04b96954d950b8925>` = "LOG_NONE";
	static constexpr auto :target:`LOG_ERROR<doxid-namespace_inference_engine_1_1_plugin_config_params_1a5e77bdc50b6ccd7e708f381fafa84f9b>` = "LOG_ERROR";
	static constexpr auto :target:`LOG_WARNING<doxid-namespace_inference_engine_1_1_plugin_config_params_1a5f03215b4f83d352ccaa92f406f52ddb>` = "LOG_WARNING";
	static constexpr auto :target:`LOG_INFO<doxid-namespace_inference_engine_1_1_plugin_config_params_1a0433a005740f0f892bc854ae17ec373f>` = "LOG_INFO";
	static constexpr auto :target:`LOG_DEBUG<doxid-namespace_inference_engine_1_1_plugin_config_params_1a3426ac77a15e2dcad755a6e497c2da81>` = "LOG_DEBUG";
	static constexpr auto :target:`LOG_TRACE<doxid-namespace_inference_engine_1_1_plugin_config_params_1aa7a4eca602db8c0dd756f48ec14b6081>` = "LOG_TRACE";
	static constexpr auto :ref:`KEY_DEVICE_ID<doxid-namespace_inference_engine_1_1_plugin_config_params_1a5f4163dbc2c805b6adcadb4b90033d0b>` = "DEVICE_ID";
	static constexpr auto :ref:`KEY_EXCLUSIVE_ASYNC_REQUESTS<doxid-namespace_inference_engine_1_1_plugin_config_params_1a411b655991a73fdf759a52a8a8da80d7>` = "EXCLUSIVE_ASYNC_REQUESTS";
	static constexpr auto :ref:`KEY_DUMP_EXEC_GRAPH_AS_DOT<doxid-namespace_inference_engine_1_1_plugin_config_params_1a02ac10820f3dc0b48358a343d54f3a52>` = "DUMP_EXEC_GRAPH_AS_DOT";
	static constexpr auto :ref:`KEY_ENFORCE_BF16<doxid-namespace_inference_engine_1_1_plugin_config_params_1ad07882767454df65a64f02c793c8e212>` = "ENFORCE_BF16";
	static constexpr auto :ref:`KEY_CACHE_DIR<doxid-namespace_inference_engine_1_1_plugin_config_params_1ab02b7b3b01439a8bc9570f34f9fd5e91>` = "CACHE_DIR";

	} // namespace PluginConfigParams
.. _details-namespace_inference_engine_1_1_plugin_config_params:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Generic plugin configuration.

Global Variables
----------------

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1afc54f5b44baa3209fb0002919b6d8341:
.. index:: pair: variable; KEY_MODEL_PRIORITY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_MODEL_PRIORITY = "MODEL_PRIORITY"

(Optional) config key that defines what model should be provided with more performant bounded resource first It provides 3 types of levels: High, Medium and Low. The default value is Medium

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a62ae1b72a60eb8b54045f5cfa82048d3:
.. index:: pair: variable; KEY_PERFORMANCE_HINT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_PERFORMANCE_HINT = "PERFORMANCE_HINT"

High-level OpenVINO Performance Hints unlike low-level config keys that are individual (per-device), the hints are smth that every device accepts and turns into device-specific settings.

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1af396a7cb36e02d0a51a11f5d4c6cc85c:
.. index:: pair: variable; KEY_PERFORMANCE_HINT_NUM_REQUESTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_PERFORMANCE_HINT_NUM_REQUESTS = "PERFORMANCE_HINT_NUM_REQUESTS"

(Optional) config key that backs the (above) Performance Hints by giving additional information on how many inference requests the application will be keeping in flight usually this value comes from the actual use-case (e.g. number of video-cameras, or other sources of inputs)

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a7fecce127f588c812ce5ca925b81ec07:
.. index:: pair: variable; KEY_ALLOW_AUTO_BATCHING

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_ALLOW_AUTO_BATCHING = "ALLOW_AUTO_BATCHING"

(Optional) config key that governs Auto-Batching (with YES/NO values, below)

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a42d48631fa3332ded8c776513e897bf3:
.. index:: pair: variable; YES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto YES = "YES"

generic boolean values

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a698874939203a09d306958261807690d:
.. index:: pair: variable; KEY_AUTO_BATCH_DEVICE_CONFIG

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_AUTO_BATCH_DEVICE_CONFIG = "AUTO_BATCH_DEVICE_CONFIG"

Auto-batching configuration, string for the device + batch size, e.g. "GPU(4)".

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a50dbf909c0f72673a4de8dcee99d7f42:
.. index:: pair: variable; KEY_AUTO_BATCH_TIMEOUT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_AUTO_BATCH_TIMEOUT = "AUTO_BATCH_TIMEOUT"

Auto-batching configuration: string with timeout (in ms), e.g. "100".

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1afd027d0800ad52c8658bb0098848d5ad:
.. index:: pair: variable; KEY_CPU_THREADS_NUM

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_CPU_THREADS_NUM = "CPU_THREADS_NUM"

Limit ``#threads`` that are used by Inference Engine for inference on the CPU.

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a1264fc1aa7f58c908e884eb8fbaff8b2:
.. index:: pair: variable; KEY_CPU_BIND_THREAD

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_CPU_BIND_THREAD = "CPU_BIND_THREAD"

The name for setting CPU affinity per thread option.

It is passed to :ref:`Core::SetConfig() <doxid-class_inference_engine_1_1_core_1a34aa9ac6fb237b634d5bf08b288e88d4>`, this option should be used with values: :ref:`PluginConfigParams::NO <doxid-namespace_inference_engine_1_1_plugin_config_params_1a3ceab5fe6f519a82b92c7a3794561c5f>` (no pinning for CPU inference threads) :ref:`PluginConfigParams::YES <doxid-namespace_inference_engine_1_1_plugin_config_params_1a42d48631fa3332ded8c776513e897bf3>`, which is default on the conventional CPUs (pinning threads to cores, best for static benchmarks),

the following options are implemented only for the TBB as a threading option :ref:`PluginConfigParams::NUMA <doxid-namespace_inference_engine_1_1_plugin_config_params_1a5d5f2e4ab8ae11d7fe9a718cad499615>` (pinning threads to NUMA nodes, best for real-life, contented cases) on the Windows and MacOS\* this option behaves as YES :ref:`PluginConfigParams::HYBRID_AWARE <doxid-namespace_inference_engine_1_1_plugin_config_params_1a9696ef14ba31df6345323cecfe2a4a81>` (let the runtime to do pinning to the cores types, e.g. prefer the "big" cores for latency tasks) on the hybrid CPUs this option is default

Also, the settings are ignored, if the OpenVINO compiled with OpenMP and any affinity-related OpenMP's environment variable is set (as affinity is configured explicitly)

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1ae04df28b5ac394e398297e432f3c7b6e:
.. index:: pair: variable; KEY_CPU_THROUGHPUT_STREAMS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_CPU_THROUGHPUT_STREAMS = "CPU_THROUGHPUT_STREAMS"

Optimize CPU execution to maximize throughput.

It is passed to :ref:`Core::SetConfig() <doxid-class_inference_engine_1_1_core_1a34aa9ac6fb237b634d5bf08b288e88d4>`, this option should be used with values:

* KEY_CPU_THROUGHPUT_NUMA creates as many streams as needed to accommodate NUMA and avoid associated penalties

* KEY_CPU_THROUGHPUT_AUTO creates bare minimum of streams to improve the performance, this is the most portable option if you have no insights into how many cores you target machine will have (and what is the optimal number of streams)

* finally, specifying the positive integer value creates the requested number of streams

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a06e7d1c7f8905f0915d73eba49fa1bed:
.. index:: pair: variable; KEY_PERF_COUNT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_PERF_COUNT = "PERF_COUNT"

The name for setting performance counters option.

It is passed to :ref:`Core::SetConfig() <doxid-class_inference_engine_1_1_core_1a34aa9ac6fb237b634d5bf08b288e88d4>`, this option should be used with values: :ref:`PluginConfigParams::YES <doxid-namespace_inference_engine_1_1_plugin_config_params_1a42d48631fa3332ded8c776513e897bf3>` or :ref:`PluginConfigParams::NO <doxid-namespace_inference_engine_1_1_plugin_config_params_1a3ceab5fe6f519a82b92c7a3794561c5f>`

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a66d52f19002274e481440b0c3a2d12e3:
.. index:: pair: variable; KEY_DYN_BATCH_LIMIT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_DYN_BATCH_LIMIT = "DYN_BATCH_LIMIT"

The key defines dynamic limit of batch processing.

Specified value is applied to all following Infer() calls. Inference Engine processes min(batch_limit, original_batch_size) first pictures from input blob. For example, if input blob has sizes 32x3x224x224 after applying plugin.SetConfig({KEY_DYN_BATCH_LIMIT, 10}) Inference Engine primitives processes only beginner subblobs with size 10x3x224x224. This value can be changed before any Infer() call to specify a new batch limit.

The paired parameter value should be convertible to integer number. Acceptable values: -1 - Do not limit batch processing >0 - Direct value of limit. Batch size to process is min(new batch_limit, original_batch)

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a7640912dbc0cb75c3396371760048f19:
.. index:: pair: variable; KEY_DYN_BATCH_ENABLED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_DYN_BATCH_ENABLED = "DYN_BATCH_ENABLED"

The key checks whether dynamic batch is enabled.

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a8b8c53f571862c6c394c67f3a66e7db2:
.. index:: pair: variable; KEY_CONFIG_FILE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_CONFIG_FILE = "CONFIG_FILE"

This key directs the plugin to load a configuration file.

The value should be a file name with the plugin specific configuration

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a0ad8e81ea6681cb216494f308f353a1b:
.. index:: pair: variable; KEY_LOG_LEVEL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_LOG_LEVEL = "LOG_LEVEL"

the key for setting desirable log level.

This option should be used with values: :ref:`PluginConfigParams::LOG_NONE <doxid-namespace_inference_engine_1_1_plugin_config_params_1ae1b4cc88b88790c04b96954d950b8925>` (default), :ref:`PluginConfigParams::LOG_ERROR <doxid-namespace_inference_engine_1_1_plugin_config_params_1a5e77bdc50b6ccd7e708f381fafa84f9b>`, :ref:`PluginConfigParams::LOG_WARNING <doxid-namespace_inference_engine_1_1_plugin_config_params_1a5f03215b4f83d352ccaa92f406f52ddb>`, :ref:`PluginConfigParams::LOG_INFO <doxid-namespace_inference_engine_1_1_plugin_config_params_1a0433a005740f0f892bc854ae17ec373f>`, :ref:`PluginConfigParams::LOG_DEBUG <doxid-namespace_inference_engine_1_1_plugin_config_params_1a3426ac77a15e2dcad755a6e497c2da81>`, :ref:`PluginConfigParams::LOG_TRACE <doxid-namespace_inference_engine_1_1_plugin_config_params_1aa7a4eca602db8c0dd756f48ec14b6081>`

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a5f4163dbc2c805b6adcadb4b90033d0b:
.. index:: pair: variable; KEY_DEVICE_ID

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_DEVICE_ID = "DEVICE_ID"

the key for setting of required device to execute on values: device id starts from "0" - first device, "1" - second device, etc

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a411b655991a73fdf759a52a8a8da80d7:
.. index:: pair: variable; KEY_EXCLUSIVE_ASYNC_REQUESTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_EXCLUSIVE_ASYNC_REQUESTS = "EXCLUSIVE_ASYNC_REQUESTS"

the key for enabling exclusive mode for async requests of different executable networks and the same plugin.

Sometimes it is necessary to avoid oversubscription requests that are sharing the same device in parallel. E.g. There 2 task executors for CPU device: one - in the Hetero plugin, another - in pure CPU plugin. Parallel execution both of them might lead to oversubscription and not optimal CPU usage. More efficient to run the corresponding tasks one by one via single executor. By default, the option is set to YES for hetero cases, and to NO for conventional (single-plugin) cases Notice that setting YES disables the CPU streams feature (see another config key in this file)

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1a02ac10820f3dc0b48358a343d54f3a52:
.. index:: pair: variable; KEY_DUMP_EXEC_GRAPH_AS_DOT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_DUMP_EXEC_GRAPH_AS_DOT = "DUMP_EXEC_GRAPH_AS_DOT"

This key enables dumping of the internal primitive graph.

Deprecated Use InferenceEngine::ExecutableNetwork::GetExecGraphInfo::serialize method

Should be passed into LoadNetwork method to enable dumping of internal graph of primitives and corresponding configuration information. Value is a name of output dot file without extension. Files ``<dot_file_name>_init.dot`` and ``<dot_file_name>_perf.dot`` will be produced.

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1ad07882767454df65a64f02c793c8e212:
.. index:: pair: variable; KEY_ENFORCE_BF16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_ENFORCE_BF16 = "ENFORCE_BF16"

The name for setting to execute in bfloat16 precision whenever it is possible.

This option let plugin know to downscale the precision where it see performance benefits from bfloat16 execution Such option do not guarantee accuracy of the network, the accuracy in this mode should be verified separately by the user and basing on performance and accuracy results it should be user's decision to use this option or not to use

.. _doxid-namespace_inference_engine_1_1_plugin_config_params_1ab02b7b3b01439a8bc9570f34f9fd5e91:
.. index:: pair: variable; KEY_CACHE_DIR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto KEY_CACHE_DIR = "CACHE_DIR"

This key defines the directory which will be used to store any data cached by plugins.

The underlying cache structure is not defined and might differ between OpenVINO releases Cached data might be platform / device specific and might be invalid after OpenVINO version change If this key is not specified or value is empty string, then caching is disabled. The key might enable caching for the plugin using the following code:

.. ref-code-block:: cpp

	ie.SetConfig({{CONFIG_KEY(CACHE_DIR), "cache/"}}, "GPU"); // enables cache for GPU plugin

The following code enables caching of compiled network blobs for devices where import/export is supported

.. ref-code-block:: cpp

	ie.SetConfig({{CONFIG_KEY(CACHE_DIR), "cache/"}}); // enables models cache

