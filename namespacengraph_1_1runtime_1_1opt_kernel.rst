.. index:: pair: namespace; ngraph::runtime::opt_kernel
.. _doxid-namespacengraph_1_1runtime_1_1opt__kernel:

namespace ngraph::runtime::opt_kernel
=====================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace opt_kernel {

	// global functions

	void :target:`reshape<doxid-namespacengraph_1_1runtime_1_1opt__kernel_1a90b91edefb389a6af33840c78e6f0570>`(
		const char \* in,
		char \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& in_shape,
		const :ref:`AxisVector<doxid-classov_1_1_axis_vector>`& in_axis_order,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape,
		size_t elem_size
		);

	} // namespace opt_kernel
