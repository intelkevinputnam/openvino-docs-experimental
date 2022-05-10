.. index:: pair: class; ov::op::util::MultiSubGraphOp::InputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description:

class ov::op::util::MultiSubGraphOp::InputDescription
=====================================================



Abstract class describes a connection between a :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input and the body.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class InputDescription
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<InputDescription> :ref:`Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a750d0d553f8c4d59c87775f8ba335568>`;
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a95bf848fcb2e4fe106397f1153647a4c>`;

		// fields
	
		uint64_t :ref:`m_input_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1ac46052c55790ec9683709526387b7c84>` {0};
		uint64_t :ref:`m_body_parameter_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a713aaf296a25beb90665248a4206c497>` {0};

		// methods
	
		virtual std::shared_ptr<InputDescription> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a3beee4948ec33b271b8e369a4670a230>`() const = 0;
		virtual const :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a95bf848fcb2e4fe106397f1153647a4c>`& :ref:`get_type_info<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a889cecbf7e215552f17acf10c9e38cbf>`() const = 0;
	};

	// direct descendants

	class :ref:`InvariantInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description>`;
	class :ref:`MergedInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description>`;
	class :ref:`SliceInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description>`;

