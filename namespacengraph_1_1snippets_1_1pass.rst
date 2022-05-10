.. index:: pair: namespace; ngraph::snippets::pass
.. _doxid-namespacengraph_1_1snippets_1_1pass:

namespace ngraph::snippets::pass
================================

.. toctree::
	:hidden:

	SnippetsNodeType <enumngraph_1_1snippets_1_1pass_1_1SnippetsNodeType.rst>
	AssignRegisters <classngraph_1_1snippets_1_1pass_1_1AssignRegisters.rst>
	ConvertConstantsToScalars <classngraph_1_1snippets_1_1pass_1_1ConvertConstantsToScalars.rst>
	EnumerateNodes <classngraph_1_1snippets_1_1pass_1_1EnumerateNodes.rst>
	InsertLoad <classngraph_1_1snippets_1_1pass_1_1InsertLoad.rst>
	InsertMoveBroadcast <classngraph_1_1snippets_1_1pass_1_1InsertMoveBroadcast.rst>
	InsertStore <classngraph_1_1snippets_1_1pass_1_1InsertStore.rst>
	LoadMoveBroadcastToBroadcastLoad <classngraph_1_1snippets_1_1pass_1_1LoadMoveBroadcastToBroadcastLoad.rst>
	ReplaceLoadsWithScalarLoads <classngraph_1_1snippets_1_1pass_1_1ReplaceLoadsWithScalarLoads.rst>
	ReplaceStoresWithScalarStores <classngraph_1_1snippets_1_1pass_1_1ReplaceStoresWithScalarStores.rst>
	TokenizeSnippets <classngraph_1_1snippets_1_1pass_1_1TokenizeSnippets.rst>
	ConvertPowerToPowerStatic <classngraph_1_1snippets_1_1pass_1_1ConvertPowerToPowerStatic.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace pass {

	// enums

	enum :ref:`SnippetsNodeType<doxid-namespacengraph_1_1snippets_1_1pass_1ae01407bb5a9b9bf82566a1512fdbb332>`;

	// templates

	template :ref:`AssignRegisters<doxid-classngraph_1_1snippets_1_1pass_1_1_assign_registers>`;
	template :ref:`ConvertConstantsToScalars<doxid-classngraph_1_1snippets_1_1pass_1_1_convert_constants_to_scalars>`;
	template :ref:`EnumerateNodes<doxid-classngraph_1_1snippets_1_1pass_1_1_enumerate_nodes>`;
	template :ref:`InsertLoad<doxid-classngraph_1_1snippets_1_1pass_1_1_insert_load>`;
	template :ref:`InsertMoveBroadcast<doxid-classngraph_1_1snippets_1_1pass_1_1_insert_move_broadcast>`;
	template :ref:`InsertStore<doxid-classngraph_1_1snippets_1_1pass_1_1_insert_store>`;
	template :ref:`LoadMoveBroadcastToBroadcastLoad<doxid-classngraph_1_1snippets_1_1pass_1_1_load_move_broadcast_to_broadcast_load>`;
	template :ref:`ReplaceLoadsWithScalarLoads<doxid-classngraph_1_1snippets_1_1pass_1_1_replace_loads_with_scalar_loads>`;
	template :ref:`ReplaceStoresWithScalarStores<doxid-classngraph_1_1snippets_1_1pass_1_1_replace_stores_with_scalar_stores>`;
	template :ref:`TokenizeSnippets<doxid-classngraph_1_1snippets_1_1pass_1_1_tokenize_snippets>`;

	// classes

	class :ref:`ConvertPowerToPowerStatic<doxid-classngraph_1_1snippets_1_1pass_1_1_convert_power_to_power_static>`;

	// global functions

	void :target:`SetSnippetsNodeType<doxid-namespacengraph_1_1snippets_1_1pass_1a68a0d73b7c4a9fe00a59c4eef8889c7d>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>&, :ref:`SnippetsNodeType<doxid-namespacengraph_1_1snippets_1_1pass_1ae01407bb5a9b9bf82566a1512fdbb332>`);
	:ref:`SnippetsNodeType<doxid-namespacengraph_1_1snippets_1_1pass_1ae01407bb5a9b9bf82566a1512fdbb332>` :target:`GetSnippetsNodeType<doxid-namespacengraph_1_1snippets_1_1pass_1a6684a11a70c4f4b9198f6802a81a1e1e>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>&);
	void :target:`SetTopologicalOrder<doxid-namespacengraph_1_1snippets_1_1pass_1ab34835e6db048f622714a17dd53744aa>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>&, int64_t);
	int64_t :target:`GetTopologicalOrder<doxid-namespacengraph_1_1snippets_1_1pass_1ae55e4045b3c2c42bb8ff2ccf7ee63944>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>&);
	bool :target:`AppropriateForSubgraph<doxid-namespacengraph_1_1snippets_1_1pass_1ad6551aee7887919cba6a82c20ae9e998>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>&);

	} // namespace pass
