.. index:: pair: class; ngraph::pass::low_precision::UpdateSharedPrecisionPreserved
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved:

class ngraph::pass::low_precision::UpdateSharedPrecisionPreserved
=================================================================



Overview
~~~~~~~~

:ref:`UpdateSharedPrecisionPreserved <doxid-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved>` transformation updates shared AttributeType attribute instance value to true for precision preserved operations if ExpectedAttributeType exist. :ref:`More...<details-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <update_shared_precision_preserved.hpp>
	
	template <
		typename AttributeType,
		typename ExpectedAttributeType = AttributeType
		>
	class UpdateSharedPrecisionPreserved
	{
	public:
		// construction
	
		:target:`UpdateSharedPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved_1a3195a48b6405472fcd2e062d686da703>`(const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`);
	};
.. _details-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`UpdateSharedPrecisionPreserved <doxid-classngraph_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved>` transformation updates shared AttributeType attribute instance value to true for precision preserved operations if ExpectedAttributeType exist.

For more details about the transformation, refer to :ref:`UpdateSharedPrecisionPreserved <doxid-openvino_docs__o_v__u_g_lpt__update_shared_precision_preserved>` page in the Inference Engine Developer Guide.


