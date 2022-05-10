.. index:: pair: namespace; ngraph::op
.. _doxid-namespacengraph_1_1op:

namespace ngraph::op
====================

.. toctree::
	:hidden:

	internal <namespacengraph_1_1op_1_1internal.rst>
	util <namespacengraph_1_1op_1_1util.rst>
	v0 <namespacengraph_1_1op_1_1v0.rst>
	v1 <namespacengraph_1_1op_1_1v1.rst>
	v3 <namespacengraph_1_1op_1_1v3.rst>
	v4 <namespacengraph_1_1op_1_1v4.rst>
	v5 <namespacengraph_1_1op_1_1v5.rst>
	v6 <namespacengraph_1_1op_1_1v6.rst>
	v7 <namespacengraph_1_1op_1_1v7.rst>
	v8 <namespacengraph_1_1op_1_1v8.rst>
	v9 <namespacengraph_1_1op_1_1v9.rst>
	InterpolateIEAttrs <structngraph_1_1op_1_1InterpolateIEAttrs.rst>
	ResampleIEAttrs <structngraph_1_1op_1_1ResampleIEAttrs.rst>
	ConvolutionIE <classngraph_1_1op_1_1ConvolutionIE.rst>
	CropIE <classngraph_1_1op_1_1CropIE.rst>
	DeconvolutionIE <classngraph_1_1op_1_1DeconvolutionIE.rst>
	Eltwise <classngraph_1_1op_1_1Eltwise.rst>
	FullyConnected <classngraph_1_1op_1_1FullyConnected.rst>
	GRUCellIE <classngraph_1_1op_1_1GRUCellIE.rst>
	GRUSequenceIE <classngraph_1_1op_1_1GRUSequenceIE.rst>
	GatherIE <classngraph_1_1op_1_1GatherIE.rst>
	GatherTreeIE <classngraph_1_1op_1_1GatherTreeIE.rst>
	HardSigmoid_IE <classngraph_1_1op_1_1HardSigmoid_IE.rst>
	Interp <classngraph_1_1op_1_1Interp.rst>
	LRN_IE <classngraph_1_1op_1_1LRN_IE.rst>
	LSTMCellIE <classngraph_1_1op_1_1LSTMCellIE.rst>
	LSTMSequenceIE <classngraph_1_1op_1_1LSTMSequenceIE.rst>
	NonMaxSuppressionIE <classngraph_1_1op_1_1NonMaxSuppressionIE.rst>
	NonMaxSuppressionIE2 <classngraph_1_1op_1_1NonMaxSuppressionIE2.rst>
	NonMaxSuppressionIE3 <classngraph_1_1op_1_1NonMaxSuppressionIE3.rst>
	NormalizeIE <classngraph_1_1op_1_1NormalizeIE.rst>
	OneHotIE <classngraph_1_1op_1_1OneHotIE.rst>
	PadIE <classngraph_1_1op_1_1PadIE.rst>
	PowerIE <classngraph_1_1op_1_1PowerIE.rst>
	ProposalIE <classngraph_1_1op_1_1ProposalIE.rst>
	RNNCellIE <classngraph_1_1op_1_1RNNCellIE.rst>
	RNNSequenceIE <classngraph_1_1op_1_1RNNSequenceIE.rst>
	ReLUIE <classngraph_1_1op_1_1ReLUIE.rst>
	ResampleV2 <classngraph_1_1op_1_1ResampleV2.rst>
	ScaleShiftIE <classngraph_1_1op_1_1ScaleShiftIE.rst>
	SeluIE <classngraph_1_1op_1_1SeluIE.rst>
	SwishIE <classngraph_1_1op_1_1SwishIE.rst>
	TemporaryReplaceOutputType <classngraph_1_1op_1_1TemporaryReplaceOutputType.rst>
	TileIE <classngraph_1_1op_1_1TileIE.rst>
	TopKIE <classngraph_1_1op_1_1TopKIE.rst>
	TypeRelaxed <classngraph_1_1op_1_1TypeRelaxed.rst>
	TypeRelaxedBase <classngraph_1_1op_1_1TypeRelaxedBase.rst>

