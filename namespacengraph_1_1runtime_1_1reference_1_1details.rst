.. index:: pair: namespace; ngraph::runtime::reference::details
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1details:

namespace ngraph::runtime::reference::details
=============================================

.. toctree::
	:hidden:

	IsRandomAccessIt <structngraph_1_1runtime_1_1reference_1_1details_1_1IsRandomAccessIt.rst>
	ProposalBox <structngraph_1_1runtime_1_1reference_1_1details_1_1ProposalBox.rst>
	from_iterator <structngraph_1_1runtime_1_1reference_1_1details_1_1from_iterator.rst>
	is_complete <structngraph_1_1runtime_1_1reference_1_1details_1_1is_complete.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace details {

	// typedefs

	typedef typename std::enable_if<check, bool>::type :target:`Required<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1ab3a4d565c7c9528f2fe65436d715f2fa>`;
	typedef void :target:`void_t<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1aabd6e7a6a0b6e2854f80d7751aa882ea>`;

	// structs

	template <typename It>
	struct :ref:`IsRandomAccessIt<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_is_random_access_it>`;
	template <typename T>
	struct :ref:`ProposalBox<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_proposal_box>`;
	template <typename It>
	struct :ref:`from_iterator<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1from__iterator>`;
	template <typename, typename = size_t>
	struct :ref:`is_complete<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1is__complete>`;
	template <typename T>
	struct :ref:`is_complete<T, decltype(sizeof(T))><doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1is__complete_3_01_t_00_01decltype_07sizeof_07_t_08_08_4>`;

	// global functions

	uint8_t :target:`extract_bit<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a05790341b0413ea6cef789026956ae85>`(uint8_t val, uint8_t bit);

	template <typename T>
	bool :target:`xnor<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1acf5594fba538b5f1ea00ce4bbb710c31>`(T a, T b);

	template <typename T_IN, typename T_F>
	void :target:`binary_convolve_3D_channels<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a5d2f9c48e187322cbc73b0673eb56b44>`(
		const ConvolutionParams& p,
		const T_IN \* batch,
		const :ref:`Shape<doxid-classov_1_1_shape>`& batch_shape,
		const T_F \* filter,
		const :ref:`Shape<doxid-classov_1_1_shape>`& filter_shape,
		T_IN \*& out,
		const float pad_value
		);

	template <typename Iterator>
	std::vector<size_t> :target:`get_indices_offsets<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a54397e23f1de104fabafb103935dfd7b>`(
		const Iterator beg,
		const Iterator end,
		size_t last_slice_size
		);

	template <typename T>
	void :target:`dot<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a1ad87b531ff62a74a53dd4daeffc9d15>`(
		const T \* arg0,
		const T \* arg1,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg0_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& arg1_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape
		);

	std::vector<size_t> :target:`get_transpose_order<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1adba97cdd533364d35009ef19bb375d88>`(const :ref:`Shape<doxid-classov_1_1_shape>`& input_shape);

	std::vector<float> :target:`generate_anchors<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a54791209c7b2958015fc508e50b6da35>`(
		const :ref:`op::ProposalAttrs<doxid-namespacengraph_1_1op_1a4358e1e5587270d7e246c6a9c90b1c51>`& attrs,
		const unsigned int anchor_count
		);

	template <typename T>
	static void :target:`enumerate_proposals<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a2fff17f47d8fca540e069a7b3196f284>`(
		const T \* bottom4d,
		const T \* d_anchor4d,
		const float \* anchors,
		std::vector<:ref:`ProposalBox<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_proposal_box>`<T>>& proposals,
		const unsigned int num_anchors,
		const unsigned int bottom_H,
		const unsigned int bottom_W,
		const float img_H,
		const float img_W,
		const float min_box_H,
		const float min_box_W,
		const int feat_stride,
		const float box_coordinate_scale,
		const float box_size_scale,
		float coordinates_offset,
		bool initial_clip,
		bool swap_xy,
		bool clip_before_nms
		);

	template <typename T>
	static void :target:`nms<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1adacd7d7bc81f5c800fc57332c9983892>`(
		const int num_boxes,
		const std::vector<:ref:`ProposalBox<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_proposal_box>`<T>>& proposals,
		std::vector<unsigned int>& index_out,
		int& num_out,
		const int base_index,
		const float nms_thresh,
		const int max_num_out,
		T coordinates_offset
		);

	template <typename T>
	static void :target:`retrieve_rois<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1abaa20960589c1898c021de7da0500722>`(
		const int num_rois,
		const int item_index,
		const int num_proposals,
		const std::vector<:ref:`ProposalBox<doxid-structngraph_1_1runtime_1_1reference_1_1details_1_1_proposal_box>`<T>>& proposals,
		const std::vector<unsigned int>& roi_indices,
		T \* rois,
		int post_nms_topn_,
		bool normalize,
		float img_h,
		float img_w,
		bool clip_after_nms,
		T \* probs = nullptr
		);

	template <typename T>
	static void :target:`proposal_exec<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a721a52a5d85e3a3ee520bfe11b32e825>`(
		const T \* class_probs,
		const T \* bbox_deltas,
		const T \* image_shape,
		T \* output,
		T \* out_probs,
		const :ref:`Shape<doxid-classov_1_1_shape>`& class_probs_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& bbox_deltas_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& image_shape_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_probs_shape,
		const :ref:`op::ProposalAttrs<doxid-namespacengraph_1_1op_1a4358e1e5587270d7e246c6a9c90b1c51>`& attrs
		);

	template <
		typename T,
		typename std::enable_if<std::is_floating_point<T>::value, bool>::type = true
		>
	bool :target:`is_finite<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1a229db039723ee07fc56666cdbb11eadd>`(T x);

	template <typename T>
	void :ref:`kahan_summation<doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1aea70aea6b490a920c7b5e1f946d64c62>`(
		const T& elem,
		T& compensation,
		T& sum
		);

	} // namespace details
.. _details-namespacengraph_1_1runtime_1_1reference_1_1details:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1details_1aea70aea6b490a920c7b5e1f946d64c62:
.. index:: pair: function; kahan_summation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void kahan_summation(
		const T& elem,
		T& compensation,
		T& sum
		)

Performs one element summation based on Kahan algorithm to significantly reduce the numerical error.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- elem

		- Element to add into the accumulator.

	*
		- compensation

		- Variable that accumulates the error.

	*
		- sum

		- Result of compensated summation.

