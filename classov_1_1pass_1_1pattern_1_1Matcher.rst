.. index:: pair: class; ov::pass::pattern::Matcher
.. _doxid-classov_1_1pass_1_1pattern_1_1_matcher:

class ov::pass::pattern::Matcher
================================



Overview
~~~~~~~~

:ref:`Matcher <doxid-classov_1_1pass_1_1pattern_1_1_matcher>` looks for node patterns in a computation graph. :ref:`More...<details-classov_1_1pass_1_1pattern_1_1_matcher>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <matcher.hpp>
	
	class Matcher
	{
	public:
		// typedefs
	
		typedef :ref:`ov::pass::pattern::PatternMap<doxid-namespaceov_1_1pass_1_1pattern_1a144abd970b801b71dce25ef83e35a736>` :target:`PatternMap<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1afedc2d0722ced5fe83e2abbc63885c24>`;

		// fields
	
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`m_match_root<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a290a70fc3ba41139b86d307ae10af40a>`;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`m_pattern_node<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a050e80bba4d09fbd904b95448426d84c>`;
		:ref:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>` :target:`m_pattern_map<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a6a1369c2013923ad07e286427337cb92>`;
		:ref:`PatternValueMaps<doxid-namespaceov_1_1pass_1_1pattern_1ab8e73ba29b51507d00110c6f5de468d3>` :target:`m_pattern_value_maps<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a13caed6d84b3bff2cbe7dfb1f8c1e99d>`;
		:ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :target:`m_matched_list<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a63e6567f0b9ee787267346e3cf67c6aa>`;

		// construction
	
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a0d513e3b916035223fb95bb28231ce4b>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> pattern_node, std::nullptr_t name);
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a4da82fe35ae76848c782129d74b73b09>`();
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a6564a26004c34df1dcce934e2a61cce3>`(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_node);
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a1749fcfa9ddf214724f9587eb9c3cb04>`(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_node, const std::string& name);
	
		:ref:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1abd74a12142fb82df7b6b89bae4fda9fd>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_node,
			const std::string& name,
			bool strict_mode
			);
	
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a3c78215de6e3dc29bc54e6e3b3b69e5c>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> pattern_node);
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a8fd7b6a7b8362a3683310e05ed9502dd>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> pattern_node, const std::string& name);
	
		:target:`Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a66db84c899accc2a87e7c0d59e6c1caa>`(
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> pattern_node,
			const std::string& name,
			bool strict_mode
			);

		// methods
	
		bool :ref:`match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a22d0626fa95b62de023cd6d92eca441c>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value);
		bool :target:`match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a266208cbb06a094794312662a5d87b3e>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> graph_node);
		bool :ref:`match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ae21bae739de8f418cc0fd15fe37fba33>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value, const :ref:`PatternMap<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1afedc2d0722ced5fe83e2abbc63885c24>`& previous_matches);
	
		bool :target:`match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a8458845a2a7b8151696e89b8cbbb99bd>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value,
			const :ref:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>`& previous_matches
			);
	
		bool :target:`is_contained_match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ab85c7b010b9aca0a532f3572b4266516>`(
			const :ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& exclusions = {},
			bool ignore_unused = true
			);
	
		const :ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` :target:`get_matched_nodes<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1af5b3772fee76a22f9f75fd10e25ed61e>`();
		const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& :target:`get_matched_values<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1af2ae2f4956619c9983a41df5347811cc>`() const;
		:ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& :target:`get_matched_values<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a743a3c374cc869d829b9c14712322242>`();
		void :target:`reset<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a407d4317955facd74ac8b87d504e8794>`();
		const std::string& :target:`get_name<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ad563efbe98612c64ddfefd5f3c53ed22>`();
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_pattern<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ab0af67adeed20d5417c92e318530d108>`();
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_pattern_value<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ae6028c996ddf49af96b31fd4c899e34f>`();
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_match_root<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1aac78406378ae7df09548336d89cf8ac4>`();
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_match_value<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a381fd33c0b1513c7936f99a42616104d>`();
		:ref:`PatternMap<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1afedc2d0722ced5fe83e2abbc63885c24>` :target:`get_pattern_map<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1adddddad33ec1e3d721ce9174b2c2fd67>`() const;
		:ref:`PatternValueMap<doxid-namespaceov_1_1pass_1_1pattern_1ae043de24e08e8683fa62ea0a66b27af5>`& :target:`get_pattern_value_map<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a7cd4e7eaf4fb4c3c28f434c3c73543ea>`();
		:ref:`PatternValueMaps<doxid-namespaceov_1_1pass_1_1pattern_1ab8e73ba29b51507d00110c6f5de468d3>`& :target:`get_pattern_value_maps<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a8a8d03bc70e59784464b452b9b93a18e>`();
		size_t :ref:`add_node<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ac9ddcb541cf739aad96a006e2138aa89>`(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> node);
	
		virtual bool :target:`match_value<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a5ae521499ddc88c0ca5239cd82f18161>`(
			const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_value,
			const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value
			);
	
		bool :target:`is_strict_mode<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a62a0f95b99797c8a97dad563c1137ed9>`();
	
		virtual bool :target:`match_arguments<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a0d7e896f06c18e4f04bdc047579899c8>`(
			:ref:`Node<doxid-classov_1_1_node>` \* pattern_node,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& graph_node
			);
	
		void :target:`capture<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ae11f560ba6246ade46a59e0a6113c41a>`(const std::set<:ref:`Node<doxid-classov_1_1_node>` \*>& static_nodes);
		void :target:`clear_state<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a7691800ffaf0453f223805db0a337e44>`();
		size_t :target:`get_number_of_recurrent_matches<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a51ce3a828baa6ff23ef73e54072d8014>`() const;
		:ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` :target:`get_bound_nodes_for_pattern<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a5132682f00841cc83d56c682ed0ef4fe>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern) const;
		size_t :target:`get_number_of_bound_labels<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a0c6b2e2cd4e5ee2b8f10a202b60970fd>`() const;
		:ref:`MatcherState<doxid-classov_1_1pass_1_1pattern_1_1_matcher_state>` :ref:`start_match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1aa999fc1293f4ecd6627a77fd8423a1c6>`();
	
		template <typename T>
		static std::shared_ptr<T> :target:`unique_match<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a5827cc78174b1bdde6429d3e5472ed53>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	};
