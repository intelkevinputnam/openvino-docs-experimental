.. index:: pair: namespace; ngraph::pass::low_precision::precision_set
.. _doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set:

namespace ngraph::pass::low_precision::precision_set
====================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace precision_set {

	// global variables

	const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`> :target:`int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>` = {             ngraph::element::u8,  ngraph::element::i8     };
	const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`> :target:`int8_int16_int32_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1a0e6ccb35db9d82372051aaf484cd1ec7>` = {             ngraph::element::u8,  ngraph::element::i8,             ngraph::element::u16, ngraph::element::i16,             ngraph::element::u32, ngraph::element::i32     };

	} // namespace precision_set