Ops used in graph-building.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace op {

	// namespaces

	namespace :ref:`ngraph::op::internal<doxid-namespacengraph_1_1op_1_1internal>`;
	namespace :ref:`ngraph::op::util<doxid-namespacengraph_1_1op_1_1util>`;
		namespace :ref:`ngraph::op::util::detail<doxid-namespacengraph_1_1op_1_1util_1_1detail>`;
		namespace :ref:`ngraph::op::util::error<doxid-namespacengraph_1_1op_1_1util_1_1error>`;
	namespace :ref:`ngraph::op::v0<doxid-namespacengraph_1_1op_1_1v0>`;
	namespace :ref:`ngraph::op::v1<doxid-namespacengraph_1_1op_1_1v1>`;
	namespace :ref:`ngraph::op::v3<doxid-namespacengraph_1_1op_1_1v3>`;
	namespace :ref:`ngraph::op::v4<doxid-namespacengraph_1_1op_1_1v4>`;
	namespace :ref:`ngraph::op::v5<doxid-namespacengraph_1_1op_1_1v5>`;
	namespace :ref:`ngraph::op::v6<doxid-namespacengraph_1_1op_1_1v6>`;
	namespace :ref:`ngraph::op::v7<doxid-namespacengraph_1_1op_1_1v7>`;
	namespace :ref:`ngraph::op::v8<doxid-namespacengraph_1_1op_1_1v8>`;
	namespace :ref:`ngraph::op::v9<doxid-namespacengraph_1_1op_1_1v9>`;

	// typedefs

	typedef :ref:`ov::op::v0::DetectionOutput::Attributes<doxid-structov_1_1op_1_1v0_1_1_detection_output_1_1_attributes>` :target:`DetectionOutputAttrs<doxid-namespacengraph_1_1op_1a6b495dc76d75ee3962694caf87698e9b>`;
	typedef :ref:`ov::op::v0::PriorBox::Attributes<doxid-structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes>` :target:`PriorBoxAttrs<doxid-namespacengraph_1_1op_1a0c1edeb2380c863deb678ec3e66b8219>`;
	typedef :ref:`ov::op::v0::PriorBoxClustered::Attributes<doxid-structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes>` :target:`PriorBoxClusteredAttrs<doxid-namespacengraph_1_1op_1aace968ed86791f8a1fdd72ca869c5ae0>`;
	typedef :ref:`ov::op::v0::Proposal::Attributes<doxid-structov_1_1op_1_1v0_1_1_proposal_1_1_attributes>` :target:`ProposalAttrs<doxid-namespacengraph_1_1op_1a4358e1e5587270d7e246c6a9c90b1c51>`;

	// structs

	struct :ref:`InterpolateIEAttrs<doxid-structngraph_1_1op_1_1_interpolate_i_e_attrs>`;
	struct :ref:`ResampleIEAttrs<doxid-structngraph_1_1op_1_1_resample_i_e_attrs>`;

	// classes

	class :ref:`ConvolutionIE<doxid-classngraph_1_1op_1_1_convolution_i_e>`;
	class :ref:`CropIE<doxid-classngraph_1_1op_1_1_crop_i_e>`;
	class :ref:`DeconvolutionIE<doxid-classngraph_1_1op_1_1_deconvolution_i_e>`;
	class :ref:`Eltwise<doxid-classngraph_1_1op_1_1_eltwise>`;
	class :ref:`FullyConnected<doxid-classngraph_1_1op_1_1_fully_connected>`;
	class :ref:`GRUCellIE<doxid-classngraph_1_1op_1_1_g_r_u_cell_i_e>`;
	class :ref:`GRUSequenceIE<doxid-classngraph_1_1op_1_1_g_r_u_sequence_i_e>`;
	class :ref:`GatherIE<doxid-classngraph_1_1op_1_1_gather_i_e>`;
	class :ref:`GatherTreeIE<doxid-classngraph_1_1op_1_1_gather_tree_i_e>`;
	class :ref:`HardSigmoid_IE<doxid-classngraph_1_1op_1_1_hard_sigmoid___i_e>`;
	class :ref:`Interp<doxid-classngraph_1_1op_1_1_interp>`;
	class :ref:`LRN_IE<doxid-classngraph_1_1op_1_1_l_r_n___i_e>`;
	class :ref:`LSTMCellIE<doxid-classngraph_1_1op_1_1_l_s_t_m_cell_i_e>`;
	class :ref:`LSTMSequenceIE<doxid-classngraph_1_1op_1_1_l_s_t_m_sequence_i_e>`;
	class :ref:`NonMaxSuppressionIE<doxid-classngraph_1_1op_1_1_non_max_suppression_i_e>`;
	class :ref:`NonMaxSuppressionIE2<doxid-classngraph_1_1op_1_1_non_max_suppression_i_e2>`;
	class :ref:`NonMaxSuppressionIE3<doxid-classngraph_1_1op_1_1_non_max_suppression_i_e3>`;
	class :ref:`NormalizeIE<doxid-classngraph_1_1op_1_1_normalize_i_e>`;
	class :ref:`OneHotIE<doxid-classngraph_1_1op_1_1_one_hot_i_e>`;
	class :ref:`PadIE<doxid-classngraph_1_1op_1_1_pad_i_e>`;
	class :ref:`PowerIE<doxid-classngraph_1_1op_1_1_power_i_e>`;
	class :ref:`ProposalIE<doxid-classngraph_1_1op_1_1_proposal_i_e>`;
	class :ref:`RNNCellIE<doxid-classngraph_1_1op_1_1_r_n_n_cell_i_e>`;
	class :ref:`RNNSequenceIE<doxid-classngraph_1_1op_1_1_r_n_n_sequence_i_e>`;
	class :ref:`ReLUIE<doxid-classngraph_1_1op_1_1_re_l_u_i_e>`;
	class :ref:`ResampleV2<doxid-classngraph_1_1op_1_1_resample_v2>`;
	class :ref:`ScaleShiftIE<doxid-classngraph_1_1op_1_1_scale_shift_i_e>`;
	class :ref:`SeluIE<doxid-classngraph_1_1op_1_1_selu_i_e>`;
	class :ref:`SwishIE<doxid-classngraph_1_1op_1_1_swish_i_e>`;
	class :ref:`TemporaryReplaceOutputType<doxid-classngraph_1_1op_1_1_temporary_replace_output_type>`;
	class :ref:`TileIE<doxid-classngraph_1_1op_1_1_tile_i_e>`;
	class :ref:`TopKIE<doxid-classngraph_1_1op_1_1_top_k_i_e>`;
	template <typename BaseOp>
	class :ref:`TypeRelaxed<doxid-classngraph_1_1op_1_1_type_relaxed>`;
	class :ref:`TypeRelaxedBase<doxid-classngraph_1_1op_1_1_type_relaxed_base>`;

	} // namespace op
