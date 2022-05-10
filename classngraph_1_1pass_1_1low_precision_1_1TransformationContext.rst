.. index:: pair: class; ngraph::pass::low_precision::TransformationContext
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context:

class ngraph::pass::low_precision::TransformationContext
========================================================



:ref:`TransformationContext <doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context>` instance is used to pass model transformation context data between transformations.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <transformation_context.hpp>
	
	class TransformationContext
	{
	public:
		// fields
	
		std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :target:`function<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context_1ab0bd78e8f8566cc1de666c70474aa1fa>`;
		std::unordered_set<std::string> :target:`quantizedFakeQuantizeNames<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context_1a10340728aee084c7cad31587ac0560f5>`;

		// construction
	
		:target:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context_1a454d20a9d0593b3068340a8ab13af25b>`();
		:target:`TransformationContext<doxid-classngraph_1_1pass_1_1low__precision_1_1_transformation_context_1a04aab7b824736a52e532018d6b6a98b7>`(std::shared_ptr<:ref:`Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> function);
	};

