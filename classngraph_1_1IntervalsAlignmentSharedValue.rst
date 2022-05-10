.. index:: pair: class; ngraph::IntervalsAlignmentSharedValue
.. _doxid-classngraph_1_1_intervals_alignment_shared_value:

class ngraph::IntervalsAlignmentSharedValue
===========================================

.. toctree::
	:hidden:

	Interval <classngraph_1_1IntervalsAlignmentSharedValue_1_1Interval.rst>

:ref:`IntervalsAlignmentSharedValue <doxid-classngraph_1_1_intervals_alignment_shared_value>` is used by :ref:`IntervalsAlignmentAttribute <doxid-classngraph_1_1_intervals_alignment_attribute>` as attribute shared value.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <intervals_alignment_attribute.hpp>
	
	class IntervalsAlignmentSharedValue
	{
	public:
		// classes
	
		class :ref:`Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>`;

		// fields
	
		:ref:`Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>` :target:`combinedInterval<doxid-classngraph_1_1_intervals_alignment_shared_value_1a31f901332422672afc2324cad713d7ee>`;
		:ref:`Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>` :target:`minInterval<doxid-classngraph_1_1_intervals_alignment_shared_value_1a40ce741257d6bd64ae4acbfd152abf60>`;
		size_t :target:`minLevels<doxid-classngraph_1_1_intervals_alignment_shared_value_1a9af4d91ee963e859085c4f1203228edb>` = 0;
		std::set<element::Type> :target:`preferablePrecisions<doxid-classngraph_1_1_intervals_alignment_shared_value_1a9f3e5a781510b5a101c700abfba67a9f>`;

		// construction
	
		:target:`IntervalsAlignmentSharedValue<doxid-classngraph_1_1_intervals_alignment_shared_value_1a05dccf36f66e409ef0bcba27e19dcf38>`();
	
		:target:`IntervalsAlignmentSharedValue<doxid-classngraph_1_1_intervals_alignment_shared_value_1a60b6021a8aaf63e90c44a59931ee00bf>`(
			const :ref:`Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>`& combinedInterval,
			const :ref:`Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>`& minInterval,
			const size_t minLevels
			);
	};

