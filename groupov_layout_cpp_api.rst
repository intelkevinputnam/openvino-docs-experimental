.. index:: pair: group; Layout
.. _doxid-group__ov__layout__cpp__api:

Layout
======

.. toctree::
	:hidden:

	Layout <classov_1_1Layout.rst>

Overview
~~~~~~~~

OpenVINO :ref:`Layout <doxid-classov_1_1_layout>` API to work and configure layouts for :ref:`ov::Model <doxid-classov_1_1_model>` inputs or outputs :ref:`More...<details-group__ov__layout__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`ov::Layout<doxid-classov_1_1_layout>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`ov::layout::has_batch<doxid-group__ov__layout__cpp__api_1gac4ad1b38a5756e524aac263da03de24c>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`ov::layout::batch_idx<doxid-group__ov__layout__cpp__api_1gae57e9fcaa7d8eaa7ddbcdfece346bccb>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`ov::layout::has_channels<doxid-group__ov__layout__cpp__api_1gafff6ea3fec4ebb7fd772843feb2cf369>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`ov::layout::channels_idx<doxid-group__ov__layout__cpp__api_1ga4c4a2d4a226d5b264a0f74c6c7839f4f>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`ov::layout::has_depth<doxid-group__ov__layout__cpp__api_1gac31cb65d9378dc73990ee9f93c1f0b01>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`ov::layout::depth_idx<doxid-group__ov__layout__cpp__api_1ga69af957b8f6a69956f38dfa1afc7039a>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`ov::layout::has_height<doxid-group__ov__layout__cpp__api_1gadf2117a34f7195e4b0756303af11995f>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`ov::layout::height_idx<doxid-group__ov__layout__cpp__api_1ga83da0183fe7f811912436ddb4aa4bb28>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool :ref:`ov::layout::has_width<doxid-group__ov__layout__cpp__api_1ga36be840f4a6d4554a556349d52aa4ea3>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t :ref:`ov::layout::width_idx<doxid-group__ov__layout__cpp__api_1ga8730a2b5c3fd24f752c550ee3d07b870>`(const :ref:`Layout<doxid-classov_1_1_layout>`& layout);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void :ref:`ov::layout::set_layout<doxid-group__ov__layout__cpp__api_1ga18464fb8ed029acb5fdc2bb1737358d9>`(
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> output,
		const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ov::Layout<doxid-classov_1_1_layout>` :ref:`ov::layout::get_layout<doxid-group__ov__layout__cpp__api_1ga3d711b0631dfdf8642484998f4981857>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& output);
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ov::Layout<doxid-classov_1_1_layout>` :ref:`ov::layout::get_layout<doxid-group__ov__layout__cpp__api_1gad9a00c376273a51d26f62b6c105072fc>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& output);

.. _details-group__ov__layout__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

OpenVINO :ref:`Layout <doxid-classov_1_1_layout>` API to work and configure layouts for :ref:`ov::Model <doxid-classov_1_1_model>` inputs or outputs

Global Functions
----------------

.. _doxid-group__ov__layout__cpp__api_1gac4ad1b38a5756e524aac263da03de24c:
.. index:: pair: function; has_batch

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool ov::layout::has_batch(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Checks if layout has 'batch' dimension.

.. _doxid-group__ov__layout__cpp__api_1gae57e9fcaa7d8eaa7ddbcdfece346bccb:
.. index:: pair: function; batch_idx

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t ov::layout::batch_idx(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Returns 'batch' dimension index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension doesn't exist.

.. _doxid-group__ov__layout__cpp__api_1gafff6ea3fec4ebb7fd772843feb2cf369:
.. index:: pair: function; has_channels

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool ov::layout::has_channels(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Checks if layout has 'channels' dimension.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension doesn't exist.

.. _doxid-group__ov__layout__cpp__api_1ga4c4a2d4a226d5b264a0f74c6c7839f4f:
.. index:: pair: function; channels_idx

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t ov::layout::channels_idx(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Returns 'channels' dimension index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension doesn't exist.

.. _doxid-group__ov__layout__cpp__api_1gac31cb65d9378dc73990ee9f93c1f0b01:
.. index:: pair: function; has_depth

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool ov::layout::has_depth(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Checks if layout has 'depth' dimension.

.. _doxid-group__ov__layout__cpp__api_1ga69af957b8f6a69956f38dfa1afc7039a:
.. index:: pair: function; depth_idx

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t ov::layout::depth_idx(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Returns 'depth' dimension index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension doesn't exist.

.. _doxid-group__ov__layout__cpp__api_1gadf2117a34f7195e4b0756303af11995f:
.. index:: pair: function; has_height

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool ov::layout::has_height(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Checks if layout has 'height' dimension.

.. _doxid-group__ov__layout__cpp__api_1ga83da0183fe7f811912436ddb4aa4bb28:
.. index:: pair: function; height_idx

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t ov::layout::height_idx(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Returns 'height' dimension index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension doesn't exist.

.. _doxid-group__ov__layout__cpp__api_1ga36be840f4a6d4554a556349d52aa4ea3:
.. index:: pair: function; has_width

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` bool ov::layout::has_width(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Checks if layout has 'width' dimension.

.. _doxid-group__ov__layout__cpp__api_1ga8730a2b5c3fd24f752c550ee3d07b870:
.. index:: pair: function; width_idx

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::int64_t ov::layout::width_idx(const :ref:`Layout<doxid-classov_1_1_layout>`& layout)

Returns 'width' dimension index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension doesn't exist.

.. _doxid-group__ov__layout__cpp__api_1ga18464fb8ed029acb5fdc2bb1737358d9:
.. index:: pair: function; set_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` void ov::layout::set_layout(
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> output,
		const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout
		)

Sets :ref:`Layout <doxid-classov_1_1_layout>` of port.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::Exception <doxid-classov_1_1_exception>`

		- if port is not connected with Result or Parameter

.. _doxid-group__ov__layout__cpp__api_1ga3d711b0631dfdf8642484998f4981857:
.. index:: pair: function; get_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ov::Layout<doxid-classov_1_1_layout>` ov::layout::get_layout(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& output)

Gets :ref:`Layout <doxid-classov_1_1_layout>` of port.



.. rubric:: Returns:

layout from port and empty layout in other case

.. _doxid-group__ov__layout__cpp__api_1gad9a00c376273a51d26f62b6c105072fc:
.. index:: pair: function; get_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`ov::Layout<doxid-classov_1_1_layout>` ov::layout::get_layout(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& output)

Gets :ref:`Layout <doxid-classov_1_1_layout>` of port.



.. rubric:: Returns:

layout from port and empty layout in other case

