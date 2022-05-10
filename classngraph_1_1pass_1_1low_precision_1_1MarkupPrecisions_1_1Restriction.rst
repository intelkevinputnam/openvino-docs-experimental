.. index:: pair: class; ngraph::pass::low_precision::MarkupPrecisions::Restriction
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions_1_1_restriction:

class ngraph::pass::low_precision::MarkupPrecisions::Restriction
================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <markup_precisions.hpp>
	
	class Restriction
	{
	public:
		// fields
	
		bool :target:`versionIsRequired<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions_1_1_restriction_1acbba08c1e6470eafae3b643cd8ac21c2>`;
		std::unordered_map<uint64_t, std::vector<std::pair<size_t, std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>>>> :target:`precisionsByVersion<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions_1_1_restriction_1aab271165345632aab24d8130ba62cfa7>`;

		// construction
	
		:target:`Restriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions_1_1_restriction_1a67ff7cab4089dd1b5c56d07112fd0670>`(const bool versionIsRequired);

		// methods
	
		void :target:`add<doxid-classngraph_1_1pass_1_1low__precision_1_1_markup_precisions_1_1_restriction_1a8a487272b2b62cc4fe10eda9d1a19e19>`(
			const uint64_t version,
			const std::vector<std::pair<size_t, std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>>>& precisions
			);
	};

