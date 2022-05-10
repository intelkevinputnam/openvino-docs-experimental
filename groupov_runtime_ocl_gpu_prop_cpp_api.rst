.. index:: pair: group; Intel GPU OpenCL specific properties
.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api:

Intel GPU OpenCL specific properties
====================================



Overview
~~~~~~~~

Set of Intel GPU OpenCL specific properties. :ref:`More...<details-group__ov__runtime__ocl__gpu__prop__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// typedefs

	typedef :ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>` :ref:`ov::intel_gpu::hint::ThrottleLevel<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gabeb80bf9522a2518878afb54e3fd2204>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint64_t, PropertyMutability::RO> :ref:`ov::intel_gpu::device_total_mem_size<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga4545149544127b7f82b5d673b8a5a017>` {"GPU_DEVICE_TOTAL_MEM_SIZE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`ov::intel_gpu::uarch_version<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga55179d37180f123686ab43b27ed3f2c9>` {"GPU_UARCH_VERSION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, PropertyMutability::RO> :ref:`ov::intel_gpu::execution_units_count<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga86642bacd4b0fa7f803c212e72318d79>` {"GPU_EXECUTION_UNITS_COUNT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<std::string, uint64_t>, PropertyMutability::RO> :ref:`ov::intel_gpu::memory_statistics<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga2364c38776f270d5b9560e745fd8ff80>` {     "GPU_MEMORY_STATISTICS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> :ref:`ov::intel_gpu::enable_loop_unrolling<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga2d18d0f9e29ddde42b95d523405ae322>` {"GPU_ENABLE_LOOP_UNROLLING"};
	static constexpr static const auto :ref:`ov::intel_gpu::capability::HW_MATMUL<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga25bd539a936391cc77b4217058c73c23>` = "GPU_HW_MATMUL";
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ThrottleLevel<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`ov::intel_gpu::hint::queue_throttle<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gace6031a0761c1917aa84135fe2163d56>` {"GPU_QUEUE_THROTTLE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`ov::intel_gpu::hint::queue_priority<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga41a9b0bfa860966128952ebfcca324b9>` {"GPU_QUEUE_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`ov::intel_gpu::hint::host_task_priority<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga1650ac020ec6e9ea8d03f898ef454e43>` {"GPU_HOST_TASK_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int64_t> :ref:`ov::intel_gpu::hint::available_device_mem<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gaa8a412c241cdb43c392422b6a2b40c15>` {"AVAILABLE_DEVICE_MEM_SIZE"};
	static constexpr auto :ref:`ov::intel_gpu::memory_type::surface<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gaec0856a3b996876371138961269b742d>` = "GPU_SURFACE";

.. _details-group__ov__runtime__ocl__gpu__prop__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of Intel GPU OpenCL specific properties.

Typedefs
--------

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gabeb80bf9522a2518878afb54e3fd2204:
.. index:: pair: typedef; ThrottleLevel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef :ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>` ov::intel_gpu::hint::ThrottleLevel

This enum represents the possible value of :ref:`ov::intel_gpu::hint::queue_throttle <doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gace6031a0761c1917aa84135fe2163d56>` property:

* LOW is used for CL_QUEUE_THROTTLE_LOW_KHR OpenCL throttle hint

* MEDIUM (DEFAULT) is used for CL_QUEUE_THROTTLE_MED_KHR OpenCL throttle hint

* HIGH is used for CL_QUEUE_THROTTLE_HIGH_KHR OpenCL throttle hint

Global Variables
----------------

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga4545149544127b7f82b5d673b8a5a017:
.. index:: pair: variable; device_total_mem_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<uint64_t, PropertyMutability::RO> ov::intel_gpu::device_total_mem_size {"GPU_DEVICE_TOTAL_MEM_SIZE"}

Read-only property which defines size of memory in bytes available for the device. For iGPU it returns host memory size, for dGPU - dedicated gpu memory size.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga55179d37180f123686ab43b27ed3f2c9:
.. index:: pair: variable; uarch_version

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> ov::intel_gpu::uarch_version {"GPU_UARCH_VERSION"}

Read-only property to get microarchitecture identifier in major.minor.revision format.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga86642bacd4b0fa7f803c212e72318d79:
.. index:: pair: variable; execution_units_count

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int32_t, PropertyMutability::RO> ov::intel_gpu::execution_units_count {"GPU_EXECUTION_UNITS_COUNT"}