.. _details-classov_1_1pass_1_1pattern_1_1_matcher:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Matcher <doxid-classov_1_1pass_1_1pattern_1_1_matcher>` looks for node patterns in a computation graph. The patterns are described by an automaton that is described by an extended computation graph. The matcher executes by attempting to match the start node of the pattern to a computation graph value (output of a :ref:`Node <doxid-classov_1_1_node>`). In addition to determing if a match occurs, a pattern node may add graph nodes to a list of matched nodes, associate nodes with graph values, and start submatches. Submatches add match state changes to the enclosing match if the submatch succeeds; otherwise the state is reverted.

The default match behavior of a pattern node with a graph nodes is that the computation graph value is added to the end of the matched value list and the match succeeds if the node/pattern types match and the input values match. In the case of a commutative node, the inputs can match in any order. If the matcher is in strict mode, the graph value element type and shape must also match.

Pattern nodes that have different match behavior are in :ref:`ov::pass::pattern::op <doxid-namespaceov_1_1pass_1_1pattern_1_1op>` and have descriptions of their match behavior.

Construction
------------

.. _doxid-classov_1_1pass_1_1pattern_1_1_matcher_1abd74a12142fb82df7b6b89bae4fda9fd:
.. index:: pair: function; Matcher

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Matcher(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_node,
		const std::string& name,
		bool strict_mode
		)

Constructs a :ref:`Matcher <doxid-classov_1_1pass_1_1pattern_1_1_matcher>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pattern_node

		- is a pattern sub graph that will be matched against input graphs

	*
		- name

		- is a string which is used for logging and disabling a matcher

	*
		- strict_mode

		- forces a matcher to consider shapes and ET of nodes

Methods
-------

.. _doxid-classov_1_1pass_1_1pattern_1_1_matcher_1a22d0626fa95b62de023cd6d92eca441c:
.. index:: pair: function; match

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool match(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value)

Matches a pattern to ``graph_node``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- graph_value

		- is an input graph to be matched against

.. _doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ae21bae739de8f418cc0fd15fe37fba33:
.. index:: pair: function; match

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool match(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value, const :ref:`PatternMap<doxid-classov_1_1pass_1_1pattern_1_1_matcher_1afedc2d0722ced5fe83e2abbc63885c24>`& previous_matches)

Matches a pattern to ``graph_node``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- graph_value

		- is an input graph to be matched against

	*
		- previous_matches

		- contains previous mappings from labels to nodes to use

.. _doxid-classov_1_1pass_1_1pattern_1_1_matcher_1ac9ddcb541cf739aad96a006e2138aa89:
.. index:: pair: function; add_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t add_node(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> node)

Low-level helper to match recurring patterns.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- graph

		- is a graph to be matched against

	*
		- pattern

		- is a recurring pattern

	*
		- rpattern

		- specifies a node to recur from next

	*
		- patterns

		- a map from labels to matches

.. _doxid-classov_1_1pass_1_1pattern_1_1_matcher_1aa999fc1293f4ecd6627a77fd8423a1c6:
.. index:: pair: function; start_match

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`MatcherState<doxid-classov_1_1pass_1_1pattern_1_1_matcher_state>` start_match()

Try a match.


