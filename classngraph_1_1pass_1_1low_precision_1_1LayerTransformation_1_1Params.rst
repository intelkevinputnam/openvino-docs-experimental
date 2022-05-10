.. index:: pair: class; ngraph::pass::low_precision::LayerTransformation::Params
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params:

class ngraph::pass::low_precision::LayerTransformation::Params
==============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layer_transformation.hpp>
	
	class Params
	{
	public:
		// fields
	
		bool :ref:`updatePrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1a6b22ed4b52a8ef3cf3122f675743f1e1>`;
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :ref:`deqPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1a3331f01dbab0be618a0a6deedf22d94d>`;
		std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`> :ref:`defaultPrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1a77123752433b7bf1b660c688986982ed>`;
		bool :ref:`reshapeIgnorePerTensorQuantizationCheck<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1a419dac522f7d60648f7fe5932553bbcd>`;

		// construction
	
		:ref:`Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1a5e62ebc7f8053eda4f4895f2813383ee>`(
			const bool updatePrecisions = true,
			:ref:`element::Type<doxid-classov_1_1element_1_1_type>` deqPrecision = element::f32,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`> defaultPrecisions = { ngraph::element::u8, ngraph::element::i8 },
			const bool reshapeIgnorePerTensorQuantizationCheck = false
			);

		// methods
	
		Params& :ref:`setUpdatePrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1ae07982bea5394713acb5fc038aa53791>`(const bool updatePrecisions);
		Params& :ref:`setDeqPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1ae877dd859e63b2f5b2c69bbebf9c7708>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& deqPrecision);
		Params& :ref:`setDefaultPrecisions<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params_1afce28861175077be602533bdfc94539c>`(const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions);
	};

