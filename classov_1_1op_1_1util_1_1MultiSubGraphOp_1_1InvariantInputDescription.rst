.. index:: pair: class; ov::op::util::MultiSubGraphOp::InvariantInputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description:

class ov::op::util::MultiSubGraphOp::InvariantInputDescription
==============================================================



Overview
~~~~~~~~

Produces an input. :ref:`More...<details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class InvariantInputDescription: public :ref:`ov::op::util::MultiSubGraphOp::InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`
	{
	public:
		// fields
	
		 :ref:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description_1a95d5c8bad83c73373e58e2af798ef4be>`;

		// construction
	
		:ref:`InvariantInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description_1ab15d5a3ed091986305c8f5da14f2ec44>`(uint64_t input_index, uint64_t body_parameter_index);
		:ref:`InvariantInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description_1acd9e9a688645ec1b8b78007e3cc6cb10>`();

		// methods
	
		:ref:`OPENVINO_RTTI<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description_1afd05638bfe95d4b5f6eec3680b70de3d>`("InvariantInputDescription");
		virtual std::shared_ptr<:ref:`InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description_1ae8f4a001ed94643fe455c91d16bd1514>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`> :ref:`Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a750d0d553f8c4d59c87775f8ba335568>`;
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a95bf848fcb2e4fe106397f1153647a4c>`;

		// fields
	
		uint64_t :ref:`m_input_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1ac46052c55790ec9683709526387b7c84>` {0};
		uint64_t :ref:`m_body_parameter_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a713aaf296a25beb90665248a4206c497>` {0};

		// methods
	
		virtual std::shared_ptr<:ref:`InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a3beee4948ec33b271b8e369a4670a230>`() const = 0;
		virtual const :ref:`type_info_t<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a95bf848fcb2e4fe106397f1153647a4c>`& :ref:`get_type_info<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a889cecbf7e215552f17acf10c9e38cbf>`() const = 0;

.. _details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Produces an input.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description_1ab15d5a3ed091986305c8f5da14f2ec44:
.. index:: pair: function; InvariantInputDescription

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InvariantInputDescription(uint64_t input_index, uint64_t body_parameter_index)

Constructs a new instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_index

		- Position of the :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input

	*
		- body_parameter_index

		- Body parameter to receive input


