.. index:: pair: class; ov::op::util::MultiSubGraphOp::BodyOutputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description:

class ov::op::util::MultiSubGraphOp::BodyOutputDescription
==========================================================



Overview
~~~~~~~~

Produces an output from a specific iteration. :ref:`More...<details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class BodyOutputDescription: public :ref:`ov::op::util::MultiSubGraphOp::OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`
	{
	public:
		// fields
	
		 :ref:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1a11d2e306ecd0cd1dee0b046836d2af63>`;
		int64_t :ref:`m_iteration<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1aedf2749265998ece99708b3a05c19fdd>` {0};

		// construction
	
		:ref:`BodyOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1a20868202eaba9965cf6bd50926fbe57e>`(
			uint64_t body_value_index,
			uint64_t output_index,
			int64_t iteration = -1
			);
	
		:ref:`BodyOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1a1611a04601b35fa148382f322383045d>`();

		// methods
	
		:ref:`OPENVINO_RTTI<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1acb73fae540cce0d65e65622f923d5e5a>`("BodyOutputDescription");
		virtual std::shared_ptr<:ref:`MultiSubGraphOp::OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1a64889d73ea4ceb84c41e60ea13202ecd>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`> :ref:`Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a53043b195b0af5f636fc35d5c8a501bc>`;
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a0afbfe5fd0e5c3ae1cad1d5171eca65f>`;

		// fields
	
		uint64_t :ref:`m_body_value_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a9d947f1afcfa8824f465cd12a031fe4c>` {0};
		uint64_t :ref:`m_output_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a7e49d71bfff773097a4b902b3c6c8329>` {0};

		// methods
	
		virtual std::shared_ptr<:ref:`OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1ad4f288f5621c81c7beb65dab2ad8c9f5>`() const = 0;
		virtual const :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a0afbfe5fd0e5c3ae1cad1d5171eca65f>`& :ref:`get_type_info<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a483f130b4214ecd407c9ed3f1ef40009>`() const = 0;

.. _details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Produces an output from a specific iteration.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description_1a20868202eaba9965cf6bd50926fbe57e:
.. index:: pair: function; BodyOutputDescription

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BodyOutputDescription(
		uint64_t body_value_index,
		uint64_t output_index,
		int64_t iteration = -1
		)

Constructs a new instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- body_value_index

		- A body value that produces the output

	*
		- output_index

		- The :ref:`SubGraphOp <doxid-classov_1_1op_1_1util_1_1_sub_graph_op>` output index

	*
		- iteration

		- which iteration (typically -1, final) will supply the value


