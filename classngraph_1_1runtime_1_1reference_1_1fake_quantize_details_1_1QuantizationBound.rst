.. index:: pair: class; ngraph::runtime::reference::fake_quantize_details::QuantizationBound
.. _doxid-classngraph_1_1runtime_1_1reference_1_1fake__quantize__details_1_1_quantization_bound:

class ngraph::runtime::reference::fake_quantize_details::QuantizationBound
==========================================================================

.. toctree::
	:hidden:

	Bound <enumngraph_1_1runtime_1_1reference_1_1fake_quantize_details_1_1QuantizationBound_1_1Bound.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <fake_quantize.hpp>
	
	template <typename T>
	class QuantizationBound
	{
	public:
		// enums
	
		enum :ref:`Bound<doxid-classngraph_1_1runtime_1_1reference_1_1fake__quantize__details_1_1_quantization_bound_1a9c34490c3f994bcd62308c27b815818f>`;

		// construction
	
		:target:`QuantizationBound<doxid-classngraph_1_1runtime_1_1reference_1_1fake__quantize__details_1_1_quantization_bound_1a648315a50d40336efb2daba8da6fd922>`(
			const T \*const bound_data,
			const :ref:`Shape<doxid-classov_1_1_shape>`& bound_shape,
			const :ref:`Shape<doxid-classov_1_1_shape>`& arg_shape,
			const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& broadcast_spec
			);

		// methods
	
		T :target:`get_value<doxid-classngraph_1_1runtime_1_1reference_1_1fake__quantize__details_1_1_quantization_bound_1a1451115eccf77db4fb9d87ec9a1b3736>`(const std::vector<size_t>& current_dim, size_t idx) const;
	};

