.. index:: pair: namespace; ov::intel_gpu::hint
.. _doxid-namespaceov_1_1intel__gpu_1_1hint:

namespace ov::intel_gpu::hint
=============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace hint {

	// typedefs

	typedef :ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>` :ref:`ThrottleLevel<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gabeb80bf9522a2518878afb54e3fd2204>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ThrottleLevel<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`queue_throttle<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gace6031a0761c1917aa84135fe2163d56>` {"GPU_QUEUE_THROTTLE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`queue_priority<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga41a9b0bfa860966128952ebfcca324b9>` {"GPU_QUEUE_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ov::hint::Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`host_task_priority<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1ga1650ac020ec6e9ea8d03f898ef454e43>` {"GPU_HOST_TASK_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int64_t> :ref:`available_device_mem<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api_1gaa8a412c241cdb43c392422b6a2b40c15>` {"AVAILABLE_DEVICE_MEM_SIZE"};

	} // namespace hint
