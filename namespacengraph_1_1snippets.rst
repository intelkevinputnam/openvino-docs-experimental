.. index:: pair: namespace; ngraph::snippets
.. _doxid-namespacengraph_1_1snippets:

namespace ngraph::snippets
==========================

.. toctree::
	:hidden:

	isa <namespacengraph_1_1snippets_1_1isa.rst>
	op <namespacengraph_1_1snippets_1_1op.rst>
	pass <namespacengraph_1_1snippets_1_1pass.rst>
	Emitter <classngraph_1_1snippets_1_1Emitter.rst>
	Generator <classngraph_1_1snippets_1_1Generator.rst>
	Schedule <classngraph_1_1snippets_1_1Schedule.rst>
	TargetMachine <classngraph_1_1snippets_1_1TargetMachine.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace snippets {

	// namespaces

	namespace :ref:`ngraph::snippets::isa<doxid-namespacengraph_1_1snippets_1_1isa>`;
	namespace :ref:`ngraph::snippets::op<doxid-namespacengraph_1_1snippets_1_1op>`;
	namespace :ref:`ngraph::snippets::pass<doxid-namespacengraph_1_1snippets_1_1pass>`;

	// typedefs

	typedef const uint8_t \* :target:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>`;
	typedef std::pair<std::vector<size_t>, std::vector<size_t>> :target:`RegInfo<doxid-namespacengraph_1_1snippets_1a3d2700d6955f8b1f9e2fffa540cd5556>`;

	// templates

	template :ref:`Emitter<doxid-classngraph_1_1snippets_1_1_emitter>`;
	template :ref:`Generator<doxid-classngraph_1_1snippets_1_1_generator>`;
	template :ref:`Schedule<doxid-classngraph_1_1snippets_1_1_schedule>`;
	template :ref:`TargetMachine<doxid-classngraph_1_1snippets_1_1_target_machine>`;

	// global functions

	auto :target:`getRegisters<doxid-namespacengraph_1_1snippets_1ac759d890f5a0e93a4fddd446e23ba789>`(std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& n);

	} // namespace snippets
