.. index:: pair: group; Inference
.. _doxid-group__ov__runtime__cpp__api:

Inference
=========

.. toctree::
	:hidden:

	groupov_runtime_cpp_prop_api.rst
	groupov_runtime_gna_prop_cpp_api.rst
	groupov_runtime_ocl_gpu_cpp_api.rst
	groupov_runtime_ocl_gpu_prop_cpp_api.rst
	groupov_runtime_hddl_prop_cpp_api.rst
	groupov_runtime_myriad_hddl_prop_cpp_api.rst
	groupov_runtime_myriad_prop_cpp_api.rst
	ProfilingInfo <structov_1_1ProfilingInfo.rst>
	Allocator <classov_1_1Allocator.rst>
	Busy <classov_1_1Busy.rst>
	Cancelled <classov_1_1Cancelled.rst>
	CompiledModel <classov_1_1CompiledModel.rst>
	Core <classov_1_1Core.rst>
	InferRequest <classov_1_1InferRequest.rst>
	RemoteContext <classov_1_1RemoteContext.rst>
	RemoteTensor <classov_1_1RemoteTensor.rst>
	Tensor <classov_1_1Tensor.rst>
	VariableState <classov_1_1VariableState.rst>

Overview
~~~~~~~~

OpenVINO Inference C++ API provides :ref:`ov::Core <doxid-classov_1_1_core>`, :ref:`ov::CompiledModel <doxid-classov_1_1_compiled_model>`, :ref:`ov::InferRequest <doxid-classov_1_1_infer_request>` and :ref:`ov::Tensor <doxid-classov_1_1_tensor>` classes :ref:`More...<details-group__ov__runtime__cpp__api>`

|	:ref:`Device properties<doxid-group__ov__runtime__cpp__prop__api>`
|	:ref:`Intel GNA specific properties<doxid-group__ov__runtime__gna__prop__cpp__api>`
|	:ref:`Intel GPU OpenCL interoperability<doxid-group__ov__runtime__ocl__gpu__cpp__api>`
|	:ref:`Intel GPU OpenCL specific properties<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api>`
|	:ref:`Intel HDDL specific properties<doxid-group__ov__runtime__hddl__prop__cpp__api>`
|	:ref:`Intel MYRIAD & HDDL specific properties<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api>`
|	:ref:`Intel MYRIAD specific properties<doxid-group__ov__runtime__myriad__prop__cpp__api>`



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// typedefs

	typedef std::map<std::string, std::string> :ref:`ov::SupportedOpsMap<doxid-group__ov__runtime__cpp__api_1gae52f095f7ed180ae11f2a8bca5dfc16b>`;

	// structs

	struct :ref:`ov::ProfilingInfo<doxid-structov_1_1_profiling_info>`;

	// classes

	class :ref:`ov::Allocator<doxid-classov_1_1_allocator>`;
	class :ref:`ov::Busy<doxid-classov_1_1_busy>`;
	class :ref:`ov::Cancelled<doxid-classov_1_1_cancelled>`;
	class :ref:`ov::CompiledModel<doxid-classov_1_1_compiled_model>`;
	class :ref:`ov::Core<doxid-classov_1_1_core>`;
	class :ref:`ov::InferRequest<doxid-classov_1_1_infer_request>`;
	class :ref:`ov::RemoteContext<doxid-classov_1_1_remote_context>`;
	class :ref:`ov::RemoteTensor<doxid-classov_1_1_remote_tensor>`;
	class :ref:`ov::Tensor<doxid-classov_1_1_tensor>`;
	class :ref:`ov::VariableState<doxid-classov_1_1_variable_state>`;

.. _details-group__ov__runtime__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

OpenVINO Inference C++ API provides :ref:`ov::Core <doxid-classov_1_1_core>`, :ref:`ov::CompiledModel <doxid-classov_1_1_compiled_model>`, :ref:`ov::InferRequest <doxid-classov_1_1_infer_request>` and :ref:`ov::Tensor <doxid-classov_1_1_tensor>` classes

Typedefs
--------

.. _doxid-group__ov__runtime__cpp__api_1gae52f095f7ed180ae11f2a8bca5dfc16b:
.. index:: pair: typedef; SupportedOpsMap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::map<std::string, std::string> ov::SupportedOpsMap

This type of map is used for result of :ref:`Core::query_model <doxid-classov_1_1_core_1acdf8e64824fe4cf147c3b52ab32c1aab>`.

* ``key`` means operation name

* ``value`` means device name supporting this operation

