.. index:: pair: namespace; ov::op::v7
.. _doxid-namespaceov_1_1op_1_1v7:

namespace ov::op::v7
====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v7 {

	// classes

	class :ref:`DFT<doxid-classov_1_1op_1_1v7_1_1_d_f_t>`;
	class :ref:`Einsum<doxid-classov_1_1op_1_1v7_1_1_einsum>`;
	class :ref:`Gather<doxid-classov_1_1op_1_1v7_1_1_gather>`;
	class :ref:`Gelu<doxid-classov_1_1op_1_1v7_1_1_gelu>`;
	class :ref:`IDFT<doxid-classov_1_1op_1_1v7_1_1_i_d_f_t>`;
	class :ref:`Roll<doxid-classov_1_1op_1_1v7_1_1_roll>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v7_1a40d3d2476a6eadd2404eb3b439586e80>`(
		const :ref:`Einsum<doxid-classov_1_1op_1_1v7_1_1_einsum>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v7_1a2485a8aa332eaf0ab00259681355162a>`(
		const :ref:`ov::op::v7::Roll<doxid-classov_1_1op_1_1v7_1_1_roll>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	} // namespace v7
