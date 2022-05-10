.. index:: pair: class; ngraph::pass::low_precision::PropagateThroughPrecisionPreserved
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved:

class ngraph::pass::low_precision::PropagateThroughPrecisionPreserved
=====================================================================



Overview
~~~~~~~~

:ref:`PropagateThroughPrecisionPreserved <doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved>` transformation propagates AttributeType attribute instances through precision preserved operations. :ref:`More...<details-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <propagate_through_precision_preserved.hpp>
	
	template <typename AttributeType>
	class PropagateThroughPrecisionPreserved
	{
	public:
		// construction
	
		:target:`PropagateThroughPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved_1ab4e0c03531a801fa44b628d1c4ed816f>`(const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`);
	};
.. _details-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`PropagateThroughPrecisionPreserved <doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved>` transformation propagates AttributeType attribute instances through precision preserved operations.

For more details about the transformation, refer to :ref:`PropagateThroughPrecisionPreserved <doxid-openvino_docs__o_v__u_g_lpt__propagate_through_precision_preserved>` page in the Inference Engine Developer Guide.


