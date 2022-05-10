.. index:: pair: group; Device properties
.. _doxid-group__ov__runtime__cpp__prop__api:

Device properties
=================

.. toctree::
	:hidden:

	Affinity <enumov_1_1Affinity.rst>
	Level <enumov_1_1log_1_1Level.rst>
	PerformanceMode <enumov_1_1hint_1_1PerformanceMode.rst>
	Priority <enumov_1_1hint_1_1Priority.rst>
	Type <enumov_1_1device_1_1Type.rst>
	Num <structov_1_1streams_1_1Num.rst>
	Priorities <structov_1_1device_1_1Priorities.rst>
	Properties <structov_1_1device_1_1Properties.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// enums

	enum :ref:`ov::Affinity<doxid-group__ov__runtime__cpp__prop__api_1ga72b7c6cde7f94f07bc1519464c55e9c5>`;
	enum :ref:`ov::log::Level<doxid-group__ov__runtime__cpp__prop__api_1ga9868e1ed6b0286d17cdb0ab85b2cc66b>`;
	enum :ref:`ov::hint::PerformanceMode<doxid-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73>`;
	enum :ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`;
	enum :ref:`ov::device::Type<doxid-group__ov__runtime__cpp__prop__api_1ga3c08e596389a1a1266dfa52681acd314>`;

	// structs

	struct :ref:`ov::streams::Num<doxid-structov_1_1streams_1_1_num>`;
	struct :ref:`ov::device::Priorities<doxid-structov_1_1device_1_1_priorities>`;
	struct :ref:`ov::device::Properties<doxid-structov_1_1device_1_1_properties>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<:ref:`PropertyName<doxid-structov_1_1_property_name>`>, PropertyMutability::RO> :ref:`ov::supported_properties<doxid-group__ov__runtime__cpp__prop__api_1ga097f1274f26f3f4e1aa4fc3928748592>` {     "SUPPORTED_PROPERTIES"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`ov::available_devices<doxid-group__ov__runtime__cpp__prop__api_1gac4d3e86ef4fc43b1a80ec28c7be39ef1>` {"AVAILABLE_DEVICES"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`ov::model_name<doxid-group__ov__runtime__cpp__prop__api_1gab390fe044f10a2c787357b06619597b2>` {"NETWORK_NAME"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t, PropertyMutability::RO> :ref:`ov::optimal_number_of_infer_requests<doxid-group__ov__runtime__cpp__prop__api_1ga087c6da667f7c3d8374aec5f6cbba027>` {     "OPTIMAL_NUMBER_OF_INFER_REQUESTS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> :ref:`ov::enable_profiling<doxid-group__ov__runtime__cpp__prop__api_1gafc5bef2fc2b5cfb5a0709cfb04346438>` {"PERF_COUNT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> :ref:`ov::cache_dir<doxid-group__ov__runtime__cpp__prop__api_1ga3276fc4ed7cc7d0bbdcf0ae12063728d>` {"CACHE_DIR"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::tuple<unsigned int, unsigned int>, PropertyMutability::RO> :ref:`ov::range_for_streams<doxid-group__ov__runtime__cpp__prop__api_1ga8a5d84196f6873729167aa512c34a94a>` {     "RANGE_FOR_STREAMS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<unsigned int, PropertyMutability::RO> :ref:`ov::optimal_batch_size<doxid-group__ov__runtime__cpp__prop__api_1ga129bad2da2fc2a40a7d746d86fc9c68d>` {"OPTIMAL_BATCH_SIZE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t, PropertyMutability::RO> :ref:`ov::max_batch_size<doxid-group__ov__runtime__cpp__prop__api_1ga5dbd8ab0c8a177234cade9a54c96249c>` {"MAX_BATCH_SIZE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::auto_batch_timeout<doxid-group__ov__runtime__cpp__prop__api_1gadfe7b9f18bff5f4851528f7a50e31a93>` {"AUTO_BATCH_TIMEOUT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::tuple<unsigned int, unsigned int, unsigned int>, PropertyMutability::RO> :ref:`ov::range_for_async_infer_requests<doxid-group__ov__runtime__cpp__prop__api_1ga3549425153790834c212d905b8216196>` {"RANGE_FOR_ASYNC_INFER_REQUESTS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`streams::Num<doxid-structov_1_1streams_1_1_num>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::num_streams<doxid-group__ov__runtime__cpp__prop__api_1ga6c63a0223565f650475450fdb466bc0c>` {"NUM_STREAMS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::inference_num_threads<doxid-group__ov__runtime__cpp__prop__api_1gae73c9d9977901744090317e2afe09440>` {"INFERENCE_NUM_THREADS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::compilation_num_threads<doxid-group__ov__runtime__cpp__prop__api_1ga91555d2fad22aa802aa9d36698805755>` {"COMPILATION_NUM_THREADS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Affinity<doxid-group__ov__runtime__cpp__prop__api_1ga72b7c6cde7f94f07bc1519464c55e9c5>`> :ref:`ov::affinity<doxid-group__ov__runtime__cpp__prop__api_1ga9c99a177a56685a70875302c59541887>` {"AFFINITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> :ref:`ov::device::id<doxid-group__ov__runtime__cpp__prop__api_1ga433b8ea52e99c2b1fa8b26453485d75d>` {"DEVICE_ID"};
	static constexpr :ref:`Priorities<doxid-structov_1_1device_1_1_priorities>` :ref:`ov::device::priorities<doxid-group__ov__runtime__cpp__prop__api_1gae88af90a18871677f39739cb0ef0101e>` {"MULTI_DEVICE_PRIORITIES"};
	static constexpr :ref:`Properties<doxid-structov_1_1device_1_1_properties>` :ref:`ov::device::properties<doxid-group__ov__runtime__cpp__prop__api_1ga794d09f2bd8aad506508b2c53ef6a6fc>`;
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`ov::device::full_name<doxid-group__ov__runtime__cpp__prop__api_1gaabacd9ea113b966be7b53b1d70fd6f42>` {"FULL_DEVICE_NAME"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`ov::device::architecture<doxid-group__ov__runtime__cpp__prop__api_1gae2e72a4510ecf768ca196959b6c92fd4>` {"DEVICE_ARCHITECTURE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Type<doxid-group__ov__runtime__cpp__prop__api_1ga3c08e596389a1a1266dfa52681acd314>`, PropertyMutability::RO> :ref:`ov::device::type<doxid-group__ov__runtime__cpp__prop__api_1gaf9b20fd37487c1f525e68c6e0567f1f1>` {"DEVICE_TYPE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, float>, PropertyMutability::RO> :ref:`ov::device::gops<doxid-group__ov__runtime__cpp__prop__api_1gae233c458317f6ae508b887eb09308c4c>` {"DEVICE_GOPS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<float, PropertyMutability::RO> :ref:`ov::device::thermal<doxid-group__ov__runtime__cpp__prop__api_1ga821543ca749cd78a8ced9930e0fec466>` {"DEVICE_THERMAL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`ov::device::capabilities<doxid-group__ov__runtime__cpp__prop__api_1gadb13d62787fc4485733329f044987294>` {"OPTIMIZATION_CAPABILITIES"};
	static constexpr static const auto :ref:`ov::device::capability::FP32<doxid-group__ov__runtime__cpp__prop__api_1gac0c6536f1d5028d74b5437c4dd271b40>` = "FP32";
	static constexpr static const auto :ref:`ov::device::capability::BF16<doxid-group__ov__runtime__cpp__prop__api_1gaec464f8e50dc918435e2075958e08c22>` = "BF16";
	static constexpr static const auto :ref:`ov::device::capability::FP16<doxid-group__ov__runtime__cpp__prop__api_1gac34fe8227d97ab21b6590d24d242a9bf>` = "FP16";
	static constexpr static const auto :ref:`ov::device::capability::INT8<doxid-group__ov__runtime__cpp__prop__api_1ga5f530cce16a9328ed92264d345d3050d>` = "INT8";
	static constexpr static const auto :ref:`ov::device::capability::INT16<doxid-group__ov__runtime__cpp__prop__api_1gaf51dd5f7fc341ec72c4f5b8dbab9bfac>` = "INT16";
	static constexpr static const auto :ref:`ov::device::capability::BIN<doxid-group__ov__runtime__cpp__prop__api_1ga1813163301667f77c7711ff465501aa7>` = "BIN";
	static constexpr static const auto :ref:`ov::device::capability::WINOGRAD<doxid-group__ov__runtime__cpp__prop__api_1ga88814f8b1b9d305edef8e8f4bebb92c6>` = "WINOGRAD";
	static constexpr static const auto :ref:`ov::device::capability::EXPORT_IMPORT<doxid-group__ov__runtime__cpp__prop__api_1ga5fb520b3e5765fa4c2c747ab4732132c>` = "EXPORT_IMPORT";
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::hint::inference_precision<doxid-group__ov__runtime__cpp__prop__api_1gad605a888f3c9b7598ab55023fbf44240>` {"INFERENCE_PRECISION_HINT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`ov::hint::model_priority<doxid-group__ov__runtime__cpp__prop__api_1ga3663a3976ff7c4bdc3ccdb9ce44945ce>` {"MODEL_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`PerformanceMode<doxid-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73>`> :ref:`ov::hint::performance_mode<doxid-group__ov__runtime__cpp__prop__api_1ga2691fe27acc8aa1d1700ad40b6da3ba2>` {"PERFORMANCE_HINT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>> :ref:`ov::hint::model<doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` {"MODEL_PTR"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::hint::allow_auto_batching<doxid-group__ov__runtime__cpp__prop__api_1ga445a111e7219955c585eb418d2f4f80d>` {"ALLOW_AUTO_BATCHING"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Level<doxid-group__ov__runtime__cpp__prop__api_1ga9868e1ed6b0286d17cdb0ab85b2cc66b>`> :ref:`ov::log::level<doxid-group__ov__runtime__cpp__prop__api_1gab4f55acc0df42391be3e9356ca0be7f8>` {"LOG_LEVEL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Num<doxid-structov_1_1streams_1_1_num>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::streams::num<doxid-group__ov__runtime__cpp__prop__api_1gaeeef815df8212c810bfa11a3f0bd8300>` {"NUM_STREAMS"};
	static constexpr :ref:`Num<doxid-structov_1_1streams_1_1_num>` :ref:`ov::streams::AUTO<doxid-group__ov__runtime__cpp__prop__api_1gaddb29425af71fbb6ad3379c59342ff0e>` {-1};
	static constexpr :ref:`Num<doxid-structov_1_1streams_1_1_num>` :ref:`ov::streams::NUMA<doxid-group__ov__runtime__cpp__prop__api_1ga62ff8b4a46d136c181eee7654fb99bc8>` {-2};

.. _details-group__ov__runtime__cpp__prop__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Variables
----------------

.. _doxid-group__ov__runtime__cpp__prop__api_1ga097f1274f26f3f4e1aa4fc3928748592:
.. index:: pair: variable; supported_properties

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<:ref:`PropertyName<doxid-structov_1_1_property_name>`>, PropertyMutability::RO> ov::supported_properties {     "SUPPORTED_PROPERTIES"}

Read-only property to get a std::vector<PropertyName> of supported read-only properties. This can be used as a compiled model property as well.

.. _doxid-group__ov__runtime__cpp__prop__api_1gac4d3e86ef4fc43b1a80ec28c7be39ef1:
.. index:: pair: variable; available_devices

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> ov::available_devices {"AVAILABLE_DEVICES"}

Read-only property to get a std::vector<std::string> of available device IDs.

.. _doxid-group__ov__runtime__cpp__prop__api_1gab390fe044f10a2c787357b06619597b2:
.. index:: pair: variable; model_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> ov::model_name {"NETWORK_NAME"}

Read-only property to get a name of name of a model.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga087c6da667f7c3d8374aec5f6cbba027:
.. index:: pair: variable; optimal_number_of_infer_requests

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t, PropertyMutability::RO> ov::optimal_number_of_infer_requests {     "OPTIMAL_NUMBER_OF_INFER_REQUESTS"}

Read-only property to get an unsigned integer value of optimal number of compiled model infer requests.

.. _doxid-group__ov__runtime__cpp__prop__api_1gafc5bef2fc2b5cfb5a0709cfb04346438:
.. index:: pair: variable; enable_profiling

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> ov::enable_profiling {"PERF_COUNT"}

The name for setting performance counters option.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga3276fc4ed7cc7d0bbdcf0ae12063728d:
.. index:: pair: variable; cache_dir

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> ov::cache_dir {"CACHE_DIR"}

This property defines the directory which will be used to store any data cached by plugins.

The underlying cache structure is not defined and might differ between OpenVINO releases Cached data might be platform / device specific and might be invalid after OpenVINO version change If this property is not specified or value is empty string, then caching is disabled. The property might enable caching for the plugin using the following code:

.. ref-code-block:: cpp

	ie.set_property("GPU", ov::cache_dir("cache/")); // enables cache for GPU plugin

The following code enables caching of compiled network blobs for devices where import/export is supported

.. ref-code-block:: cpp

	ie.set_property(ov::cache_dir("cache/")); // enables models cache

.. _doxid-group__ov__runtime__cpp__prop__api_1ga8a5d84196f6873729167aa512c34a94a:
.. index:: pair: variable; range_for_streams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::tuple<unsigned int, unsigned int>, PropertyMutability::RO> ov::range_for_streams {     "RANGE_FOR_STREAMS"}

Read-only property to provide information about a range for streams on platforms where streams are supported.

:ref:`Property <doxid-classov_1_1_property>` returns a value of std::tuple<unsigned int, unsigned int> type, where:

* First value is bottom bound.

* Second value is upper bound.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga129bad2da2fc2a40a7d746d86fc9c68d:
.. index:: pair: variable; optimal_batch_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<unsigned int, PropertyMutability::RO> ov::optimal_batch_size {"OPTIMAL_BATCH_SIZE"}

Read-only property to query information optimal batch size for the given device and the network.

:ref:`Property <doxid-classov_1_1_property>` returns a value of unsigned int type, Returns optimal batch size for a given network on the given device. The returned value is aligned to power of 2. Also, :ref:`ov::hint::model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` is the required option for this metric since the optimal batch size depends on the model, so if the :ref:`ov::hint::model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` is not given, the result of the metric is always 1. For the GPU the metric is queried automatically whenever the OpenVINO performance hint for the throughput is used, so that the result (>1) governs the automatic batching (transparently to the application). The automatic batching can be disabled with ALLOW_AUTO_BATCHING set to NO

.. _doxid-group__ov__runtime__cpp__prop__api_1ga5dbd8ab0c8a177234cade9a54c96249c:
.. index:: pair: variable; max_batch_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t, PropertyMutability::RO> ov::max_batch_size {"MAX_BATCH_SIZE"}

Read-only property to get maximum batch size which does not cause performance degradation due to memory swap impact.

.. _doxid-group__ov__runtime__cpp__prop__api_1gadfe7b9f18bff5f4851528f7a50e31a93:
.. index:: pair: variable; auto_batch_timeout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::auto_batch_timeout {"AUTO_BATCH_TIMEOUT"}

Read-write property to set the timeout used to collect the inputs for the auto-batching impact.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga3549425153790834c212d905b8216196:
.. index:: pair: variable; range_for_async_infer_requests

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::tuple<unsigned int, unsigned int, unsigned int>, PropertyMutability::RO> ov::range_for_async_infer_requests {"RANGE_FOR_ASYNC_INFER_REQUESTS"}

Read-only property to provide a hint for a range for number of async infer requests. If device supports streams, the metric provides range for number of IRs per stream.

:ref:`Property <doxid-classov_1_1_property>` returns a value of std::tuple<unsigned int, unsigned int, unsigned int> type, where:

* First value is bottom bound.

* Second value is upper bound.

* Third value is step inside this range.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga6c63a0223565f650475450fdb466bc0c:
.. index:: pair: variable; num_streams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`streams::Num<doxid-structov_1_1streams_1_1_num>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::num_streams {"NUM_STREAMS"}

The number of executor logical partitions.

.. _doxid-group__ov__runtime__cpp__prop__api_1gae73c9d9977901744090317e2afe09440:
.. index:: pair: variable; inference_num_threads

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::inference_num_threads {"INFERENCE_NUM_THREADS"}

Maximum number of threads that can be used for inference tasks.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga91555d2fad22aa802aa9d36698805755:
.. index:: pair: variable; compilation_num_threads

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::compilation_num_threads {"COMPILATION_NUM_THREADS"}

Maximum number of threads that can be used for compilation tasks.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga9c99a177a56685a70875302c59541887:
.. index:: pair: variable; affinity

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Affinity<doxid-group__ov__runtime__cpp__prop__api_1ga72b7c6cde7f94f07bc1519464c55e9c5>`> ov::affinity {"AFFINITY"}

The name for setting CPU affinity per thread option.

The setting is ignored, if the OpenVINO compiled with OpenMP and any affinity-related OpenMP's environment variable is set (as affinity is configured explicitly)

.. _doxid-group__ov__runtime__cpp__prop__api_1ga433b8ea52e99c2b1fa8b26453485d75d:
.. index:: pair: variable; id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> ov::device::id {"DEVICE_ID"}

the property for setting of required device to execute on values: device id starts from "0" - first device, "1" - second device, etc

.. _doxid-group__ov__runtime__cpp__prop__api_1gae88af90a18871677f39739cb0ef0101e:
.. index:: pair: variable; priorities

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Priorities<doxid-structov_1_1device_1_1_priorities>` ov::device::priorities {"MULTI_DEVICE_PRIORITIES"}

Device :ref:`Priorities <doxid-structov_1_1device_1_1_priorities>` config option, with comma-separated devices listed in the desired priority.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga794d09f2bd8aad506508b2c53ef6a6fc:
.. index:: pair: variable; properties

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Properties<doxid-structov_1_1device_1_1_properties>` ov::device::properties

:ref:`Property <doxid-classov_1_1_property>` to pass set of property values to specified device

Usage Example:

.. ref-code-block:: cpp

	core.compile_model("HETERO"
	    ov::device::priorities("GPU", "CPU"),
	    ov::device::properties("CPU", ov::enable_profiling(true)),
	    ov::device::properties("GPU", ov::enable_profiling(false)));

.. _doxid-group__ov__runtime__cpp__prop__api_1gaabacd9ea113b966be7b53b1d70fd6f42:
.. index:: pair: variable; full_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> ov::device::full_name {"FULL_DEVICE_NAME"}

Read-only property to get a std::string value representing a full device name.

.. _doxid-group__ov__runtime__cpp__prop__api_1gae2e72a4510ecf768ca196959b6c92fd4:
.. index:: pair: variable; architecture

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> ov::device::architecture {"DEVICE_ARCHITECTURE"}

Read-only property which defines the device architecture.

.. _doxid-group__ov__runtime__cpp__prop__api_1gaf9b20fd37487c1f525e68c6e0567f1f1:
.. index:: pair: variable; type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Type<doxid-group__ov__runtime__cpp__prop__api_1ga3c08e596389a1a1266dfa52681acd314>`, PropertyMutability::RO> ov::device::type {"DEVICE_TYPE"}

Read-only property to get a type of device. See Type enum definition for possible return values.

.. _doxid-group__ov__runtime__cpp__prop__api_1gae233c458317f6ae508b887eb09308c4c:
.. index:: pair: variable; gops

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, float>, PropertyMutability::RO> ov::device::gops {"DEVICE_GOPS"}

Read-only property which defines Giga OPS per second count (GFLOPS or GIOPS) for a set of precisions supported by specified device.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga821543ca749cd78a8ced9930e0fec466:
.. index:: pair: variable; thermal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<float, PropertyMutability::RO> ov::device::thermal {"DEVICE_THERMAL"}

Read-only property to get a float of device thermal.

.. _doxid-group__ov__runtime__cpp__prop__api_1gadb13d62787fc4485733329f044987294:
.. index:: pair: variable; capabilities

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> ov::device::capabilities {"OPTIMIZATION_CAPABILITIES"}

Read-only property to get a std::vector<std::string> of capabilities options per device.

.. _doxid-group__ov__runtime__cpp__prop__api_1gac0c6536f1d5028d74b5437c4dd271b40:
.. index:: pair: variable; FP32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::FP32 = "FP32"

Device supports fp32 inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1gaec464f8e50dc918435e2075958e08c22:
.. index:: pair: variable; BF16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::BF16 = "BF16"

Device supports bf16 inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1gac34fe8227d97ab21b6590d24d242a9bf:
.. index:: pair: variable; FP16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::FP16 = "FP16"

Device supports fp16 inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga5f530cce16a9328ed92264d345d3050d:
.. index:: pair: variable; INT8

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::INT8 = "INT8"

Device supports int8 inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1gaf51dd5f7fc341ec72c4f5b8dbab9bfac:
.. index:: pair: variable; INT16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::INT16 = "INT16"

Device supports int16 inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga1813163301667f77c7711ff465501aa7:
.. index:: pair: variable; BIN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::BIN = "BIN"

Device supports binary inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga88814f8b1b9d305edef8e8f4bebb92c6:
.. index:: pair: variable; WINOGRAD

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::WINOGRAD = "WINOGRAD"

Device supports winograd optimization.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga5fb520b3e5765fa4c2c747ab4732132c:
.. index:: pair: variable; EXPORT_IMPORT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::device::capability::EXPORT_IMPORT = "EXPORT_IMPORT"

Device supports compiled model export and import.

.. _doxid-group__ov__runtime__cpp__prop__api_1gad605a888f3c9b7598ab55023fbf44240:
.. index:: pair: variable; inference_precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::hint::inference_precision {"INFERENCE_PRECISION_HINT"}

Hint for device to use specified precision for inference.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga3663a3976ff7c4bdc3ccdb9ce44945ce:
.. index:: pair: variable; model_priority

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> ov::hint::model_priority {"MODEL_PRIORITY"}

High-level OpenVINO model priority hint Defines what model should be provided with more performant bounded resource first.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga2691fe27acc8aa1d1700ad40b6da3ba2:
.. index:: pair: variable; performance_mode

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`PerformanceMode<doxid-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73>`> ov::hint::performance_mode {"PERFORMANCE_HINT"}

High-level OpenVINO Performance Hints unlike low-level properties that are individual (per-device), the hints are something that every device accepts and turns into device-specific settings.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad:
.. index:: pair: variable; model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>> ov::hint::model {"MODEL_PTR"}

This key identifies shared pointer to the :ref:`ov::Model <doxid-classov_1_1_model>`, required for some properties (:ref:`ov::max_batch_size <doxid-group__ov__runtime__cpp__prop__api_1ga5dbd8ab0c8a177234cade9a54c96249c>` and :ref:`ov::optimal_batch_size <doxid-group__ov__runtime__cpp__prop__api_1ga129bad2da2fc2a40a7d746d86fc9c68d>`)

.. _doxid-group__ov__runtime__cpp__prop__api_1ga445a111e7219955c585eb418d2f4f80d:
.. index:: pair: variable; allow_auto_batching

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::hint::allow_auto_batching {"ALLOW_AUTO_BATCHING"}

Special key for auto batching feature configuration. Enabled by default.

.. _doxid-group__ov__runtime__cpp__prop__api_1gab4f55acc0df42391be3e9356ca0be7f8:
.. index:: pair: variable; level

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Level<doxid-group__ov__runtime__cpp__prop__api_1ga9868e1ed6b0286d17cdb0ab85b2cc66b>`> ov::log::level {"LOG_LEVEL"}

the property for setting desirable log level.

.. _doxid-group__ov__runtime__cpp__prop__api_1gaeeef815df8212c810bfa11a3f0bd8300:
.. index:: pair: variable; num

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Num<doxid-structov_1_1streams_1_1_num>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::streams::num {"NUM_STREAMS"}

The number of executor logical partitions.

.. _doxid-group__ov__runtime__cpp__prop__api_1gaddb29425af71fbb6ad3379c59342ff0e:
.. index:: pair: variable; AUTO

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Num<doxid-structov_1_1streams_1_1_num>` ov::streams::AUTO {-1}

Creates bare minimum of streams to improve the performance.

.. _doxid-group__ov__runtime__cpp__prop__api_1ga62ff8b4a46d136c181eee7654fb99bc8:
.. index:: pair: variable; NUMA

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Num<doxid-structov_1_1streams_1_1_num>` ov::streams::NUMA {-2}

Creates as many streams as needed to accommodate NUMA and avoid associated penalties.

