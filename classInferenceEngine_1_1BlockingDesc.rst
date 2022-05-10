.. index:: pair: class; InferenceEngine::BlockingDesc
.. _doxid-class_inference_engine_1_1_blocking_desc:

class InferenceEngine::BlockingDesc
===================================



Overview
~~~~~~~~

This class describes blocking layouts. :ref:`More...<details-class_inference_engine_1_1_blocking_desc>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layouts.h>
	
	class BlockingDesc
	{
	public:
		// construction
	
		:ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc_1aec3ce2473ed2db62190054fce13bcfd3>`();
		:ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc_1aec94d1a548354fc33c25664788637728>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout);
		:ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc_1a1385a1484ae83b2c5b9524646e945741>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims, const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order);
	
		:ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc_1a9a6b29ca7991bbe9c4c2defa14bd3ffe>`(
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order,
			size_t offset
			);
	
		:ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc_1a22f72e65f3381275ab9e7e571a1a65bf>`(
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order,
			size_t offset,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dimOffsets
			);
	
		:ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc_1a96a4fc9e95a2cc405acacf3a48180c68>`(
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order,
			size_t offset,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dimOffsets,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& strides
			);

		// methods
	
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getBlockDims<doxid-class_inference_engine_1_1_blocking_desc_1a0503cfbaacc92028773b1ce81cd50389>`() const;
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getOrder<doxid-class_inference_engine_1_1_blocking_desc_1aeb905247511bf47272629c1d9bc50039>`() const;
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getOffsetPaddingToData<doxid-class_inference_engine_1_1_blocking_desc_1ad839d5e1db7a2a80e8a607620481bc35>`() const;
		size_t :ref:`getOffsetPadding<doxid-class_inference_engine_1_1_blocking_desc_1a026cb0da5aa19450274fbe3c12ca08c6>`() const;
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getStrides<doxid-class_inference_engine_1_1_blocking_desc_1a1af204349eed6449cb233041a2089330>`() const;
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_blocking_desc_1ae313fd34b14b1eaede41c1663585e4ee>` (const BlockingDesc& rhs) const;
		bool :ref:`operator !=<doxid-class_inference_engine_1_1_blocking_desc_1a6f8e1fb7130fd89c686181a9d3a4c284>` (const BlockingDesc& rhs) const;
	};
.. _details-class_inference_engine_1_1_blocking_desc:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class describes blocking layouts.

Construction
------------

.. _doxid-class_inference_engine_1_1_blocking_desc_1aec3ce2473ed2db62190054fce13bcfd3:
.. index:: pair: function; BlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BlockingDesc()

The default constructor which creates empty blocking descriptor.

.. _doxid-class_inference_engine_1_1_blocking_desc_1aec94d1a548354fc33c25664788637728:
.. index:: pair: function; BlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BlockingDesc(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout)

The constructor which allows to create blocking descriptors for standard layouts.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- real dimensions

	*
		- layout

		- memory layout

.. _doxid-class_inference_engine_1_1_blocking_desc_1a1385a1484ae83b2c5b9524646e945741:
.. index:: pair: function; BlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BlockingDesc(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims, const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order)

The constructor allows to create blocking descriptors for blocked memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blocked_dims

		- blocked dimensions

	*
		- order

		- the order of dimensions

.. _doxid-class_inference_engine_1_1_blocking_desc_1a9a6b29ca7991bbe9c4c2defa14bd3ffe:
.. index:: pair: function; BlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BlockingDesc(
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order,
		size_t offset
		)

The constructor allows to create blocking descriptors for blocked memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blocked_dims

		- blocked dimensions

	*
		- order

		- the order of dimensions

	*
		- offset

		- offset to the current memory block

.. _doxid-class_inference_engine_1_1_blocking_desc_1a22f72e65f3381275ab9e7e571a1a65bf:
.. index:: pair: function; BlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BlockingDesc(
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order,
		size_t offset,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dimOffsets
		)

The constructor allows to create blocking descriptors for blocked memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blocked_dims

		- blocked dimensions

	*
		- order

		- the order of dimensions

	*
		- offset

		- offset to the current memory block

	*
		- dimOffsets

		- per-dimension offset from the padding to actual data,

.. _doxid-class_inference_engine_1_1_blocking_desc_1a96a4fc9e95a2cc405acacf3a48180c68:
.. index:: pair: function; BlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BlockingDesc(
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& blocked_dims,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& order,
		size_t offset,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dimOffsets,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& strides
		)

The constructor allows to create blocking descriptors for blocked memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blocked_dims

		- blocked dimensions

	*
		- order

		- the order of dimensions

	*
		- offset

		- offset to the current memory block

	*
		- dimOffsets

		- per-dimension offset from the padding to actual data,

	*
		- strides

		- strides for each dimension

Methods
-------

.. _doxid-class_inference_engine_1_1_blocking_desc_1a0503cfbaacc92028773b1ce81cd50389:
.. index:: pair: function; getBlockDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getBlockDims() const

Returns the blocked dimensions vector.



.. rubric:: Returns:

blocked dimensions

.. _doxid-class_inference_engine_1_1_blocking_desc_1aeb905247511bf47272629c1d9bc50039:
.. index:: pair: function; getOrder

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getOrder() const

Returns the vector of order.



.. rubric:: Returns:

order of dimensions

.. _doxid-class_inference_engine_1_1_blocking_desc_1ad839d5e1db7a2a80e8a607620481bc35:
.. index:: pair: function; getOffsetPaddingToData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getOffsetPaddingToData() const

Returns the per-dimension offset vector.



.. rubric:: Returns:

offsets in elements

.. _doxid-class_inference_engine_1_1_blocking_desc_1a026cb0da5aa19450274fbe3c12ca08c6:
.. index:: pair: function; getOffsetPadding

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getOffsetPadding() const

Returns the offset to the current memory block.



.. rubric:: Returns:

offset in elements

.. _doxid-class_inference_engine_1_1_blocking_desc_1a1af204349eed6449cb233041a2089330:
.. index:: pair: function; getStrides

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getStrides() const

Returns strides for each dimension.



.. rubric:: Returns:

strides in elements

.. _doxid-class_inference_engine_1_1_blocking_desc_1ae313fd34b14b1eaede41c1663585e4ee:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const BlockingDesc& rhs) const

The comparison operator for the :ref:`BlockingDesc <doxid-class_inference_engine_1_1_blocking_desc>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rhs

		- object to compare



.. rubric:: Returns:

true if objects are equal

.. _doxid-class_inference_engine_1_1_blocking_desc_1a6f8e1fb7130fd89c686181a9d3a4c284:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const BlockingDesc& rhs) const

The comparison operator for the :ref:`BlockingDesc <doxid-class_inference_engine_1_1_blocking_desc>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rhs

		- object to compare



.. rubric:: Returns:

true if objects aren't equal


