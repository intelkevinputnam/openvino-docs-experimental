.. index:: pair: class; ngraph::pass::low_precision::PropagateToInput
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input:

class ngraph::pass::low_precision::PropagateToInput
===================================================



Overview
~~~~~~~~

:ref:`PropagateToInput <doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input>` transformation propagates AttributeType shared value attribute instances from parent output ports to consumers input ports. :ref:`More...<details-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <propagate_to_input.hpp>
	
	template <typename AttributeType>
	class PropagateToInput
	{
	public:
		// construction
	
		:target:`PropagateToInput<doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input_1a3e3db4abf05c83f6dcaf68704e43ae69>`(const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = { ngraph::element::u8, ngraph::element::i8 });
	};
.. _details-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`PropagateToInput <doxid-classngraph_1_1pass_1_1low__precision_1_1_propagate_to_input>` transformation propagates AttributeType shared value attribute instances from parent output ports to consumers input ports.

For more details about the transformation, refer to :ref:`PropagateToInput <doxid-openvino_docs__o_v__u_g_lpt__propagate_to_input>` page in the Inference Engine Developer Guide.


