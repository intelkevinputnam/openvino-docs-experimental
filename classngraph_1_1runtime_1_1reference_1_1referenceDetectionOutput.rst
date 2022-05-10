.. index:: pair: class; ngraph::runtime::reference::referenceDetectionOutput
.. _doxid-classngraph_1_1runtime_1_1reference_1_1reference_detection_output:

class ngraph::runtime::reference::referenceDetectionOutput
==========================================================

.. toctree::
	:hidden:

	NormalizedBBox <structngraph_1_1runtime_1_1reference_1_1referenceDetectionOutput_1_1NormalizedBBox.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <detection_output.hpp>
	
	template <typename dataType>
	class referenceDetectionOutput
	{
	public:
		// structs
	
		struct :ref:`NormalizedBBox<doxid-structngraph_1_1runtime_1_1reference_1_1reference_detection_output_1_1_normalized_b_box>`;

		// construction
	
		:target:`referenceDetectionOutput<doxid-classngraph_1_1runtime_1_1reference_1_1reference_detection_output_1a11dfc902e676e21f37e850919d68821c>`(
			const :ref:`ngraph::op::DetectionOutputAttrs<doxid-namespacengraph_1_1op_1a6b495dc76d75ee3962694caf87698e9b>`& _attrs,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& locShape,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& priorsShape,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& outShape
			);
	
		:target:`referenceDetectionOutput<doxid-classngraph_1_1runtime_1_1reference_1_1reference_detection_output_1a6ab7f8c9d6a01ab215f57b5bcc4e72d7>`(
			const :ref:`ngraph::op::util::DetectionOutputBase::AttributesBase<doxid-structov_1_1op_1_1util_1_1_detection_output_base_1_1_attributes_base>`& _attrs,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& locShape,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& classPredShape,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& priorsShape,
			const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& outShape
			);

		// methods
	
		void :target:`run<doxid-classngraph_1_1runtime_1_1reference_1_1reference_detection_output_1a9e21d9b3722f1cf7a6f6d5a2e65e14b1>`(
			const dataType \* _location,
			const dataType \* _confidence,
			const dataType \* _priors,
			const dataType \* _armConfidence,
			const dataType \* _armLocation,
			dataType \* result
			);
	};

