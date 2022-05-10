.. index:: pair: namespace; ov::op
.. _doxid-namespaceov_1_1op:

namespace ov::op
================

.. toctree::
	:hidden:

	ShapeInferLSTM <namespaceov_1_1op_1_1ShapeInferLSTM.rst>
	ShapeInferRange <namespaceov_1_1op_1_1ShapeInferRange.rst>
	util <namespaceov_1_1op_1_1util.rst>
	v0 <namespaceov_1_1op_1_1v0.rst>
	v1 <namespaceov_1_1op_1_1v1.rst>
	v3 <namespaceov_1_1op_1_1v3.rst>
	v4 <namespaceov_1_1op_1_1v4.rst>
	v5 <namespaceov_1_1op_1_1v5.rst>
	v6 <namespaceov_1_1op_1_1v6.rst>
	v7 <namespaceov_1_1op_1_1v7.rst>
	v8 <namespaceov_1_1op_1_1v8.rst>
	v9 <namespaceov_1_1op_1_1v9.rst>
	AutoBroadcastType <enumov_1_1op_1_1AutoBroadcastType.rst>
	BroadcastType <enumov_1_1op_1_1BroadcastType.rst>
	EpsMode <enumov_1_1op_1_1EpsMode.rst>
	GeluApproximationMode <enumov_1_1op_1_1GeluApproximationMode.rst>
	LSTMWeightsFormat <enumov_1_1op_1_1LSTMWeightsFormat.rst>
	MVNEpsMode <enumov_1_1op_1_1MVNEpsMode.rst>
	PadMode <enumov_1_1op_1_1PadMode.rst>
	PadType <enumov_1_1op_1_1PadType.rst>
	RecurrentSequenceDirection <enumov_1_1op_1_1RecurrentSequenceDirection.rst>
	RoundingType <enumov_1_1op_1_1RoundingType.rst>
	TopKMode <enumov_1_1op_1_1TopKMode.rst>
	TopKSortType <enumov_1_1op_1_1TopKSortType.rst>
	AutoBroadcastSpec <structov_1_1op_1_1AutoBroadcastSpec.rst>
	BroadcastModeSpec <structov_1_1op_1_1BroadcastModeSpec.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace op {

	// namespaces

	namespace :ref:`ov::op::ShapeInferLSTM<doxid-namespaceov_1_1op_1_1_shape_infer_l_s_t_m>`;
	namespace :ref:`ov::op::ShapeInferRange<doxid-namespaceov_1_1op_1_1_shape_infer_range>`;
	namespace :ref:`ov::op::util<doxid-namespaceov_1_1op_1_1util>`;
		namespace :ref:`ov::op::util::detail<doxid-namespaceov_1_1op_1_1util_1_1detail>`;
		namespace :ref:`ov::op::util::error<doxid-namespaceov_1_1op_1_1util_1_1error>`;
		namespace :ref:`ov::op::util::rfft_common_validation<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation>`;
	namespace :ref:`ov::op::v0<doxid-namespaceov_1_1op_1_1v0>`;
	namespace :ref:`ov::op::v1<doxid-namespaceov_1_1op_1_1v1>`;
	namespace :ref:`ov::op::v3<doxid-namespaceov_1_1op_1_1v3>`;
	namespace :ref:`ov::op::v4<doxid-namespaceov_1_1op_1_1v4>`;
	namespace :ref:`ov::op::v5<doxid-namespaceov_1_1op_1_1v5>`;
	namespace :ref:`ov::op::v6<doxid-namespaceov_1_1op_1_1v6>`;
	namespace :ref:`ov::op::v7<doxid-namespaceov_1_1op_1_1v7>`;
	namespace :ref:`ov::op::v8<doxid-namespaceov_1_1op_1_1v8>`;
	namespace :ref:`ov::op::v9<doxid-namespaceov_1_1op_1_1v9>`;

	// enums

	enum :ref:`AutoBroadcastType<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>`;
	enum :ref:`BroadcastType<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>`;
	enum :ref:`EpsMode<doxid-namespaceov_1_1op_1abde68b9f95937807257f2be0a05165b3>`;
	enum :ref:`GeluApproximationMode<doxid-namespaceov_1_1op_1a1ab40a6efb6720925e3d75890dd87d63>`;
	enum :ref:`LSTMWeightsFormat<doxid-namespaceov_1_1op_1a6efe5db5f325a937a6662cd2b66e1437>`;
	enum :ref:`MVNEpsMode<doxid-namespaceov_1_1op_1a2fa6abf51a614b1b7f65f6bcafa88d99>`;
	enum :ref:`PadMode<doxid-namespaceov_1_1op_1aff39ecf8a8a3110216bfe131cc8b9ae0>`;
	enum :ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>`;
	enum :ref:`RecurrentSequenceDirection<doxid-namespaceov_1_1op_1a9ea79d465e912e768d0ac8fe24d6f0cc>`;
	enum :ref:`RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>`;
	enum :ref:`TopKMode<doxid-namespaceov_1_1op_1a1b4a5e596b7b28cc8a8746fda9ee1a97>`;
	enum :ref:`TopKSortType<doxid-namespaceov_1_1op_1adb25710a58c013466ba8b371156e09cb>`;

	// structs

	struct :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`;
	struct :ref:`BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec>`;

	// classes

	class :ref:`Op<doxid-classov_1_1op_1_1_op>`;
	class :ref:`Sink<doxid-classov_1_1op_1_1_sink>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a887fe0c89ea42dfd924d8d3be7fe95a1>` (
		std::ostream& s,
		const :ref:`GeluApproximationMode<doxid-namespaceov_1_1op_1a1ab40a6efb6720925e3d75890dd87d63>`& type
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a285f51890b7394794d8bc2b4cec64999>` (std::ostream& s, const :ref:`MVNEpsMode<doxid-namespaceov_1_1op_1a2fa6abf51a614b1b7f65f6bcafa88d99>`& type);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a136d8477a8a29287ac9cff35587b9728>` (std::ostream& s, const :ref:`PadMode<doxid-namespaceov_1_1op_1aff39ecf8a8a3110216bfe131cc8b9ae0>`& type);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a2d892910c5c3914ddc60823ab223daad>` (std::ostream& s, const :ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>`& type);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a1335a5f30968c705d0e5f56ee6998494>` (std::ostream& s, const :ref:`RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>`& type);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a1c3343dfcdae1ba339a5481ecfa73fdd>` (
		std::ostream& s,
		const :ref:`AutoBroadcastType<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>`& type
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a8086151c8d67fd1cc901abc3d248e92b>` (
		std::ostream& s,
		const :ref:`BroadcastType<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>`& type
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a18f79cdb738d0816020bcc399855e991>` (std::ostream& s, const :ref:`EpsMode<doxid-namespaceov_1_1op_1abde68b9f95937807257f2be0a05165b3>`& type);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a695569b92e32d4715ddf88f08a3fbe7b>` (std::ostream& s, const :ref:`TopKSortType<doxid-namespaceov_1_1op_1adb25710a58c013466ba8b371156e09cb>`& type);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1af33d30e1883abbb09e1bd8c5303d18e2>` (std::ostream& s, const :ref:`TopKMode<doxid-namespaceov_1_1op_1a1b4a5e596b7b28cc8a8746fda9ee1a97>`& type);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1op_1a4fed781990d3463c625581ed7b0dad2b>` (
		std::ostream& s,
		const :ref:`RecurrentSequenceDirection<doxid-namespaceov_1_1op_1a9ea79d465e912e768d0ac8fe24d6f0cc>`& direction
		);

	template <class T>
	void :target:`shape_infer<doxid-namespaceov_1_1op_1a23a88356b96f0f7916cca740b62976f5>`(
		const :ref:`ov::op::v9::Eye<doxid-classov_1_1op_1_1v9_1_1_eye>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<T>& output_shapes,
		const std::map<size_t, std::shared_ptr<:ref:`ngraph::runtime::HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`>>& constant_data = {}
		);

	template <class OpType, class ShapeType>
	void :target:`read_value_shape_infer<doxid-namespaceov_1_1op_1accc90ce73e51bb317c4607938a4d0fa5>`(
		const OpType \* op,
		const std::vector<ShapeType>& input_shapes,
		std::vector<ShapeType>& output_shapes
		);

	} // namespace op
