.. index:: pair: class; ov::op::util::MultiSubGraphOp::SliceInputDescription
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description:

class ov::op::util::MultiSubGraphOp::SliceInputDescription
==========================================================



Overview
~~~~~~~~

Describes a body input formed from slices of an input to :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`. :ref:`More...<details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class SliceInputDescription: public :ref:`ov::op::util::MultiSubGraphOp::InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`
	{
	public:
		// fields
	
		 :ref:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a3ad2913cc28381cd5a7c17531cf1e123>`;
		int64_t :ref:`m_start<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a8d02b3d2c4a690dc55fccdacf3e15435>` {0};
		int64_t :ref:`m_stride<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a89dc8bd8acc05f604b6cb29ea1d7095b>` {0};
		int64_t :ref:`m_part_size<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a53498319b451c29a804fbadd61c8653a>` {0};
		int64_t :ref:`m_end<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1ab42c6967cbaa57ebc868d6e49d6aecc7>` {0};
		int64_t :ref:`m_axis<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1ac6a371817634f69718e9fb6ed0e7cb64>` {0};

		// construction
	
		:ref:`SliceInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a2d2e9ac6476fef260efc81078f4b676c>`(
			uint64_t input_index,
			uint64_t body_parameter_index,
			int64_t start,
			int64_t stride,
			int64_t part_size,
			int64_t end,
			int64_t axis
			);
	
		:ref:`SliceInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a6db6266282f9acea20375a63d7f0229f>`();

		// methods
	
		:ref:`OPENVINO_RTTI<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a721383d99ab8be9d94b84f159e1e2b1f>`("SliceInputDescription");
		virtual std::shared_ptr<:ref:`InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`> :ref:`copy<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a9bdfb02cedd8d7690ffe79ff15994d66>`() const;
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

.. _details-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Describes a body input formed from slices of an input to :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description_1a2d2e9ac6476fef260efc81078f4b676c:
.. index:: pair: function; SliceInputDescription

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SliceInputDescription(
		uint64_t input_index,
		uint64_t body_parameter_index,
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
		- input_index

		- Position of the :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input

	*
		- body_parameter_index

		- Body parameter position to receive input

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


