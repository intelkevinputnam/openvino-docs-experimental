.. index:: pair: class; ov::pass::VisualizeTree
.. _doxid-classov_1_1pass_1_1_visualize_tree:

class ov::pass::VisualizeTree
=============================



:ref:`VisualizeTree <doxid-classov_1_1pass_1_1_visualize_tree>` pass allows to serialize :ref:`ov::Model <doxid-classov_1_1_model>` to xDot format.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <visualize_tree.hpp>
	
	class VisualizeTree: public :ref:`ov::pass::ModelPass<doxid-classov_1_1pass_1_1_model_pass>`
	{
	public:
		// typedefs
	
		typedef std::function<void(const :ref:`Node<doxid-classov_1_1_node>`&node, std::vector<std::string>&attributes)> :target:`node_modifiers_t<doxid-classov_1_1pass_1_1_visualize_tree_1a30caca7ac09732c2b0572ec40fce0cdd>`;

		// construction
	
		:target:`VisualizeTree<doxid-classov_1_1pass_1_1_visualize_tree_1a46d12e924694f30117a5ffd7f0598474>`(
			const std::string& file_name,
			:ref:`node_modifiers_t<doxid-classov_1_1pass_1_1_visualize_tree_1a30caca7ac09732c2b0572ec40fce0cdd>` nm = nullptr,
			bool dot_only = false
			);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_visualize_tree_1a08c936535bdc6cf6d826d4054d50591f>`("ov::pass::VisualizeTree");
		virtual bool :target:`run_on_model<doxid-classov_1_1pass_1_1_visualize_tree_1ad53ea316a7165b4dc3c9df43fa4e6437>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>&);
		void :target:`set_ops_to_details<doxid-classov_1_1pass_1_1_visualize_tree_1a382cde3a19e0868e2a4aa905fb056089>`(const :ref:`visualize_tree_ops_map_t<doxid-openvino_2pass_2visualize__tree_8hpp_1a2b6f709a98f49287ebb440f9b88ce8e7>`& ops_map);
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


