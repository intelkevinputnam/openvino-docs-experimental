.. index:: pair: namespace; ngraph::runtime
.. _doxid-namespacengraph_1_1runtime:

namespace ngraph::runtime
=========================

.. toctree::
	:hidden:

	opt_kernel <namespacengraph_1_1runtime_1_1opt_kernel.rst>
	reference <namespacengraph_1_1runtime_1_1reference.rst>
	AlignedBuffer <classngraph_1_1runtime_1_1AlignedBuffer.rst>
	HostTensor <classngraph_1_1runtime_1_1HostTensor.rst>
	SharedBuffer <classngraph_1_1runtime_1_1SharedBuffer.rst>
	Tensor <classngraph_1_1runtime_1_1Tensor.rst>

The objects used for executing the graph.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace runtime {

	// namespaces

	namespace :ref:`ngraph::runtime::opt_kernel<doxid-namespacengraph_1_1runtime_1_1opt__kernel>`;
	namespace :ref:`ngraph::runtime::reference<doxid-namespacengraph_1_1runtime_1_1reference>`;
		namespace :ref:`ngraph::runtime::reference::adaptive_pool<doxid-namespacengraph_1_1runtime_1_1reference_1_1adaptive__pool>`;
		namespace :ref:`ngraph::runtime::reference::detail<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail>`;
		namespace :ref:`ngraph::runtime::reference::details<doxid-namespacengraph_1_1runtime_1_1reference_1_1details>`;
		namespace :ref:`ngraph::runtime::reference::fake_quantize_details<doxid-namespacengraph_1_1runtime_1_1reference_1_1fake__quantize__details>`;
		namespace :ref:`ngraph::runtime::reference::fft_common<doxid-namespacengraph_1_1runtime_1_1reference_1_1fft__common>`;
		namespace :ref:`ngraph::runtime::reference::internal<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal>`;
		namespace :ref:`ngraph::runtime::reference::kernel<doxid-namespacengraph_1_1runtime_1_1reference_1_1kernel>`;
		namespace :ref:`ngraph::runtime::reference::nms_common<doxid-namespacengraph_1_1runtime_1_1reference_1_1nms__common>`;

	// classes

	class :ref:`AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer>`;
	class :ref:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`;
	template <typename T>
	class :ref:`SharedBuffer<doxid-classngraph_1_1runtime_1_1_shared_buffer>`;
	class :ref:`Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`;

	} // namespace runtime
