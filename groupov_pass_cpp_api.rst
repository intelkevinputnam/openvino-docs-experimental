.. index:: pair: group; Transformation passes
.. _doxid-group__ov__pass__cpp__api:

Transformation passes
=====================

.. toctree::
	:hidden:

	ConstantFolding <classov_1_1pass_1_1ConstantFolding.rst>
	ConvertFP32ToFP16 <classov_1_1pass_1_1ConvertFP32ToFP16.rst>
	GraphRewrite <classov_1_1pass_1_1GraphRewrite.rst>
	LowLatency2 <classov_1_1pass_1_1LowLatency2.rst>
	MakeStateful <classov_1_1pass_1_1MakeStateful.rst>
	Manager <classov_1_1pass_1_1Manager.rst>
	MatcherPass <classov_1_1pass_1_1MatcherPass.rst>
	ModelPass <classov_1_1pass_1_1ModelPass.rst>
	PassBase <classov_1_1pass_1_1PassBase.rst>
	PassConfig <classov_1_1pass_1_1PassConfig.rst>
	Serialize <classov_1_1pass_1_1Serialize.rst>
	StreamSerialize <classov_1_1pass_1_1StreamSerialize.rst>
	Validate <classov_1_1pass_1_1Validate.rst>
	VisualizeTree <classov_1_1pass_1_1VisualizeTree.rst>

Overview
~~~~~~~~

OpenVINO C++ API to work with OpenVINO transformations :ref:`More...<details-group__ov__pass__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`ov::pass::ConstantFolding<doxid-classov_1_1pass_1_1_constant_folding>`;
	class :ref:`ov::pass::ConvertFP32ToFP16<doxid-classov_1_1pass_1_1_convert_f_p32_to_f_p16>`;
	class :ref:`ov::pass::GraphRewrite<doxid-classov_1_1pass_1_1_graph_rewrite>`;
	class :ref:`ov::pass::LowLatency2<doxid-classov_1_1pass_1_1_low_latency2>`;
	class :ref:`ov::pass::MakeStateful<doxid-classov_1_1pass_1_1_make_stateful>`;
	class :ref:`ov::pass::Manager<doxid-classov_1_1pass_1_1_manager>`;
	class :ref:`ov::pass::MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`;
	class :ref:`ov::pass::ModelPass<doxid-classov_1_1pass_1_1_model_pass>`;
	class :ref:`ov::pass::PassBase<doxid-classov_1_1pass_1_1_pass_base>`;
	class :ref:`ov::pass::PassConfig<doxid-classov_1_1pass_1_1_pass_config>`;
	class :ref:`ov::pass::Serialize<doxid-classov_1_1pass_1_1_serialize>`;
	class :ref:`ov::pass::StreamSerialize<doxid-classov_1_1pass_1_1_stream_serialize>`;
	class :ref:`ov::pass::Validate<doxid-classov_1_1pass_1_1_validate>`;
	class :ref:`ov::pass::VisualizeTree<doxid-classov_1_1pass_1_1_visualize_tree>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void :ref:`ov::pass::disable_constant_folding<doxid-group__ov__pass__cpp__api_1ga39583fbe9bf1dc98c7d203bdaa7b4275>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

.. _details-group__ov__pass__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

OpenVINO C++ API to work with OpenVINO transformations

Global Functions
----------------

.. _doxid-group__ov__pass__cpp__api_1ga39583fbe9bf1dc98c7d203bdaa7b4275:
.. index:: pair: function; disable_constant_folding

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void ov::pass::disable_constant_folding(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node)

this method disables constant folding for given node. Under constant folding we consider :ref:`ConstantFolding <doxid-classov_1_1pass_1_1_constant_folding>` transformation, so other type of constant folding like ``get_constant_from_source`` doesn't work with this attribute. Also before using this attribute please consider two corner cases:

#. If for sub-graph like ShapeOf->ShapeOf we disable cf for first ShapeOf node, it doesn't spread to the second ShapeOf, so the entire sub-graph will be folded. (In case if first ShapeOf has exactly one consumer)

#. If node with disable_constant_folding was replaced with another node, the attribute will be lost because it is not copyable.

