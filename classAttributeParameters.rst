.. index:: pair: class; AttributeParameters
.. _doxid-class_attribute_parameters:

class AttributeParameters
=========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_parameters.hpp>
	
	class AttributeParameters
	{
	public:
		// fields
	
		:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` :target:`deqPrecision<doxid-class_attribute_parameters_1ae682c8bfc8c73dc563a0d8c851b658e0>`;
		std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`> :target:`defaultPrecisions<doxid-class_attribute_parameters_1a5b8d3cb6f032a344685b0b9f884205d0>`;

		// construction
	
		:target:`AttributeParameters<doxid-class_attribute_parameters_1aca8bb98089d59d635bb6b52b4405c379>`(
			const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` deqPrecision = ngraph::element::f32,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`> defaultPrecisions = { ngraph::element::u8, ngraph::element::i8 }
			);
	};

