.. index:: pair: namespace; ngraph::snippets::op
.. _doxid-namespacengraph_1_1snippets_1_1op:

namespace ngraph::snippets::op
==============================

.. toctree::
	:hidden:

	BlockedLoad <classngraph_1_1snippets_1_1op_1_1BlockedLoad.rst>
	BlockedParameter <classngraph_1_1snippets_1_1op_1_1BlockedParameter.rst>
	BroadcastLoad <classngraph_1_1snippets_1_1op_1_1BroadcastLoad.rst>
	BroadcastMove <classngraph_1_1snippets_1_1op_1_1BroadcastMove.rst>
	Kernel <classngraph_1_1snippets_1_1op_1_1Kernel.rst>
	Load <classngraph_1_1snippets_1_1op_1_1Load.rst>
	Nop <classngraph_1_1snippets_1_1op_1_1Nop.rst>
	PowerStatic <classngraph_1_1snippets_1_1op_1_1PowerStatic.rst>
	Scalar <classngraph_1_1snippets_1_1op_1_1Scalar.rst>
	ScalarLoad <classngraph_1_1snippets_1_1op_1_1ScalarLoad.rst>
	ScalarStore <classngraph_1_1snippets_1_1op_1_1ScalarStore.rst>
	Subgraph <classngraph_1_1snippets_1_1op_1_1Subgraph.rst>
	Tile <classngraph_1_1snippets_1_1op_1_1Tile.rst>
	VectorLoad <classngraph_1_1snippets_1_1op_1_1VectorLoad.rst>
	VectorStore <classngraph_1_1snippets_1_1op_1_1VectorStore.rst>
	Store <classngraph_1_1snippets_1_1op_1_1Store.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace op {

	// templates

	template :ref:`BlockedLoad<doxid-classngraph_1_1snippets_1_1op_1_1_blocked_load>`;
	template :ref:`BlockedParameter<doxid-classngraph_1_1snippets_1_1op_1_1_blocked_parameter>`;
	template :ref:`BroadcastLoad<doxid-classngraph_1_1snippets_1_1op_1_1_broadcast_load>`;
	template :ref:`BroadcastMove<doxid-classngraph_1_1snippets_1_1op_1_1_broadcast_move>`;
	template :ref:`Kernel<doxid-classngraph_1_1snippets_1_1op_1_1_kernel>`;
	template :ref:`Load<doxid-classngraph_1_1snippets_1_1op_1_1_load>`;
	template :ref:`Nop<doxid-classngraph_1_1snippets_1_1op_1_1_nop>`;
	template :ref:`PowerStatic<doxid-classngraph_1_1snippets_1_1op_1_1_power_static>`;
	template :ref:`Scalar<doxid-classngraph_1_1snippets_1_1op_1_1_scalar>`;
	template :ref:`ScalarLoad<doxid-classngraph_1_1snippets_1_1op_1_1_scalar_load>`;
	template :ref:`ScalarStore<doxid-classngraph_1_1snippets_1_1op_1_1_scalar_store>`;
	template :ref:`Subgraph<doxid-classngraph_1_1snippets_1_1op_1_1_subgraph>`;
	template :ref:`Tile<doxid-classngraph_1_1snippets_1_1op_1_1_tile>`;
	template :ref:`VectorLoad<doxid-classngraph_1_1snippets_1_1op_1_1_vector_load>`;
	template :ref:`VectorStore<doxid-classngraph_1_1snippets_1_1op_1_1_vector_store>`;

	// classes

	class :ref:`Store<doxid-classngraph_1_1snippets_1_1op_1_1_store>`;

	// global functions

	static std::ostream& :target:`operator <<<doxid-namespacengraph_1_1snippets_1_1op_1a70d57cdfeda8a9d043afe807105b2891>` (
		std::ostream& os,
		const :ref:`op::Subgraph::BlockedShape<doxid-classngraph_1_1snippets_1_1op_1_1_subgraph_1a7e97415e53465bb9cc47301198a87bb3>`& blocked_shape
		);

	static auto :target:`is_scalar_constant<doxid-namespacengraph_1_1snippets_1_1op_1a991de741ece23e7dadc10d92418d023b>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& source_output_node);

	static auto :target:`create_body<doxid-namespacengraph_1_1snippets_1_1op_1a08a230131d779c6e2f65cd1b944ef789>`(
		std::string name,
		const :ref:`ngraph::ResultVector<doxid-classngraph_1aedfbc99202fbf343071141f5e0e26eff>`& results,
		const :ref:`ngraph::ParameterVector<doxid-classngraph_1a8288ec615d4e98f673d38597891c6e49>`& parameters
		);

	static auto :target:`build_subgraph<doxid-namespacengraph_1_1snippets_1_1op_1abd71282d01acd0e242566733b3d05548>`(
		const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
		const :ref:`ngraph::OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& inputs,
		const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& body,
		const std::string name = ""
		);

	} // namespace op
