.. index:: pair: class; ov::op::util::MultiSubGraphOp::OutputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description:

class ov::op::util::MultiSubGraphOp::OutputDescription
======================================================



Abstract class describes how a :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` output is produced from the body.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class OutputDescription
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<OutputDescription> :ref:`Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a53043b195b0af5f636fc35d5c8a501bc>`;
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a0afbfe5fd0e5c3ae1cad1d5171eca65f>`;

		// fields
	
		uint64_t :ref:`m_body_value_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a9d947f1afcfa8824f465cd12a031fe4c>` {0};
		uint64_t :ref:`m_output_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a7e49d71bfff773097a4b902b3c6c8329>` {0};

		// methods
	
		virtual std::shared_ptr<OutputDescription> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1ad4f288f5621c81c7beb65dab2ad8c9f5>`() const = 0;
		virtual const :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a0afbfe5fd0e5c3ae1cad1d5171eca65f>`& :ref:`get_type_info<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a483f130b4214ecd407c9ed3f1ef40009>`() const = 0;
	};

	// direct descendants

	class :ref:`BodyOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description>`;
	class :ref:`ConcatOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description>`;

