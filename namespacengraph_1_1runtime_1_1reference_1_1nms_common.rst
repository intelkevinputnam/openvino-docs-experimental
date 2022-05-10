.. index:: pair: namespace; ngraph::runtime::reference::nms_common
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1nms__common:

namespace ngraph::runtime::reference::nms_common
================================================

.. toctree::
	:hidden:

	BoxInfo <structngraph_1_1runtime_1_1reference_1_1nms_common_1_1BoxInfo.rst>
	Rectangle <structngraph_1_1runtime_1_1reference_1_1nms_common_1_1Rectangle.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace nms_common {

	// structs

	struct :ref:`BoxInfo<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_box_info>`;
	struct :ref:`Rectangle<doxid-structngraph_1_1runtime_1_1reference_1_1nms__common_1_1_rectangle>`;

	// global functions

	void :target:`nms_common_postprocessing<doxid-namespacengraph_1_1runtime_1_1reference_1_1nms__common_1aacc0366a11d6779af81d198008262a1e>`(
		void \* prois,
		void \* pscores,
		void \* pselected_num,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`& output_type,
		const std::vector<float>& selected_outputs,
		const std::vector<int64_t>& selected_indices,
		const std::vector<int64_t>& valid_outputs,
		const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`& selected_outputs_type
		);

	} // namespace nms_common
