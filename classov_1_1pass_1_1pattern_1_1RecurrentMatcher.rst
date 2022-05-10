.. index:: pair: class; ov::pass::pattern::RecurrentMatcher
.. _doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher:

class ov::pass::pattern::RecurrentMatcher
=========================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <matcher.hpp>
	
	class RecurrentMatcher
	{
	public:
		// construction
	
		:ref:`RecurrentMatcher<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1a087e5d9dcb57aadeeaba177566d988b6>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& initial_pattern,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& rpattern,
			const std::set<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& correlated_patterns
			);
	
		:ref:`RecurrentMatcher<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1ac26c169bad975d858dcec3eaf8ce1c03>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& rpattern,
			const std::set<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& correlated_patterns
			);
	
		:target:`RecurrentMatcher<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1ae5e30d2f382a74e5d4622325a9c50fff>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& initial_pattern,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& rpattern,
			const std::set<std::shared_ptr<:ref:`op::Label<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_label>`>>& correlated_patterns
			);
	
		:target:`RecurrentMatcher<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1a41aba58f4ef4212e657c8d3c905606bc>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& rpattern,
			const std::set<std::shared_ptr<:ref:`op::Label<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_label>`>>& correlated_patterns
			);

		// methods
	
		:ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` :ref:`get_bound_nodes_for_pattern<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1aa36a13901a8b3842814d20e3cb3d0ae7>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& pattern) const;
		size_t :target:`get_number_of_recurrent_matches<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1aaafdb3b07ee00c024b9e66984cf20319>`() const;
		size_t :target:`get_number_of_bound_labels<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1a1b8c3ebc996e801d7e2c2bbed51d8ed7>`() const;
		bool :ref:`match<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1ac3311a1f5f1d87b24f6532e9bb765400>`(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> graph);
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_match_root<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1abc1bab98fe54ce6f05a19e87b6e8c288>`();
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_match_value<doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1a138f4c64a839d0ac35de895dba12b120>`();
	};
.. _details-classov_1_1pass_1_1pattern_1_1_recurrent_matcher:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Construction
------------

.. _doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1a087e5d9dcb57aadeeaba177566d988b6:
.. index:: pair: function; RecurrentMatcher

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RecurrentMatcher(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& initial_pattern,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern,
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& rpattern,
		const std::set<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& correlated_patterns
		)

Constructs a :ref:`RecurrentMatcher <doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher>` object. Reccurent Matchers are used to match repeating patterns (e.g. RNN, LSTM, GRU cells)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- initial_pattern

		- is a pattern sub graph describing the initial cell

	*
		- pattern

		- is a pattern sub graph describing an individual cell

	*
		- rpattern

		- is a (recurring) label to denote which node the next match should start at

	*
		- correlated_patterns

		- is a set of labels whose bound nodes must remain the same across all cells

.. _doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1ac26c169bad975d858dcec3eaf8ce1c03:
.. index:: pair: function; RecurrentMatcher

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RecurrentMatcher(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern,
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& rpattern,
		const std::set<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& correlated_patterns
		)

Constructs a :ref:`RecurrentMatcher <doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher>` object. Reccurent Matchers are used to match repeating patterns (e.g. RNN, LSTM, GRU cells)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pattern

		- is a pattern sub graph describing an individual cell

	*
		- rpattern

		- is a (recurring) label to denote which node the next match should start at

	*
		- correlated_patterns

		- is a set of labels whose bound nodes must remain the same across all cells

Methods
-------

.. _doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1aa36a13901a8b3842814d20e3cb3d0ae7:
.. index:: pair: function; get_bound_nodes_for_pattern

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` get_bound_nodes_for_pattern(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& pattern) const

Returns a vector of bound nodes for a given label (used in a pattern describing an individual cell.

.. _doxid-classov_1_1pass_1_1pattern_1_1_recurrent_matcher_1ac3311a1f5f1d87b24f6532e9bb765400:
.. index:: pair: function; match

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool match(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> graph)

Tries to match a pattern for an individual cell to a given ``graph``.


