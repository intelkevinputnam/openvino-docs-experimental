.. index:: pair: namespace; ov::op::v3
.. _doxid-namespaceov_1_1op_1_1v3:

namespace ov::op::v3
====================

.. toctree::
	:hidden:

	Asinh <classov_1_1op_1_1v3_1_1Asinh.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace v3 {

	// classes

	class :ref:`Acosh<doxid-classov_1_1op_1_1v3_1_1_acosh>`;
	class :ref:`Asinh<doxid-classov_1_1op_1_1v3_1_1_asinh>`;
	class :ref:`Assign<doxid-classov_1_1op_1_1v3_1_1_assign>`;
	class :ref:`Atanh<doxid-classov_1_1op_1_1v3_1_1_atanh>`;
	class :ref:`Broadcast<doxid-classov_1_1op_1_1v3_1_1_broadcast>`;
	class :ref:`Bucketize<doxid-classov_1_1op_1_1v3_1_1_bucketize>`;
	class :ref:`EmbeddingBagOffsetsSum<doxid-classov_1_1op_1_1v3_1_1_embedding_bag_offsets_sum>`;
	class :ref:`EmbeddingBagPackedSum<doxid-classov_1_1op_1_1v3_1_1_embedding_bag_packed_sum>`;
	class :ref:`EmbeddingSegmentsSum<doxid-classov_1_1op_1_1v3_1_1_embedding_segments_sum>`;
	class :ref:`ExtractImagePatches<doxid-classov_1_1op_1_1v3_1_1_extract_image_patches>`;
	class :ref:`GRUCell<doxid-classov_1_1op_1_1v3_1_1_g_r_u_cell>`;
	class :ref:`NonMaxSuppression<doxid-classov_1_1op_1_1v3_1_1_non_max_suppression>`;
	class :ref:`NonZero<doxid-classov_1_1op_1_1v3_1_1_non_zero>`;
	class :ref:`ROIAlign<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align>`;
	class :ref:`ReadValue<doxid-classov_1_1op_1_1v3_1_1_read_value>`;
	class :ref:`ScatterElementsUpdate<doxid-classov_1_1op_1_1v3_1_1_scatter_elements_update>`;
	class :ref:`ScatterNDUpdate<doxid-classov_1_1op_1_1v3_1_1_scatter_n_d_update>`;
	class :ref:`ScatterUpdate<doxid-classov_1_1op_1_1v3_1_1_scatter_update>`;
	class :ref:`ShapeOf<doxid-classov_1_1op_1_1v3_1_1_shape_of>`;
	class :ref:`TopK<doxid-classov_1_1op_1_1v3_1_1_top_k>`;

	// global functions

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1a39314e1c3b31ea2b0012eeb30c1c36a8>`(
		const :ref:`Assign<doxid-classov_1_1op_1_1v3_1_1_assign>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1a0f87063a0aac460e8b1c90c5042f9f75>`(
		const :ref:`ov::op::v3::Broadcast<doxid-classov_1_1op_1_1v3_1_1_broadcast>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1abecc1758d7412ce9dd9aa6657f1814da>`(
		const :ref:`Bucketize<doxid-classov_1_1op_1_1v3_1_1_bucketize>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1a32ae95ce246055476be4f364a58c064d>`(
		const :ref:`EmbeddingSegmentsSum<doxid-classov_1_1op_1_1v3_1_1_embedding_segments_sum>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	int32_t :target:`calc_shape_padding<doxid-namespaceov_1_1op_1_1v3_1a232b789ac49f014fdd2463a50238f18a>`(
		const int32_t input,
		const int32_t rate,
		const int32_t stride,
		const int32_t patch_size,
		const :ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>` type
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1a09c5cebd273ac83d70b1ccddd6ba8318>`(
		const :ref:`ExtractImagePatches<doxid-classov_1_1op_1_1v3_1_1_extract_image_patches>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1a128735d25ba630c37ecd26d671aee7fa>`(
		const :ref:`ReadValue<doxid-classov_1_1op_1_1v3_1_1_read_value>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class OpType, class ShapeType>
	void :target:`infer_roi_align_shape<doxid-namespaceov_1_1op_1_1v3_1af00cea834181be27a28ade3d35ffa569>`(
		const OpType \* op,
		const std::vector<ShapeType>& input_shapes,
		std::vector<ShapeType>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1a4c2774d4325121f5f29a15c3326a0907>`(
		const :ref:`ov::op::v3::ROIAlign<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1_1v3_1aa9c6a83f601740c63433e749a281b0c6>`(
		const :ref:`ScatterElementsUpdate<doxid-classov_1_1op_1_1v3_1_1_scatter_elements_update>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	} // namespace v3
