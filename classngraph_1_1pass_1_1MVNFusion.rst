.. index:: pair: class; ngraph::pass::MVNFusion
.. _doxid-classngraph_1_1pass_1_1_m_v_n_fusion:

class ngraph::pass::MVNFusion
=============================



:ref:`MVNFusion <doxid-classngraph_1_1pass_1_1_m_v_n_fusion>` transformation replaces various sub-graphs with a MVN op.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <mvn_fusion.hpp>
	
	class MVNFusion: public :ref:`ov::pass::GraphRewrite<doxid-classov_1_1pass_1_1_graph_rewrite>`
	{
	public:
		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1pass_1_1_m_v_n_fusion_1af57873c2d54e6c7ef45bffa30994c67a>`("MVNFusion", "0");
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
		:ref:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_graph_rewrite_1a90ee0a4c5a161722d738ab1971545167>`("ov::pass::GraphRewrite");
	
		template <
			typename T,
			bool Enabled = true,
			class... Args,
			typename std::enable_if<std::is_base_of<pass::MatcherPass, T>::value, bool>::type = true
			>
		std::shared_ptr<T> :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac>`(Args&&... args);
	
		template <
			typename T,
			class... Args,
			typename std::enable_if<std::is_base_of<pass::GraphRewrite, T>::value, bool>::type = true
			>
		void :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1a826f4e2d1dfbf1a9905b97c5346010a6>`(Args&&... args);
	
		std::shared_ptr<:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`> :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1aa50614ed692bf256413fd8e7928871eb>`(const std::shared_ptr<:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`>& pass);
	
		void :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1af00561a5f69ca8657dde0dc550d67aa1>`(
			const std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`>& m,
			const :ref:`graph_rewrite_callback<doxid-namespaceov_1a5fe08faf69e9897c58d168a54359047e>`& callback,
			const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& property
			);
	
		void :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1a1f1275df9bdc023c902114d3d2f1aa1c>`(
			const std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`>& m,
			const :ref:`ov::graph_rewrite_callback<doxid-namespaceov_1a5fe08faf69e9897c58d168a54359047e>`& callback
			);
	
		virtual bool :ref:`run_on_model<doxid-classov_1_1pass_1_1_graph_rewrite_1ad27ed8542330330ce9a524ff17564c21>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_graph_rewrite_1a97d000b54a0073754ca1dbc4516acbf2>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);


