.. index:: pair: namespace; InferenceEngine::Metrics
.. _doxid-namespace_inference_engine_1_1_metrics:

namespace InferenceEngine::Metrics
==================================

.. toctree::
	:hidden:

	DeviceType <enumInferenceEngine_1_1Metrics_1_1DeviceType.rst>

Overview
~~~~~~~~

Metrics :ref:`More...<details-namespace_inference_engine_1_1_metrics>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace Metrics {

	// enums

	enum :ref:`DeviceType<doxid-namespace_inference_engine_1_1_metrics_1af18bf88a30d9dca9a14038c76aeae805>`;

	// global variables

	static constexpr auto :ref:`METRIC_AVAILABLE_DEVICES<doxid-namespace_inference_engine_1_1_metrics_1a04ce5d4fb24fde259b329caffa358fa5>` =  "AVAILABLE_DEVICES";
	static constexpr auto :ref:`METRIC_SUPPORTED_METRICS<doxid-namespace_inference_engine_1_1_metrics_1a67a2c5ea1cb1ea7d42c71b8bf0d0b97d>` =  "SUPPORTED_METRICS";
	static constexpr auto :ref:`METRIC_SUPPORTED_CONFIG_KEYS<doxid-namespace_inference_engine_1_1_metrics_1a41d90ac79d73d8706ae2e9eb46a673a1>` =  "SUPPORTED_CONFIG_KEYS";
	static constexpr auto :ref:`METRIC_FULL_DEVICE_NAME<doxid-namespace_inference_engine_1_1_metrics_1a33c5772e0e22fab7b981cb33c2820f32>` =  "FULL_DEVICE_NAME";
	static constexpr auto :ref:`METRIC_OPTIMIZATION_CAPABILITIES<doxid-namespace_inference_engine_1_1_metrics_1a54ebc63520c179a5854f5a199d24e1d2>` =  "OPTIMIZATION_CAPABILITIES";
	static constexpr auto :target:`FP32<doxid-namespace_inference_engine_1_1_metrics_1a33f8ec1373b4a3550b87abf3a7773aa2>` = "FP32";
	static constexpr auto :target:`BF16<doxid-namespace_inference_engine_1_1_metrics_1a52363b102c11b099d764aeeec84bf555>` = "BF16";
	static constexpr auto :target:`FP16<doxid-namespace_inference_engine_1_1_metrics_1a45ef215735092ccc913e9d6c54cfb226>` = "FP16";
	static constexpr auto :target:`INT8<doxid-namespace_inference_engine_1_1_metrics_1ad31c07cfba5d2d2859af67742ca5a89b>` = "INT8";
	static constexpr auto :target:`BIN<doxid-namespace_inference_engine_1_1_metrics_1a888cf88b6ec040a80dc63b4995be2b0a>` = "BIN";
	static constexpr auto :target:`WINOGRAD<doxid-namespace_inference_engine_1_1_metrics_1a765ae7767f0eca6abc8dfaa67ce5d2ee>` = "WINOGRAD";
	static constexpr auto :target:`BATCHED_BLOB<doxid-namespace_inference_engine_1_1_metrics_1a85275335fc433b45a95bf2fa0392906d>` = "BATCHED_BLOB";
	static constexpr auto :ref:`METRIC_RANGE_FOR_STREAMS<doxid-namespace_inference_engine_1_1_metrics_1a39f21cea314e4a122b857d4112be2eb1>` =  "RANGE_FOR_STREAMS";
	static constexpr auto :ref:`METRIC_OPTIMAL_BATCH_SIZE<doxid-namespace_inference_engine_1_1_metrics_1a968dac22a47169809d9589cb4c211f97>` =  "OPTIMAL_BATCH_SIZE";
	static constexpr auto :ref:`METRIC_MAX_BATCH_SIZE<doxid-namespace_inference_engine_1_1_metrics_1a5469d6dadbd3297e3a5ece72701ebee5>` =  "MAX_BATCH_SIZE";
	static constexpr auto :ref:`METRIC_RANGE_FOR_ASYNC_INFER_REQUESTS<doxid-namespace_inference_engine_1_1_metrics_1a4335554dc78de02b95418bb29ade2831>` =  "RANGE_FOR_ASYNC_INFER_REQUESTS";
	static constexpr auto :ref:`METRIC_NUMBER_OF_WAITING_INFER_REQUESTS<doxid-namespace_inference_engine_1_1_metrics_1a4cc6b8c1b548fad1e03ea2a897b15400>` =  "NUMBER_OF_WAITING_INFER_REQUESTS";
	static constexpr auto :ref:`METRIC_NUMBER_OF_EXEC_INFER_REQUESTS<doxid-namespace_inference_engine_1_1_metrics_1a8bb4bb50ecf459e83f2dec54e5506e0b>` =  "NUMBER_OF_EXEC_INFER_REQUESTS";
	static constexpr auto :ref:`METRIC_DEVICE_ARCHITECTURE<doxid-namespace_inference_engine_1_1_metrics_1a8869591f9fc938a5caf68d05109ab348>` =  "DEVICE_ARCHITECTURE";
	static constexpr auto :ref:`METRIC_DEVICE_TYPE<doxid-namespace_inference_engine_1_1_metrics_1af5394d85cc2ede6485a65b1707e5b262>` =  "DEVICE_TYPE";
	static constexpr auto :ref:`METRIC_DEVICE_GOPS<doxid-namespace_inference_engine_1_1_metrics_1a6a0aefa372f436611dea9b92cd768ff1>` =  "DEVICE_GOPS";
	static constexpr auto :ref:`METRIC_IMPORT_EXPORT_SUPPORT<doxid-namespace_inference_engine_1_1_metrics_1a8ca1a5188eba1ec5ad73f951f0949381>` =  "IMPORT_EXPORT_SUPPORT";
	static constexpr auto :ref:`METRIC_NETWORK_NAME<doxid-namespace_inference_engine_1_1_metrics_1ac8a47d4063517a77764b632962d4cc8d>` =  "NETWORK_NAME";
	static constexpr auto :ref:`METRIC_DEVICE_THERMAL<doxid-namespace_inference_engine_1_1_metrics_1a2f746c0fabfb75a6fced6cf394cb9b2e>` =  "DEVICE_THERMAL";
	static constexpr auto :ref:`METRIC_OPTIMAL_NUMBER_OF_INFER_REQUESTS<doxid-namespace_inference_engine_1_1_metrics_1a57a821fbccfb015f161e00b805415a58>` =  "OPTIMAL_NUMBER_OF_INFER_REQUESTS";

	} // namespace Metrics
.. _details-namespace_inference_engine_1_1_metrics:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Metrics

Global Variables
----------------

.. _doxid-namespace_inference_engine_1_1_metrics_1a04ce5d4fb24fde259b329caffa358fa5:
.. index:: pair: variable; METRIC_AVAILABLE_DEVICES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_AVAILABLE_DEVICES =  "AVAILABLE_DEVICES"

Metric to get a std::vector<std::string> of available device IDs. String value is "AVAILABLE_DEVICES".

.. _doxid-namespace_inference_engine_1_1_metrics_1a67a2c5ea1cb1ea7d42c71b8bf0d0b97d:
.. index:: pair: variable; METRIC_SUPPORTED_METRICS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_SUPPORTED_METRICS =  "SUPPORTED_METRICS"

Metric to get a std::vector<std::string> of supported metrics. String value is "SUPPORTED_METRICS".

This can be used as an executable network metric as well.

Each of the returned device metrics can be passed to :ref:`Core::GetMetric <doxid-class_inference_engine_1_1_core_1a27b1476aa8095c237eeabacfce73b38e>`, executable network metrics can be passed to :ref:`ExecutableNetwork::GetMetric <doxid-class_inference_engine_1_1_executable_network_1a5b38590cad3a68144c679af5f5a6090d>`.

.. _doxid-namespace_inference_engine_1_1_metrics_1a41d90ac79d73d8706ae2e9eb46a673a1:
.. index:: pair: variable; METRIC_SUPPORTED_CONFIG_KEYS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_SUPPORTED_CONFIG_KEYS =  "SUPPORTED_CONFIG_KEYS"

Metric to get a std::vector<std::string> of supported config keys. String value is "SUPPORTED_CONFIG_KEYS".

This can be used as an executable network metric as well.

Each of the returned device configuration keys can be passed to :ref:`Core::SetConfig <doxid-class_inference_engine_1_1_core_1a34aa9ac6fb237b634d5bf08b288e88d4>`, :ref:`Core::GetConfig <doxid-class_inference_engine_1_1_core_1a415077386694f95b57e4cccb0d334a55>`, and :ref:`Core::LoadNetwork <doxid-class_inference_engine_1_1_core_1a7b0b5ab0009abc572762422105b5c666>`, configuration keys for executable networks can be passed to :ref:`ExecutableNetwork::SetConfig <doxid-class_inference_engine_1_1_executable_network_1aa1ed6418b25be96a413c452ca8c1480a>` and :ref:`ExecutableNetwork::GetConfig <doxid-class_inference_engine_1_1_executable_network_1af43953e9d84965914d1ce50f90480145>`.

.. _doxid-namespace_inference_engine_1_1_metrics_1a33c5772e0e22fab7b981cb33c2820f32:
.. index:: pair: variable; METRIC_FULL_DEVICE_NAME

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_FULL_DEVICE_NAME =  "FULL_DEVICE_NAME"

Metric to get a std::string value representing a full device name. String value is "FULL_DEVICE_NAME".

.. _doxid-namespace_inference_engine_1_1_metrics_1a54ebc63520c179a5854f5a199d24e1d2:
.. index:: pair: variable; METRIC_OPTIMIZATION_CAPABILITIES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_OPTIMIZATION_CAPABILITIES =  "OPTIMIZATION_CAPABILITIES"

Metric to get a std::vector<std::string> of optimization options per device. String value is "OPTIMIZATION_CAPABILITIES".

The possible values:

* "FP32" - device can support FP32 models

* "BF16" - device can support BF16 computations for models

* "FP16" - device can support FP16 models

* "INT8" - device can support models with INT8 layers

* "BIN" - device can support models with BIN layers

* "WINOGRAD" - device can support models where convolution implemented via Winograd transformations

* "BATCHED_BLOB" - device can support :ref:`BatchedBlob <doxid-class_inference_engine_1_1_batched_blob>`

.. _doxid-namespace_inference_engine_1_1_metrics_1a39f21cea314e4a122b857d4112be2eb1:
.. index:: pair: variable; METRIC_RANGE_FOR_STREAMS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_RANGE_FOR_STREAMS =  "RANGE_FOR_STREAMS"

Metric to provide information about a range for streams on platforms where streams are supported.

Metric returns a value of std::tuple<unsigned int, unsigned int> type, where:

* First value is bottom bound.

* Second value is upper bound. String value for metric name is "RANGE_FOR_STREAMS".

.. _doxid-namespace_inference_engine_1_1_metrics_1a968dac22a47169809d9589cb4c211f97:
.. index:: pair: variable; METRIC_OPTIMAL_BATCH_SIZE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_OPTIMAL_BATCH_SIZE =  "OPTIMAL_BATCH_SIZE"

Metric to query information optimal batch size for the given device and the network.

Metric returns a value of unsigned int type, Returns optimal batch size for a given network on the given device. The returned value is aligned to power of 2. Also, MODEL_PTR is the required option for this metric since the optimal batch size depends on the model, so if the MODEL_PTR is not given, the result of the metric is always 1. For the GPU the metric is queried automatically whenever the OpenVINO performance hint for the throughput is used, so that the result (>1) governs the automatic batching (transparently to the application). The automatic batching can be disabled with ALLOW_AUTO_BATCHING set to NO

.. _doxid-namespace_inference_engine_1_1_metrics_1a5469d6dadbd3297e3a5ece72701ebee5:
.. index:: pair: variable; METRIC_MAX_BATCH_SIZE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_MAX_BATCH_SIZE =  "MAX_BATCH_SIZE"

Metric to get maximum batch size which does not cause performance degradation due to memory swap impact.

Metric returns a value of unsigned int type, Note that the returned value may not aligned to power of 2. Also, MODEL_PTR is the required option for this metric since the available max batch size depends on the model size. If the MODEL_PTR is not given, it will return 1.

.. _doxid-namespace_inference_engine_1_1_metrics_1a4335554dc78de02b95418bb29ade2831:
.. index:: pair: variable; METRIC_RANGE_FOR_ASYNC_INFER_REQUESTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_RANGE_FOR_ASYNC_INFER_REQUESTS =  "RANGE_FOR_ASYNC_INFER_REQUESTS"

Metric to provide a hint for a range for number of async infer requests. If device supports streams, the metric provides range for number of IRs per stream.

Metric returns a value of std::tuple<unsigned int, unsigned int, unsigned int> type, where:

* First value is bottom bound.

* Second value is upper bound.

* Third value is step inside this range. String value for metric name is "RANGE_FOR_ASYNC_INFER_REQUESTS".

.. _doxid-namespace_inference_engine_1_1_metrics_1a4cc6b8c1b548fad1e03ea2a897b15400:
.. index:: pair: variable; METRIC_NUMBER_OF_WAITING_INFER_REQUESTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_NUMBER_OF_WAITING_INFER_REQUESTS =  "NUMBER_OF_WAITING_INFER_REQUESTS"

Metric to get an unsigned int value of number of waiting infer request.

String value is "NUMBER_OF_WAITNING_INFER_REQUESTS". This can be used as an executable network metric as well

.. _doxid-namespace_inference_engine_1_1_metrics_1a8bb4bb50ecf459e83f2dec54e5506e0b:
.. index:: pair: variable; METRIC_NUMBER_OF_EXEC_INFER_REQUESTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_NUMBER_OF_EXEC_INFER_REQUESTS =  "NUMBER_OF_EXEC_INFER_REQUESTS"

Metric to get an unsigned int value of number of infer request in execution stage.

String value is "NUMBER_OF_EXEC_INFER_REQUESTS". This can be used as an executable network metric as well

.. _doxid-namespace_inference_engine_1_1_metrics_1a8869591f9fc938a5caf68d05109ab348:
.. index:: pair: variable; METRIC_DEVICE_ARCHITECTURE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_DEVICE_ARCHITECTURE =  "DEVICE_ARCHITECTURE"

Metric which defines the device architecture.

.. _doxid-namespace_inference_engine_1_1_metrics_1af5394d85cc2ede6485a65b1707e5b262:
.. index:: pair: variable; METRIC_DEVICE_TYPE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_DEVICE_TYPE =  "DEVICE_TYPE"

Metric to get a type of device. See DeviceType enum definition for possible return values.

.. _doxid-namespace_inference_engine_1_1_metrics_1a6a0aefa372f436611dea9b92cd768ff1:
.. index:: pair: variable; METRIC_DEVICE_GOPS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_DEVICE_GOPS =  "DEVICE_GOPS"

Metric which defines Giga OPS per second count (GFLOPS or GIOPS) for a set of precisions supported by specified device.

.. _doxid-namespace_inference_engine_1_1_metrics_1a8ca1a5188eba1ec5ad73f951f0949381:
.. index:: pair: variable; METRIC_IMPORT_EXPORT_SUPPORT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_IMPORT_EXPORT_SUPPORT =  "IMPORT_EXPORT_SUPPORT"

Metric which defines support of import/export functionality by plugin.

.. _doxid-namespace_inference_engine_1_1_metrics_1ac8a47d4063517a77764b632962d4cc8d:
.. index:: pair: variable; METRIC_NETWORK_NAME

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_NETWORK_NAME =  "NETWORK_NAME"

Metric to get a name of network. String value is "NETWORK_NAME".

.. _doxid-namespace_inference_engine_1_1_metrics_1a2f746c0fabfb75a6fced6cf394cb9b2e:
.. index:: pair: variable; METRIC_DEVICE_THERMAL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_DEVICE_THERMAL =  "DEVICE_THERMAL"

Metric to get a float of device thermal. String value is "DEVICE_THERMAL".

.. _doxid-namespace_inference_engine_1_1_metrics_1a57a821fbccfb015f161e00b805415a58:
.. index:: pair: variable; METRIC_OPTIMAL_NUMBER_OF_INFER_REQUESTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto METRIC_OPTIMAL_NUMBER_OF_INFER_REQUESTS =  "OPTIMAL_NUMBER_OF_INFER_REQUESTS"

Metric to get an unsigned integer value of optimal number of executable network infer requests.

