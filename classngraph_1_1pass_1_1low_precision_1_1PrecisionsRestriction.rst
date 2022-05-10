.. index:: pair: class; ngraph::pass::low_precision::PrecisionsRestriction
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction:

class ngraph::pass::low_precision::PrecisionsRestriction
========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <precisions_restriction.hpp>
	
	class PrecisionsRestriction
	{
	public:
		// typedefs
	
		typedef std::vector<std::pair<size_t, std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>>> :target:`PrecisionsByPort<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a69e177ca8f1f5c74962c20d6b92c6608>`;

		// fields
	
		:ref:`ngraph::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>` :target:`operationType<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1ae132dac03ff88067bc760ea6e4246100>`;
		bool :target:`specifyVersion<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a82f0440d19b9f44161985e9aa871fabc>`;
		std::vector<std::pair<size_t, std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>>> :target:`precisionsByPort<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1af8d2c9e91389cda9584b9787b0dc0432>`;

		// construction
	
		:target:`PrecisionsRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1ac157bc8231581c592cf43f7c23de9d22>`();
	
		:target:`PrecisionsRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a5761d4c99131c8cd21fd2689da9951fc>`(
			const :ref:`ngraph::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>` operationType,
			const bool specifyVersion,
			const :ref:`PrecisionsByPort<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a69e177ca8f1f5c74962c20d6b92c6608>`& precisionsByPort
			);

		// methods
	
		template <typename T>
		static PrecisionsRestriction :target:`create<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a2c93c7f783b8f580d8c836d4139dbdb8>`(
			const :ref:`PrecisionsByPort<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a69e177ca8f1f5c74962c20d6b92c6608>`& precisionsByPort,
			const bool specifyVersion = false
			);
	
		template <typename T>
		static :ref:`PrecisionsByPort<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1a69e177ca8f1f5c74962c20d6b92c6608>` :target:`getPrecisionsByOperationType<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction_1ac5298ccb474a9236a8dbd1ac7a8e9905>`(std::vector<PrecisionsRestriction>& restrictions);
	};

