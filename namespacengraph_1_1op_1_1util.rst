.. index:: pair: namespace; ngraph::op::util
.. _doxid-namespacengraph_1_1op_1_1util:

namespace ngraph::op::util
==========================

.. toctree::
	:hidden:

	detail <namespacengraph_1_1op_1_1util_1_1detail.rst>
	error <namespacengraph_1_1op_1_1util_1_1error.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace util {

	// namespaces

	namespace :ref:`ngraph::op::util::detail<doxid-namespacengraph_1_1op_1_1util_1_1detail>`;
	namespace :ref:`ngraph::op::util::error<doxid-namespacengraph_1_1op_1_1util_1_1error>`;

	// typedefs

	typedef :ref:`ov::op::util::MultiSubGraphOp::InputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a750d0d553f8c4d59c87775f8ba335568>` :target:`MultiSubgraphInputDescriptionPtr<doxid-namespacengraph_1_1op_1_1util_1a6dabd10c32c889edc8500684c7f4dd9a>`;
	typedef :ref:`ov::op::util::MultiSubGraphOp::OutputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a53043b195b0af5f636fc35d5c8a501bc>` :target:`MultiSubgraphOutputDescriptionPtr<doxid-namespacengraph_1_1op_1_1util_1a92397c6ed6312aa96a61bf9635246e8e>`;
	typedef :ref:`util::MultiSubGraphOp::MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>` :target:`MultiSubgraphInputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a3d048c2d9f6ca65f578ac3029a0a330e>`;
	typedef :ref:`util::MultiSubGraphOp::MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>` :target:`MultiSubgraphOutputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1aac4ca5b6b097bff1f0ee58648ab3f0e5>`;
	typedef :ref:`util::SubGraphOp::InputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a750d0d553f8c4d59c87775f8ba335568>` :target:`InputDescriptionPtr<doxid-namespacengraph_1_1op_1_1util_1af478d8405ae54d908671de34cbeeeea8>`;
	typedef :ref:`util::SubGraphOp::OutputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a53043b195b0af5f636fc35d5c8a501bc>` :target:`OutputDescriptionPtr<doxid-namespacengraph_1_1op_1_1util_1a0b68aa651565b5024523462e24f73c4d>`;
	typedef std::vector<:ref:`InputDescriptionPtr<doxid-namespacengraph_1_1op_1_1util_1af478d8405ae54d908671de34cbeeeea8>`> :target:`InputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a6f702135e7f8b7a71b2d071ac52f5c0c>`;
	typedef std::vector<:ref:`OutputDescriptionPtr<doxid-namespacengraph_1_1op_1_1util_1a0b68aa651565b5024523462e24f73c4d>`> :target:`OutputDescriptionVector<doxid-namespacengraph_1_1op_1_1util_1a3235964d87a00ce23118b395dc3a7e31>`;

	// global functions

	template <class T>
	bool :target:`normalize_single_value<doxid-namespacengraph_1_1op_1_1util_1a0b4a90f87fd3d3dd178320e7f7b34f30>`(
		std::vector<T> vec,
		float& value
		);

	template <class T>
	bool :target:`has_op_with_type<doxid-namespacengraph_1_1op_1_1util_1ae0346ab850662a6b81157b522d17bfc6>`(const std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& function);

	bool :target:`has_decompression_converts<doxid-namespacengraph_1_1op_1_1util_1aafc0d5c233829c81cb60b40364e95066>`(const std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& function);
	std::string :target:`create_ie_output_name<doxid-namespacengraph_1_1op_1_1util_1a8cde76ab3e2d0d4566567deaebf86168>`(const :ref:`ngraph::Output<doxid-classov_1_1_output>`<const :ref:`ngraph::Node<doxid-classov_1_1_node>`>& output);
	std::string :target:`create_ie_output_name<doxid-namespacengraph_1_1op_1_1util_1a7e8b19d93b7af7b4b0b9a26e60d846e7>`(const :ref:`ngraph::Output<doxid-classov_1_1_output>`<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& output);
	std::string :target:`get_ie_output_name<doxid-namespacengraph_1_1op_1_1util_1af293e8c9af929d11cc5f9e05fdc218da>`(const :ref:`ngraph::Output<doxid-classov_1_1_output>`<const :ref:`ngraph::Node<doxid-classov_1_1_node>`>& output);
	std::string :target:`get_ie_output_name<doxid-namespacengraph_1_1op_1_1util_1a1b842dc4c540fc55c1af4bd0b8e6a355>`(const :ref:`ngraph::Output<doxid-classov_1_1_output>`<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& output);

	template <typename T>
	bool :target:`has_constant_value<doxid-namespacengraph_1_1op_1_1util_1ab15f7731fdf31aa340d25bbdb16cd849>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const T value,
		T epsilon = std::numeric_limits<T>::epsilon()
		);

	template <typename T>
	bool :target:`has_constant_value<doxid-namespacengraph_1_1op_1_1util_1a2b8750cd0fa25a8ad176dc8d9e231e2c>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const std::vector<T> values,
		T epsilon = std::numeric_limits<T>::epsilon()
		);

	bool :target:`get_single_value<doxid-namespacengraph_1_1op_1_1util_1ae912dc111075eb32a43e25026ceddb79>`(
		const std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`>& const_node,
		float& value
		);

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`normalize_constant<doxid-namespacengraph_1_1op_1_1util_1a788bf00617d70d1018e48b77129204a4>`(
		const std::shared_ptr<:ref:`op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`>& constant,
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& shape
		);

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`broadcastTo<doxid-namespacengraph_1_1op_1_1util_1a8a77eb8ba4f8bbb9aa6cc2f7239e9927>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape
		);

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`reshapeTo<doxid-namespacengraph_1_1op_1_1util_1afbbe6494feca2da24efc5b08bdda01dd>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape
		);

	bool :target:`constantIsEqualTo<doxid-namespacengraph_1_1op_1_1util_1a1784a168e65f6647566308fcd7dc2ef4>`(
		const std::shared_ptr<:ref:`ngraph::op::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`>& const_node,
		float value,
		float eps = 1e-5
		);

	bool :target:`has_f16_constants<doxid-namespacengraph_1_1op_1_1util_1a482ae88e5fdfc6d2ec0aa2d839c082aa>`(const std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& function);

	bool :target:`check_for_broadcast<doxid-namespacengraph_1_1op_1_1util_1a6daaa15047440dcad786503837a458a1>`(
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& ref_shape,
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& other_shape
		);

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`activation<doxid-namespacengraph_1_1op_1_1util_1a5c6b1ef042f4677adf6202504bf11221>`(
		const std::string& activation_name,
		const :ref:`ngraph::Output<doxid-classov_1_1_output>`<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& apply_to
		);

	bool :target:`is_seq_len_provided<doxid-namespacengraph_1_1op_1_1util_1a525155a53df37661cf7f2ee81dd9c1c2>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& seq_len_input,
		int64_t max_seq_len
		);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`try_fold_unary_output<doxid-namespacengraph_1_1op_1_1util_1a664a2f59b951213b96dbd6256751002a>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_try_fold<doxid-namespacengraph_1_1op_1_1util_1adefff8820a53a744b9dbed9ae6effc22>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
		const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& inputs
		);

	bool :target:`shapes_equal_except_dynamic_expected_batch<doxid-namespacengraph_1_1op_1_1util_1a1e0b20bb115acc6663ada3f273e0d00c>`(
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& expected,
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& actual
		);

	void :target:`visit_shape_path<doxid-namespacengraph_1_1op_1_1util_1a04a176f40d3650473a199917b7da94c6>`(
		:ref:`ov::Node<doxid-classov_1_1_node>` \* node,
		std::unordered_set<:ref:`ov::Node<doxid-classov_1_1_node>` \*>& visited,
		std::function<void(:ref:`ov::Node<doxid-classov_1_1_node>` \*)> func
		);

	template <typename T, typename... Args>
	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`make_try_fold<doxid-namespacengraph_1_1op_1_1util_1a9a58e4fd134cb86cb277da7f77bf5cbc>`(Args&&... args);

	template <class T>
	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`eltwise_fold<doxid-namespacengraph_1_1op_1_1util_1a3cdf081b9f74d5983566a09d367b6a69>`(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input0,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input1
		);

	std::vector<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :target:`get_node_target_inputs<doxid-namespacengraph_1_1op_1_1util_1ab06f91c3c81502b8b1e4fe1399d67b24>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`node_to_get_shape_value_of_indices_from_shape_node<doxid-namespacengraph_1_1op_1_1util_1a8bf3bf9b12c81e692d653da6547dedc0>`(
		const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& shape_node,
		const std::vector<size_t>& indices
		);

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`node_to_get_shape_value_of_indices_from_shape_source<doxid-namespacengraph_1_1op_1_1util_1a10d1e3a010cd82194bda3a00c45c02c7>`(
		const :ref:`ngraph::Output<doxid-classov_1_1_output>`<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& shape_source,
		const std::vector<size_t>& indices
		);

	bool :target:`is_dequantization_subgraph<doxid-namespacengraph_1_1op_1_1util_1a1559a7a9ef366582d756d6280a4b9fec>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& node);

	bool :target:`can_eliminate_eltwise_node<doxid-namespacengraph_1_1op_1_1util_1ac97ecc92f8a1c8821f81b6e611288094>`(
		const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& eltwise,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& constant,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& non_constant_input
		);

	struct :ref:`NGRAPH_DEPRECATED<doxid-namespacengraph_1_1op_1_1util_1a8d5f3c4c2aa9fa6ee52637f4e95093dd>`("It is obsolete structure and will be removed soon");
	void :ref:`validate_seq_input_rank_dimension<doxid-namespacengraph_1_1op_1_1util_1a15f28122cd88aba29cff1f52d040b9a1>`(const std::vector<:ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`>& input);

	} // namespace util
.. _details-namespacengraph_1_1op_1_1util:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespacengraph_1_1op_1_1util_1a8d5f3c4c2aa9fa6ee52637f4e95093dd:
.. index:: pair: function; NGRAPH_DEPRECATED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	struct NGRAPH_DEPRECATED("It is obsolete structure and will be removed soon")

Base class for annotations added to graph ops.

.. _doxid-namespacengraph_1_1op_1_1util_1a15f28122cd88aba29cff1f52d040b9a1:
.. index:: pair: function; validate_seq_input_rank_dimension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void validate_seq_input_rank_dimension(const std::vector<:ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`>& input)

Validates static rank and dimension for provided input parameters. Additionally input_size dimension is checked for X and W inputs. Applies to LSTM, GRU and RNN Sequences.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input

		- Vector with RNNSequence-like op inputs in following order: X, initial_hidden_state, sequence_lengths, W, R and B.

