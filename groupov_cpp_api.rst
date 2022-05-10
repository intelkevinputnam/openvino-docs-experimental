.. index:: pair: group; OpenVINO Runtime C++ API
.. _doxid-group__ov__cpp__api:

OpenVINO Runtime C++ API
========================

.. toctree::
	:hidden:

	groupov_model_cpp_api.rst
	groupov_runtime_cpp_api.rst
	groupov_opset_cpp_api.rst
	groupov_ops_cpp_api.rst
	groupov_pass_cpp_api.rst
	ov <namespaceov.rst>

OpenVINO Runtime C++ API

|	:ref:`Basics<doxid-group__ov__model__cpp__api>`
|		:ref:`Element types<doxid-group__ov__element__cpp__api>`
|		:ref:`Layout<doxid-group__ov__layout__cpp__api>`
|	:ref:`Inference<doxid-group__ov__runtime__cpp__api>`
|		:ref:`Device properties<doxid-group__ov__runtime__cpp__prop__api>`
|		:ref:`Intel GNA specific properties<doxid-group__ov__runtime__gna__prop__cpp__api>`
|		:ref:`Intel GPU OpenCL interoperability<doxid-group__ov__runtime__ocl__gpu__cpp__api>`
|		:ref:`Intel GPU OpenCL specific properties<doxid-group__ov__runtime__ocl__gpu__prop__cpp__api>`
|		:ref:`Intel HDDL specific properties<doxid-group__ov__runtime__hddl__prop__cpp__api>`
|		:ref:`Intel MYRIAD & HDDL specific properties<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api>`
|		:ref:`Intel MYRIAD specific properties<doxid-group__ov__runtime__myriad__prop__cpp__api>`
|	:ref:`Operation sets<doxid-group__ov__opset__cpp__api>`
|	:ref:`Operations<doxid-group__ov__ops__cpp__api>`
|	:ref:`Transformation passes<doxid-group__ov__pass__cpp__api>`



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`ov<doxid-namespaceov>`;
		namespace :ref:`ov::batch_util<doxid-namespaceov_1_1batch__util>`;
		namespace :ref:`ov::descriptor<doxid-namespaceov_1_1descriptor>`;
		namespace :ref:`ov::detail<doxid-namespaceov_1_1detail>`;
		namespace :ref:`ov::device<doxid-namespaceov_1_1device>`;
			namespace :ref:`ov::device::capability<doxid-namespaceov_1_1device_1_1capability>`;
		namespace :ref:`ov::element<doxid-namespaceov_1_1element>`;
		namespace :ref:`ov::frontend<doxid-namespaceov_1_1frontend>`;
		namespace :ref:`ov::hint<doxid-namespaceov_1_1hint>`;
		namespace :ref:`ov::intel_gna<doxid-namespaceov_1_1intel__gna>`;
		namespace :ref:`ov::intel_gpu<doxid-namespaceov_1_1intel__gpu>`;
			namespace :ref:`ov::intel_gpu::capability<doxid-namespaceov_1_1intel__gpu_1_1capability>`;
			namespace :ref:`ov::intel_gpu::hint<doxid-namespaceov_1_1intel__gpu_1_1hint>`;
			namespace :ref:`ov::intel_gpu::memory_type<doxid-namespaceov_1_1intel__gpu_1_1memory__type>`;
			namespace :ref:`ov::intel_gpu::ocl<doxid-namespaceov_1_1intel__gpu_1_1ocl>`;
		namespace :ref:`ov::intel_myriad<doxid-namespaceov_1_1intel__myriad>`;
			namespace :ref:`ov::intel_myriad::hddl<doxid-namespaceov_1_1intel__myriad_1_1hddl>`;
		namespace :ref:`ov::layout<doxid-namespaceov_1_1layout>`;
		namespace :ref:`ov::log<doxid-namespaceov_1_1log>`;
		namespace :ref:`ov::op<doxid-namespaceov_1_1op>`;
			namespace :ref:`ov::op::ShapeInferLSTM<doxid-namespaceov_1_1op_1_1_shape_infer_l_s_t_m>`;
			namespace :ref:`ov::op::ShapeInferRange<doxid-namespaceov_1_1op_1_1_shape_infer_range>`;
			namespace :ref:`ov::op::util<doxid-namespaceov_1_1op_1_1util>`;
				namespace :ref:`ov::op::util::detail<doxid-namespaceov_1_1op_1_1util_1_1detail>`;
				namespace :ref:`ov::op::util::error<doxid-namespaceov_1_1op_1_1util_1_1error>`;
				namespace :ref:`ov::op::util::rfft_common_validation<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation>`;
			namespace :ref:`ov::op::v0<doxid-namespaceov_1_1op_1_1v0>`;
			namespace :ref:`ov::op::v1<doxid-namespaceov_1_1op_1_1v1>`;
			namespace :ref:`ov::op::v3<doxid-namespaceov_1_1op_1_1v3>`;
			namespace :ref:`ov::op::v4<doxid-namespaceov_1_1op_1_1v4>`;
			namespace :ref:`ov::op::v5<doxid-namespaceov_1_1op_1_1v5>`;
			namespace :ref:`ov::op::v6<doxid-namespaceov_1_1op_1_1v6>`;
			namespace :ref:`ov::op::v7<doxid-namespaceov_1_1op_1_1v7>`;
			namespace :ref:`ov::op::v8<doxid-namespaceov_1_1op_1_1v8>`;
			namespace :ref:`ov::op::v9<doxid-namespaceov_1_1op_1_1v9>`;
		namespace :ref:`ov::opset1<doxid-namespaceov_1_1opset1>`;
		namespace :ref:`ov::opset2<doxid-namespaceov_1_1opset2>`;
		namespace :ref:`ov::opset3<doxid-namespaceov_1_1opset3>`;
		namespace :ref:`ov::opset4<doxid-namespaceov_1_1opset4>`;
		namespace :ref:`ov::opset5<doxid-namespaceov_1_1opset5>`;
		namespace :ref:`ov::opset6<doxid-namespaceov_1_1opset6>`;
		namespace :ref:`ov::opset7<doxid-namespaceov_1_1opset7>`;
		namespace :ref:`ov::opset8<doxid-namespaceov_1_1opset8>`;
		namespace :ref:`ov::opset9<doxid-namespaceov_1_1opset9>`;
		namespace :ref:`ov::pass<doxid-namespaceov_1_1pass>`;
			namespace :ref:`ov::pass::pattern<doxid-namespaceov_1_1pass_1_1pattern>`;
				namespace :ref:`ov::pass::pattern::op<doxid-namespaceov_1_1pass_1_1pattern_1_1op>`;
		namespace :ref:`ov::preprocess<doxid-namespaceov_1_1preprocess>`;
		namespace :ref:`ov::runtime<doxid-namespaceov_1_1runtime>`;
		namespace :ref:`ov::streams<doxid-namespaceov_1_1streams>`;
		namespace :ref:`ov::util<doxid-namespaceov_1_1util>`;

