.. index:: pair: namespace; ov::pass::pattern::op
.. _doxid-namespaceov_1_1pass_1_1pattern_1_1op:

namespace ov::pass::pattern::op
===============================

.. toctree::
	:hidden:

	Any <classov_1_1pass_1_1pattern_1_1op_1_1Any.rst>
	AnyOf <classov_1_1pass_1_1pattern_1_1op_1_1AnyOf.rst>
	AnyOutput <classov_1_1pass_1_1pattern_1_1op_1_1AnyOutput.rst>
	Branch <classov_1_1pass_1_1pattern_1_1op_1_1Branch.rst>
	Capture <classov_1_1pass_1_1pattern_1_1op_1_1Capture.rst>
	Label <classov_1_1pass_1_1pattern_1_1op_1_1Label.rst>
	Or <classov_1_1pass_1_1pattern_1_1op_1_1Or.rst>
	Pattern <classov_1_1pass_1_1pattern_1_1op_1_1Pattern.rst>
	Skip <classov_1_1pass_1_1pattern_1_1op_1_1Skip.rst>
	True <classov_1_1pass_1_1pattern_1_1op_1_1True.rst>
	WrapType <classov_1_1pass_1_1pattern_1_1op_1_1WrapType.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace op {

	// typedefs

	typedef std::function<bool(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>)> :target:`NodePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a773344323e39ff5d3e25bc79c06dac5d>`;
	typedef std::function<bool(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>&value)> :target:`ValuePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a1c63e9ca6a1801153d3aa30f857cfbbf>`;

	// classes

	class :ref:`Any<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_any>`;
	class :ref:`AnyOf<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_any_of>`;
	class :ref:`AnyOutput<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_any_output>`;
	class :ref:`Branch<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_branch>`;
	class :ref:`Capture<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_capture>`;
	class :ref:`Label<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_label>`;
	class :ref:`Or<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_or>`;
	class :ref:`Pattern<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_pattern>`;
	class :ref:`Skip<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_skip>`;
	class :ref:`True<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_true>`;
	class :ref:`WrapType<doxid-classov_1_1pass_1_1pattern_1_1op_1_1_wrap_type>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ValuePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a1c63e9ca6a1801153d3aa30f857cfbbf>` :target:`as_value_predicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1af6fb4d8b65426cc381713d2c788a7d1f>`(:ref:`NodePredicate<doxid-namespaceov_1_1pass_1_1pattern_1_1op_1a773344323e39ff5d3e25bc79c06dac5d>` pred);

	} // namespace op
