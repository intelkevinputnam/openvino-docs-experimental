.. index:: pair: class; ngraph::op::internal::NmsStaticShapeIE
.. _doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e:

class ngraph::op::internal::NmsStaticShapeIE
============================================

.. toctree::
	:hidden:

	init_rt_result <structngraph_1_1op_1_1internal_1_1NmsStaticShapeIE_1_1init_rt_result.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <nms_static_shape_ie.hpp>
	
	template <typename BaseNmsOp>
	class NmsStaticShapeIE: public BaseNmsOp
	{
	public:
		// typedefs
	
		typedef typename BaseNmsOp::Attributes :target:`Attributes<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a3b97b48e422e79754b4782eadc5412b6>`;

		// structs
	
		struct :ref:`init_rt_result<doxid-structngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1_1init__rt__result>`;

		// construction
	
		:target:`NmsStaticShapeIE<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a61b36b4f5ecce3a8f1a043b257336581>`();
	
		:ref:`NmsStaticShapeIE<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a8a0e718348dd16f0f19a973ae11de6ad>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& boxes,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& scores,
			const :ref:`Attributes<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a3b97b48e422e79754b4782eadc5412b6>`& attrs
			);

		// methods
	
		void :target:`validate_and_infer_types<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1aeb5509fd84f68206c6f73c312e76eef4>`();
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_with_new_inputs<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a6c50f4a88af9ad237e5b0b4f901da918>`(const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& new_args) const;
	};
.. _details-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Construction
------------

.. _doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a8a0e718348dd16f0f19a973ae11de6ad:
.. index:: pair: function; NmsStaticShapeIE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NmsStaticShapeIE(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& boxes,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& scores,
		const :ref:`Attributes<doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e_1a3b97b48e422e79754b4782eadc5412b6>`& attrs
		)

Constructs a :ref:`NmsStaticShapeIE <doxid-classngraph_1_1op_1_1internal_1_1_nms_static_shape_i_e>` operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- boxes

		- Node producing the box coordinates

	*
		- scores

		- Node producing the box scores

	*
		- attrs

		- Attributes of the operation


