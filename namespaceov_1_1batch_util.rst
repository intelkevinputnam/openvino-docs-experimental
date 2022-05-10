.. index:: pair: namespace; ov::batch_util
.. _doxid-namespaceov_1_1batch__util:

namespace ov::batch_util
========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace batch_util {

	// global functions

	void :target:`mark_batch<doxid-namespaceov_1_1batch__util_1a6d27eb30ea08f802119116b05fc928e0>`(
		const std::shared_ptr<ov::opset1::Parameter>& parameter,
		:ref:`P2Btype<doxid-dimension__tracking_8hpp_1a186714ea70622d6cbc526d6f9bc65d24>`& map,
		const std::unordered_set<size_t>& batches
		);

	void :target:`mark_no_batch<doxid-namespaceov_1_1batch__util_1a9e96f673dba5cf562f7592756dec8823>`(
		const std::shared_ptr<ov::opset1::Parameter>& parameter,
		:ref:`P2Btype<doxid-dimension__tracking_8hpp_1a186714ea70622d6cbc526d6f9bc65d24>`& map
		);

	void :target:`mark_layout_independent_batch<doxid-namespaceov_1_1batch__util_1aa00bd9a8cc3399856f82089ab2554232>`(
		const std::shared_ptr<ov::opset1::Parameter>& parameter,
		const std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>& result,
		:ref:`P2Btype<doxid-dimension__tracking_8hpp_1a186714ea70622d6cbc526d6f9bc65d24>`& map
		);

	void :target:`mark_with_unique_dimension_labels<doxid-namespaceov_1_1batch__util_1a95a2c6e2308ebf36d05a1a105276ed65>`(
		const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& m,
		const ov::DimensionTracker& dt
		);

	void :target:`restore_original_dimensions<doxid-namespaceov_1_1batch__util_1aa3371e574fb29cff10d892d215885ccd>`(
		const std::map<std::shared_ptr<ov::opset1::Parameter>, :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& parameter_to_shape,
		bool leave_batch_dynamic = true
		);

	bool :target:`check_batch_tracks_through_all_the_nodes<doxid-namespaceov_1_1batch__util_1aa9b747d28eb1474fdb1534f9dff14611>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);
	:ref:`P2Btype<doxid-dimension__tracking_8hpp_1a186714ea70622d6cbc526d6f9bc65d24>` :target:`find_batch<doxid-namespaceov_1_1batch__util_1a76fafd8528ada11bb59cdee051409922>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);
	bool :target:`detach_detection_output<doxid-namespaceov_1_1batch__util_1a02d9b2275cabd60bc3f21d20f07ab60f>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& f);

	} // namespace batch_util
