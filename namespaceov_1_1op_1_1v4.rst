.. index:: pair: namespace; ov::op::v4
.. _doxid-namespaceov_1_1op_1_1v4:

namespace ov::op::v4
====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v4 {

	// classes

	class :ref:`CTCLoss<doxid-classov_1_1op_1_1v4_1_1_c_t_c_loss>`;
	class :ref:`HSwish<doxid-classov_1_1op_1_1v4_1_1_h_swish>`;
	class :ref:`Interpolate<doxid-classov_1_1op_1_1v4_1_1_interpolate>`;
	class :ref:`LSTMCell<doxid-classov_1_1op_1_1v4_1_1_l_s_t_m_cell>`;
	class :ref:`Mish<doxid-classov_1_1op_1_1v4_1_1_mish>`;
	class :ref:`NonMaxSuppression<doxid-classov_1_1op_1_1v4_1_1_non_max_suppression>`;
	class :ref:`Proposal<doxid-classov_1_1op_1_1v4_1_1_proposal>`;
	class :ref:`Range<doxid-classov_1_1op_1_1v4_1_1_range>`;
	class :ref:`ReduceL1<doxid-classov_1_1op_1_1v4_1_1_reduce_l1>`;
	class :ref:`ReduceL2<doxid-classov_1_1op_1_1v4_1_1_reduce_l2>`;
	class :ref:`SoftPlus<doxid-classov_1_1op_1_1v4_1_1_soft_plus>`;
	class :ref:`Swish<doxid-classov_1_1op_1_1v4_1_1_swish>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v4_1a62e957649fa44b204f3b36d56c9214b5>`(
		const :ref:`CTCLoss<doxid-classov_1_1op_1_1v4_1_1_c_t_c_loss>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <typename T>
	void :target:`correct_pads_attr<doxid-namespaceov_1_1op_1_1v4_1a9f2fb9dca2cd86ef8c4e9343ea4fd34f>`(
		const :ref:`Interpolate<doxid-classov_1_1op_1_1v4_1_1_interpolate>` \* op,
		std::vector<size_t>& pads_begin,
		std::vector<size_t>& pads_end,
		const std::vector<T>& input_shapes
		);

	int64_t :target:`multiply_bound_and_scale<doxid-namespaceov_1_1op_1_1v4_1a5668cf4e3c10fbbfa036aafc5eb7d906>`(int64_t bound, float scale);

	template <typename T>
	void :target:`infer_using_scales<doxid-namespaceov_1_1op_1_1v4_1aeb4ff8a5aeec02d47b192fb7435a3da9>`(
		T& output_shape,
		const std::vector<int64_t>& axes,
		const std::vector<float>& scales
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v4_1add7640bb7b9d1ddaf09c948a9b7f544c>`(
		const :ref:`Interpolate<doxid-classov_1_1op_1_1v4_1_1_interpolate>` \* op,
		std::vector<size_t>& pads_begin,
		std::vector<size_t>& pads_end,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v4_1a5567099d0056aed53da813a5c2dbca9c>`(
		const :ref:`LSTMCell<doxid-classov_1_1op_1_1v4_1_1_l_s_t_m_cell>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v4_1a3873ce1949ade731d8d907634c75192e>`(
		const :ref:`ov::op::v4::Proposal<doxid-classov_1_1op_1_1v4_1_1_proposal>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v4_1a34074a438035202dd2aeee273b7b0b02>`(
		const :ref:`Range<doxid-classov_1_1op_1_1v4_1_1_range>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	} // namespace v4