Read-only property to get count of execution units for current GPU.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga2364c38776f270d5b9560e745fd8ff80:
.. index:: pair: variable; memory_statistics

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<std::string, uint64_t>, PropertyMutability::RO> ov::intel_gpu::memory_statistics {     "GPU_MEMORY_STATISTICS"}

Read-only property to get statistics of GPU memory allocated by engine for each allocation type It contains information about current memory usage.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga2d18d0f9e29ddde42b95d523405ae322:
.. index:: pair: variable; enable_loop_unrolling

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> ov::intel_gpu::enable_loop_unrolling {"GPU_ENABLE_LOOP_UNROLLING"}

Turning on this key enables to unroll recurrent layers such as TensorIterator or Loop with fixed iteration count. This key is turned on by default. Turning this key on will achieve better inference performance for loops with not too many iteration counts (less than 16, as a rule of thumb). Turning this key off will achieve better performance for both graph loading time and inference time with many iteration counts (greater than 16). Note that turning this key on will increase the graph loading time in proportion to the iteration counts. Thus, this key should be turned off if graph loading time is considered to be most important target to optimize.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga25bd539a936391cc77b4217058c73c23:
.. index:: pair: variable; HW_MATMUL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr static const auto ov::intel_gpu::capability::HW_MATMUL = "GPU_HW_MATMUL"

Device has hardware block for matrix multiplication.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gace6031a0761c1917aa84135fe2163d56:
.. index:: pair: variable; queue_throttle

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ThrottleLevel<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> ov::intel_gpu::hint::queue_throttle {"GPU_QUEUE_THROTTLE"}

This key instructs the GPU plugin to use OpenCL queue throttle hints as defined in `https://www.khronos.org/registry/OpenCL/specs/opencl-2.1-extensions.pdf <https://www.khronos.org/registry/OpenCL/specs/opencl-2.1-extensions.pdf>`__, chapter 9.19. This option should be used with :ref:`ov::intel_gpu::hint::ThrottleLevel <doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gabeb80bf9522a2518878afb54e3fd2204>` values.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga41a9b0bfa860966128952ebfcca324b9:
.. index:: pair: variable; queue_priority

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> ov::intel_gpu::hint::queue_priority {"GPU_QUEUE_PRIORITY"}

This key instructs the GPU plugin to use the OpenCL queue priority hint as defined in `https://www.khronos.org/registry/OpenCL/specs/opencl-2.1-extensions.pdf <https://www.khronos.org/registry/OpenCL/specs/opencl-2.1-extensions.pdf>`__. This option should be used with :ref:`ov::hint::Priority <doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>` :

* LOW is used for CL_QUEUE_PRIORITY_LOW_KHR OpenCL priority hint

* MEDIUM (DEFAULT) is used for CL_QUEUE_PRIORITY_MED_KHR OpenCL priority hint

* HIGH is used for CL_QUEUE_PRIORITY_HIGH_KHR OpenCL priority hint

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga1650ac020ec6e9ea8d03f898ef454e43:
.. index:: pair: variable; host_task_priority

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> ov::intel_gpu::hint::host_task_priority {"GPU_HOST_TASK_PRIORITY"}

This key instructs the GPU plugin which cpu core type of TBB affinity used in load network. This option has 3 types of levels: HIGH, LOW, and ANY. It is only affected on Hybrid CPUs.

* LOW - instructs the GPU Plugin to use LITTLE cores if they are available

* MEDIUM (DEFAULT) - instructs the GPU Plugin to use any available cores (BIG or LITTLE cores)

* HIGH - instructs the GPU Plugin to use BIG cores if they are available

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gaa8a412c241cdb43c392422b6a2b40c15:
.. index:: pair: variable; available_device_mem

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int64_t> ov::intel_gpu::hint::available_device_mem {"AVAILABLE_DEVICE_MEM_SIZE"}

This key identifies available device memory size in bytes.

.. _doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gaec0856a3b996876371138961269b742d:
.. index:: pair: variable; surface

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr auto ov::intel_gpu::memory_type::surface = "GPU_SURFACE"

Native video decoder surface.

