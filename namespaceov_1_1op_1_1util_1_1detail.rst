.. index:: pair: namespace; ov::op::util::detail
.. _doxid-namespaceov_1_1op_1_1util_1_1detail:

namespace ov::op::util::detail
==============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace detail {

	// global functions

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`sigmoid<doxid-namespaceov_1_1op_1_1util_1_1detail_1ab6b80021d71d66e1f6eaa4ce49c28062>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& arg,
		float alpha,
		float beta
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`tanh<doxid-namespaceov_1_1op_1_1util_1_1detail_1a32432209260f9b3b6fdbab99ae0bcd7b>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& arg,
		float alpha,
		float beta
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`relu<doxid-namespaceov_1_1op_1_1util_1_1detail_1ab226e58ed2f3e7bbdea890077afe523f>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& arg,
		float alpha,
		float beta
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`hardsigmoid<doxid-namespaceov_1_1op_1_1util_1_1detail_1a6cf9b19f2f48cf60308dca968a364d20>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& arg,
		float alpha,
		float beta
		);

	} // namespace detail
