.. index:: pair: class; ngraph::pass::low_precision::LowPrecision
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision:

class ngraph::pass::low_precision::LowPrecision
===============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <low_precision.hpp>
	
	class LowPrecision: public :ref:`ov::pass::ModelPass<doxid-classov_1_1pass_1_1_model_pass>`
	{
	public:
		// construction
	
		:target:`LowPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision_1a07263a982e74f2d7c1f0e72a9a124c81>`(
			const std::vector<:ref:`PrecisionsRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_precisions_restriction>`>& precisionRestrictions = {},
			const std::vector<:ref:`QuantizationGranularityRestriction<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_granularity_restriction>`>& quantizationRestrictions = {},
			const :ref:`LayerTransformation::Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>` = :ref:`LayerTransformation::Params<doxid-classngraph_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params>`()
			);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision_1aa90f2aee84487ac835a9db715df88b9b>`("LowPrecision", "0");
		bool :target:`run_on_model<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision_1ae160ad1b8af9ae04bb79ec76673d9b94>`(const std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& m);
		static bool :target:`isFunctionQuantized<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision_1a067d6e01e3585f860bff01118399328c>`(const std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& function);
	
		static bool :target:`isFQLevelsPresent<doxid-classngraph_1_1pass_1_1low__precision_1_1_low_precision_1ac5a2376bc301faf1cf793a855ad22e81>`(
			const std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& function,
			const std::set<size_t>& levels
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`;

		// methods
	
		bool :ref:`get_property<doxid-classov_1_1pass_1_1_pass_base_1a3107964f6c4d4bf1d3fbc2bf97ccc0b8>`(const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& prop_mask) const;
		void :ref:`set_name<doxid-classov_1_1pass_1_1_pass_base_1a78ddde2a8770041d2f23ce59af908f5d>`(const std::string& name);
		std::string :ref:`get_name<doxid-classov_1_1pass_1_1_pass_base_1a6cd527d2176f1350dd999dc4632a576b>`() const;
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_base_1a6a56827a1cf76be99289bab703982869>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_pass_base_1abe74bba4b563ad367f2fdc7836016391>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);
		std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> :ref:`get_pass_config<doxid-classov_1_1pass_1_1_pass_base_1a4902f6ed9322e0fd38810d701f4409df>`();
		bool :ref:`m_transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1a568e5b1f0e01f221d36dffabbf156b3d>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		bool :ref:`transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		virtual const :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`& :ref:`get_type_info<doxid-classov_1_1pass_1_1_pass_base_1ab7020db2fcebc9b6e0741a451778fb0c>`() const = 0;
		:ref:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_model_pass_1a718f43e809339887547f5c96b84ea00a>`("ov::pass::ModelPass");
		virtual bool :ref:`run_on_function<doxid-classov_1_1pass_1_1_model_pass_1a58cf259fa3f2d8b565e6929832656aa9>`(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> m);
		virtual bool :ref:`run_on_model<doxid-classov_1_1pass_1_1_model_pass_1afdce6ef577b36b5127115dd574b6615e>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);


