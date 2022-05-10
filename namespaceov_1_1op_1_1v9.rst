.. index:: pair: namespace; ov::op::v9
.. _doxid-namespaceov_1_1op_1_1v9:

namespace ov::op::v9
====================

.. toctree::
	:hidden:

	IRDFT <classov_1_1op_1_1v9_1_1IRDFT.rst>
	RDFT <classov_1_1op_1_1v9_1_1RDFT.rst>
	ROIAlign <classov_1_1op_1_1v9_1_1ROIAlign.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v9 {

	// classes

	class :ref:`Eye<doxid-classov_1_1op_1_1v9_1_1_eye>`;
	class :ref:`IRDFT<doxid-classov_1_1op_1_1v9_1_1_i_r_d_f_t>`;
	class :ref:`RDFT<doxid-classov_1_1op_1_1v9_1_1_r_d_f_t>`;
	class :ref:`ROIAlign<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v9_1ad971a444385573680a22d58d224bc22d>`(
		const :ref:`ov::op::v9::ROIAlign<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	} // namespace v9
