.. index:: pair: class; ngraph::pass::low_precision::DataPrecision
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision:

class ngraph::pass::low_precision::DataPrecision
================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layer_transformation.hpp>
	
	class DataPrecision
	{
	public:
		// fields
	
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :target:`precision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a08431099526b544d6c1958265b89bf45>`;
		float :target:`min<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a0a8239f1624c08094ae99cda134857bd>`;
		float :target:`max<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1afdfd38cc8cc36407c4e8169d3cf824a0>`;
		bool :target:`hasZeroPoint<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1aa7c092bbc658f51201f09ae8acdf163a>`;

		// construction
	
		:target:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a7390d31ca5f076e5eb61b100a98de9a8>`();
		:target:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a01abc6cf31aff58fd824686043baef5e>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& precision);
	
		:target:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a1403a5cb36fd28574e443644112c6db7>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision,
			const float min,
			const float max,
			const bool hasZeroPoint
			);

		// methods
	
		bool :target:`empty<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a98bba2e73903c7a0c19fcc57a0465707>`() const;
		static bool :target:`isSupported<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a9109dec29465fe7ed01488815215987f>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& precision);
		static float :target:`getMinValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a7301411d5e19b92226ec2e1889db4be2>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision, const size_t levels);
		static float :target:`getMaxValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a1b67547a746c4cd0c9a5174322193fe3>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision, const size_t levels);
		static float :target:`getMaxValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a0809abfb8ff53457ef7f8c26eeb09fb5>`(const size_t maxLevelsForPrecision);
		static bool :target:`hasNegativeValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a14c58d5575068a3152e1dfff11a1776a>`(const std::vector<float>& values);
	
		static :ref:`element::Type<doxid-classov_1_1element_1_1_type>` :target:`getPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a0ec32f0589d2267e99f46f2a6f44b467>`(
			const std::vector<float>& outputLowValues,
			const std::vector<float>& outputHighValues
			);
	
		static :ref:`element::Type<doxid-classov_1_1element_1_1_type>` :target:`getPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision_1a019a9abf86b8817fbd30e1575d4c9f45>`(const size_t, const bool signedInterval);
	};

