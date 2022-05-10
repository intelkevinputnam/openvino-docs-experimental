.. index:: pair: class; ov::op::util::MultiSubGraphOp::MergedInputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description:

class ov::op::util::MultiSubGraphOp::MergedInputDescription
===========================================================



Overview
~~~~~~~~

Describes a body input initialized from a :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input on the first iteration, and then a body output thereafter. :ref:`More...<details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class MergedInputDescription: public :ref:`ov::op::util::MultiSubGraphOp::InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`
	{
	public:
		// fields
	
		 :ref:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1aab1524a076837988cf8bd8ca8001c2bf>`;
		uint64_t :ref:`m_body_value_index<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1ac1170f665c0d1ee4bdf09ed5ba8492e0>` {0};

		// construction
	
		:ref:`MergedInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1a7009a8967ae4b083023aa8c2ace65ee8>`(
			uint64_t input_index,
			uint64_t body_parameter_index,
			uint64_t body_value_index
			);
	
		:ref:`MergedInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1ac667460e8ea929de6af54a933f4a0726>`();

		// methods
	
		:ref:`OPENVINO_RTTI<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1a7b456670e175b3ac8a3c83ee2a63fd52>`("MergedInputDescription");
		virtual std::shared_ptr<:ref:`InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1a4c2326bedaa156cbab0c3279324898e1>`() const;
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

.. _details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Describes a body input initialized from a :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input on the first iteration, and then a body output thereafter.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description_1a7009a8967ae4b083023aa8c2ace65ee8:
.. index:: pair: function; MergedInputDescription

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MergedInputDescription(
		uint64_t input_index,
		uint64_t body_parameter_index,
		uint64_t body_value_index
		)

Constructs a new instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_index

		- Position of the :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input supplying a value to body_parameter for the initial iteration.

	*
		- body_parameter_index

		- Body parameter position to receive input.

	*
		- body_value_index

		- Body value to supply body_parameter for successive iterations.


