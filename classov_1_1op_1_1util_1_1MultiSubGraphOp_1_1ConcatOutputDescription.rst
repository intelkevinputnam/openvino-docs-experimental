.. index:: pair: class; ov::op::util::MultiSubGraphOp::ConcatOutputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description:

class ov::op::util::MultiSubGraphOp::ConcatOutputDescription
============================================================



Overview
~~~~~~~~

Produces an output by concatenating an output from each iteration. :ref:`More...<details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class ConcatOutputDescription: public :ref:`ov::op::util::MultiSubGraphOp::OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`
	{
	public:
		// fields
	
		 :ref:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1aec59bad6471e7bc923132576c3ac1e7d>`;
		int64_t :ref:`m_start<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a75903c86cf9f1e42a5dc0e0c2d497ff1>` {0};
		int64_t :ref:`m_stride<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a3e1aab40faf9a5e53d4915366e8ac406>` {0};
		int64_t :ref:`m_part_size<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1ac14fd20f15e1788e408fcbb8039b75ef>` {0};
		int64_t :ref:`m_end<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a22fd9b15c09fb1aad9ab3c7d2c99784e>` {0};
		int64_t :ref:`m_axis<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a0c30565af05562d7a683fe21ed3a0275>` {0};

		// construction
	
		:ref:`ConcatOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a9a84c80e81361cb3b162655984b106ff>`(
			uint64_t body_value_index,
			uint64_t output_index,
			int64_t start,
			int64_t stride,
			int64_t part_size,
			int64_t end,
			int64_t axis
			);
	
		:ref:`ConcatOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a08c390139bd9dcb0c2f1cccf3f484f01>`();

		// methods
	
		:ref:`OPENVINO_RTTI<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a44581c83bd5a43f1577f943b810c2b7d>`("ConcatOutputDescription");
		virtual std::shared_ptr<:ref:`OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1ac3cac36e1def4caf8dfe63996434e4db>`() const;
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

.. _details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Produces an output by concatenating an output from each iteration.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description_1a9a84c80e81361cb3b162655984b106ff:
.. index:: pair: function; ConcatOutputDescription

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ConcatOutputDescription(
		uint64_t body_value_index,
		uint64_t output_index,
		int64_t start,
		int64_t stride,
		int64_t part_size,
		int64_t end,
		int64_t axis
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

		- The :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` output index

	*
		- start

		- First index for slices

	*
		- stride

		- Step amount for slices

	*
		- part_size

		- Width of slices

	*
		- end

		- Last index for slices

	*
		- axis

		- Axis being sliced


