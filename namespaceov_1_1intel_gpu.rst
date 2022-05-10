.. index:: pair: namespace; ov::intel_gpu
.. _doxid-namespaceov_1_1intel__gpu:

namespace ov::intel_gpu
=======================

.. toctree::
	:hidden:

	capability <namespaceov_1_1intel_gpu_1_1capability.rst>
	hint <namespaceov_1_1intel_gpu_1_1hint.rst>
	memory_type <namespaceov_1_1intel_gpu_1_1memory_type.rst>
	ocl <namespaceov_1_1intel_gpu_1_1ocl.rst>

Namespace with Intel GPU specific properties.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace intel_gpu {

	// namespaces

	namespace :ref:`ov::intel_gpu::capability<doxid-namespaceov_1_1intel__gpu_1_1capability>`;
	namespace :ref:`ov::intel_gpu::hint<doxid-namespaceov_1_1intel__gpu_1_1hint>`;
	namespace :ref:`ov::intel_gpu::memory_type<doxid-namespaceov_1_1intel__gpu_1_1memory__type>`;
	namespace :ref:`ov::intel_gpu::ocl<doxid-namespaceov_1_1intel__gpu_1_1ocl>`;

	// typedefs

	typedef void \* :target:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`;

	// enums

	enum :ref:`ContextType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b>`;
	enum :ref:`SharedMemType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint64_t, PropertyMutability::RO> :ref:`device_total_mem_size<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga4545149544127b7f82b5d673b8a5a017>` {"GPU_DEVICE_TOTAL_MEM_SIZE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`uarch_version<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga55179d37180f123686ab43b27ed3f2c9>` {"GPU_UARCH_VERSION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, PropertyMutability::RO> :ref:`execution_units_count<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga86642bacd4b0fa7f803c212e72318d79>` {"GPU_EXECUTION_UNITS_COUNT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<std::string, uint64_t>, PropertyMutability::RO> :ref:`memory_statistics<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga2364c38776f270d5b9560e745fd8ff80>` {     "GPU_MEMORY_STATISTICS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> :ref:`enable_loop_unrolling<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga2d18d0f9e29ddde42b95d523405ae322>` {"GPU_ENABLE_LOOP_UNROLLING"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ContextType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga3d30ef6bfc7628812b855ca2031ce01b>`> :ref:`context_type<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga79db7ddeadb921be11875f65aab4fa97>` {"CONTEXT_TYPE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ocl_context<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga603300e0890eacc6a72b653f922a9b17>` {"OCL_CONTEXT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int> :ref:`ocl_context_device_id<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gaaef948041b53eca18f873d90423028a4>` {"OCL_CONTEXT_DEVICE_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int> :ref:`tile_id<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga0809250f740b2d33b1c036a508b709dd>` {"TILE_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`ocl_queue<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga293347d96f2828219be99e2796d5a58d>` {"OCL_QUEUE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`va_device<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gaead16bba9c3e710a5bbc37a3d7ec131e>` {"VA_DEVICE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`SharedMemType<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga887d079a3a8ffaa6d75aeb28c0fb3491>`> :ref:`shared_mem_type<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gad1d680fdc8440d41b4106d6e0fbbf66d>` {"SHARED_MEM_TYPE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`mem_handle<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga802dc72abf97bd4fbad889b55ac659e8>` {"MEM_HANDLE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`gpu_handle_param<doxid-namespaceov_1_1intel__gpu_1a6fd96670f1afaae5f1bab2f3d3842e47>`> :ref:`dev_object_handle<doxid-group__ov__runtime__ocl__gpu__cpp__api_1ga821530fcff2dba9aaaab557cffaf7955>` {"DEV_OBJECT_HANDLE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint32_t> :ref:`va_plane<doxid-group__ov__runtime__ocl__gpu__cpp__api_1gab033a8e885c875bef228ad92a79d32fc>` {"VA_PLANE"};

	} // namespace intel_gpu
