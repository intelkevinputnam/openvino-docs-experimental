.. index:: pair: class; ngraph::pass::low_precision::LayerTransformation::PrecisionDetails
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details:

class ngraph::pass::low_precision::LayerTransformation::PrecisionDetails
========================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layer_transformation.hpp>
	
	class PrecisionDetails
	{
	public:
		// fields
	
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :ref:`precision<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details_1a57119849ff6dcedd17aeb3fcc7a6bf8c>`;
		bool :ref:`hasNegativeOutput<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details_1a23aff6ac43fbefffb6de47f395edecf9>`;
		bool :ref:`hasZeroPoint<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details_1a8566acdfa96aa3bbda2dfac879bd3195>`;

		// construction
	
		:ref:`PrecisionDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details_1a521a6529e0fbac88276713249568fbcf>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& precision,
			const bool hasNegativeOutput,
			const bool hasZeroPoint
			);
	};

