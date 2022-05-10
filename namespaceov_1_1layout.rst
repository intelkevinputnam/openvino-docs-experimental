.. index:: pair: namespace; ov::layout
.. _doxid-namespaceov_1_1layout:

namespace ov::layout
====================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace layout {

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`has_batch<doxid-group__ov__layout__cpp__api_1gac4ad1b38a5756e524aac263da03de24c>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`batch_idx<doxid-group__ov__layout__cpp__api_1gae57e9fcaa7d8eaa7ddbcdfece346bccb>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`has_channels<doxid-group__ov__layout__cpp__api_1gafff6ea3fec4ebb7fd772843feb2cf369>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`channels_idx<doxid-group__ov__layout__cpp__api_1ga4c4a2d4a226d5b264a0f74c6c7839f4f>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`has_depth<doxid-group__ov__layout__cpp__api_1gac31cb65d9378dc73990ee9f93c1f0b01>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`depth_idx<doxid-group__ov__layout__cpp__api_1ga69af957b8f6a69956f38dfa1afc7039a>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`has_height<doxid-group__ov__layout__cpp__api_1gadf2117a34f7195e4b0756303af11995f>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`height_idx<doxid-group__ov__layout__cpp__api_1ga83da0183fe7f811912436ddb4aa4bb28>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`has_width<doxid-group__ov__layout__cpp__api_1ga36be840f4a6d4554a556349d52aa4ea3>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`width_idx<doxid-group__ov__layout__cpp__api_1ga8730a2b5c3fd24f752c550ee3d07b870>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void :ref:`set_layout<doxid-group__ov__layout__cpp__api_1ga18464fb8ed029acb5fdc2bb1737358d9>`(
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> output,
		const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ov::Layout<doxid-classov_1_1_layout>` :ref:`get_layout<doxid-group__ov__layout__cpp__api_1ga3d711b0631dfdf8642484998f4981857>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& output);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ov::Layout<doxid-classov_1_1_layout>` :ref:`get_layout<doxid-group__ov__layout__cpp__api_1gad9a00c376273a51d26f62b6c105072fc>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& output);

	} // namespace layout
