.. index:: pair: namespace; ov::pass::pattern
.. _doxid-namespaceov_1_1pass_1_1pattern:

namespace ov::pass::pattern
===========================

.. toctree::
	:hidden:

	op <namespaceov_1_1pass_1_1pattern_1_1op.rst>
	Matcher <classov_1_1pass_1_1pattern_1_1Matcher.rst>
	MatcherState <classov_1_1pass_1_1pattern_1_1MatcherState.rst>
	RecurrentMatcher <classov_1_1pass_1_1pattern_1_1RecurrentMatcher.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace pattern {

	// namespaces

	namespace :ref:`ov::pass::pattern::op<doxid-namespaceov_1_1pass_1_1pattern_1_1op>`;

	// typedefs

	typedef std::map<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`> :target:`RPatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ab6230ad6e5b69974b134345fe445c623>`;
	typedef std::map<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :target:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>`;
	typedef std::vector<:ref:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>`> :target:`PatternValueMaps<doxid-namespaceov_1_1pass_1_1pattern_1ab8e73ba29b51507d00110c6f5de468d3>`;
	typedef std::map<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :target:`PatternMap<doxid-namespaceov_1_1pass_1_1pattern_1a144abd970b801b71dce25ef83e35a736>`;

	// classes

	class :ref:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`;
	class :ref:`MatcherState<doxid-classov_1_1pass_1_1pattern_1_1_matcher_state>`;
	class :ref:`RecurrentMatcher<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`any_input<doxid-namespaceov_1_1pass_1_1pattern_1aaaacfc27e6d09ca94625c3ee2c190aff>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`any_input<doxid-namespaceov_1_1pass_1_1pattern_1aa6626ad948bf81d8f0309b2b4bb7b5eb>`(const :ref:`pattern::op::ValuePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a1c63e9ca6a1801153d3aa30f857cfbbf>`& pred);
	:ref:`PatternMap<doxid-namespaceov_1_1pass_1_1pattern_1a144abd970b801b71dce25ef83e35a736>` :target:`as_pattern_map<doxid-namespaceov_1_1pass_1_1pattern_1a0efa88e8fd883a6cce9157a2e5e791a8>`(const :ref:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>`& pattern_value_map);
	:ref:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>` :target:`as_pattern_value_map<doxid-namespaceov_1_1pass_1_1pattern_1a240f4f651f5aaa4de63f55a506f859fa>`(const :ref:`PatternMap<doxid-namespaceov_1_1pass_1_1pattern_1a144abd970b801b71dce25ef83e35a736>`& pattern_map);

	template <typename T>
	std::function<bool(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`has_class<doxid-namespaceov_1_1pass_1_1pattern_1a8e5fe8f6cf912db7736cc82ca0fb82c2>`();

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`consumers_count<doxid-namespaceov_1_1pass_1_1pattern_1a3a149c6c14b37244cfa997cd0048b390>`(size_t n);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`has_static_dim<doxid-namespaceov_1_1pass_1_1pattern_1a940d1e041aace73cde0f753da9ffd3ea>`(size_t pos);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`has_static_dims<doxid-namespaceov_1_1pass_1_1pattern_1a7cf6eee74aa108125fe322b142d6c177>`(const std::vector<size_t>& dims);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`has_static_shape<doxid-namespaceov_1_1pass_1_1pattern_1a585d1c6966bedd91a481b8942a802bca>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`has_static_rank<doxid-namespaceov_1_1pass_1_1pattern_1a4a3625760fbb2bd4f7e80d3581b270b7>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`rank_equals<doxid-namespaceov_1_1pass_1_1pattern_1a6738b5099ad006823d0a0e8dedceb65c>`(const :ref:`Dimension<doxid-classov_1_1_dimension>`& expected_rank);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`type_matches<doxid-namespaceov_1_1pass_1_1pattern_1ae0b890ec72a9185944835bd430229d8b>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::function<bool(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`type_matches_any<doxid-namespaceov_1_1pass_1_1pattern_1af26af21ef2b6d1417edfd8267c7a472a>`(const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& types);

	template <
		class T,
		typename std::enable_if<ngraph::HasTypeInfoMember<T>::value, bool>::type = true
		>
	void :target:`collect_wrap_info<doxid-namespaceov_1_1pass_1_1pattern_1adde51a8fae92bf23a3bf4fc4c15b3936>`(std::vector<:ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`>& info);

	template <
		class T,
		class... Targs,
		typename std::enable_if<sizeof...(Targs) !=0, bool>::type = true
		>
	void :target:`collect_wrap_info<doxid-namespaceov_1_1pass_1_1pattern_1a896d790274477de2c5895203cb474694>`(std::vector<:ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`>& info);

	template <class... Args>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`wrap_type<doxid-namespaceov_1_1pass_1_1pattern_1a2fd26ffb1c9bf414b99a15439fc94656>`(
		const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs,
		const :ref:`pattern::op::ValuePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a1c63e9ca6a1801153d3aa30f857cfbbf>`& pred
		);

	template <class... Args>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`wrap_type<doxid-namespaceov_1_1pass_1_1pattern_1af3a615596a7020260f0624e00a147cfe>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs = {});

	template <class... Args>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`wrap_type<doxid-namespaceov_1_1pass_1_1pattern_1ac4c4752ec26763c02c5c5fa479b98588>`(const :ref:`pattern::op::ValuePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a1c63e9ca6a1801153d3aa30f857cfbbf>`& pred);

	} // namespace pattern
