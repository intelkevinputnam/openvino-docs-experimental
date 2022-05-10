.. index:: pair: namespace; ov::op::v6
.. _doxid-namespaceov_1_1op_1_1v6:

namespace ov::op::v6
====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v6 {

	// classes

	class :ref:`Assign<doxid-classov_1_1op_1_1v6_1_1_assign>`;
	class :ref:`CTCGreedyDecoderSeqLen<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len>`;
	class :ref:`ExperimentalDetectronDetectionOutput<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_detection_output>`;
	class :ref:`ExperimentalDetectronGenerateProposalsSingleImage<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_generate_proposals_single_image>`;
	class :ref:`ExperimentalDetectronPriorGridGenerator<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_prior_grid_generator>`;
	class :ref:`ExperimentalDetectronROIFeatureExtractor<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_r_o_i_feature_extractor>`;
	class :ref:`ExperimentalDetectronTopKROIs<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_top_k_r_o_is>`;
	class :ref:`GatherElements<doxid-classov_1_1op_1_1v6_1_1_gather_elements>`;
	class :ref:`MVN<doxid-classov_1_1op_1_1v6_1_1_m_v_n>`;
	class :ref:`ReadValue<doxid-classov_1_1op_1_1v6_1_1_read_value>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1aeb4cfa1607db862af1a3f3fc4c89414d>`(
		const :ref:`Assign<doxid-classov_1_1op_1_1v6_1_1_assign>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1a861dde782807fab26e3b28ee8d76fcc9>`(
		const :ref:`CTCGreedyDecoderSeqLen<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1a0b0261c25f5345fdc809dcf52b1907d7>`(
		const :ref:`ExperimentalDetectronDetectionOutput<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_detection_output>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1a3553f71e03529f4961f890ad2e900125>`(
		const :ref:`ExperimentalDetectronGenerateProposalsSingleImage<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_generate_proposals_single_image>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1a549ad40615d8ec5ed48a4a9043d01c92>`(
		const :ref:`ExperimentalDetectronPriorGridGenerator<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_prior_grid_generator>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1a42e282a6c12d33463e3b731ab7e8b631>`(
		const :ref:`ExperimentalDetectronROIFeatureExtractor<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_r_o_i_feature_extractor>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1aaa452c8b4d1914558eb53260308ad1b7>`(
		:ref:`ExperimentalDetectronTopKROIs<doxid-classov_1_1op_1_1v6_1_1_experimental_detectron_top_k_r_o_is>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1a6f4cf75c27e94f9aa3c3fc1dccd6fbf1>`(
		const :ref:`GatherElements<doxid-classov_1_1op_1_1v6_1_1_gather_elements>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v6_1ace625714cbde056709ff1ec7653ab7d2>`(
		const :ref:`ReadValue<doxid-classov_1_1op_1_1v6_1_1_read_value>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	} // namespace v6
