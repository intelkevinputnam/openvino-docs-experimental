.. index:: pair: class; InferenceEngine::TensorDesc
.. _doxid-class_inference_engine_1_1_tensor_desc:

class InferenceEngine::TensorDesc
=================================



Overview
~~~~~~~~

This class defines Tensor description. :ref:`More...<details-class_inference_engine_1_1_tensor_desc>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layouts.h>
	
	class TensorDesc
	{
	public:
		// construction
	
		:ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc_1a0b0b4315449c446c83883797a9caba8e>`(
			const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision,
			const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims,
			const :ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc>`& blockDesc
			);
	
		:ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc_1a5f7c5ff2bbc2426bc1630c7742fa1371>`(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision, const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout);
		:ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc_1a4a5e8d74442f85f4dba492082776cd49>`(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout);
		:ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc_1aad2ed6b2f8aaa60d5354a1b77c73b9d2>`();

		// methods
	
		void :ref:`reshape<doxid-class_inference_engine_1_1_tensor_desc_1a166e977b7416c755f1a7d6496fc04a7f>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout = Layout::ANY);
		void :ref:`reshape<doxid-class_inference_engine_1_1_tensor_desc_1a24c9df0c17f8dc01d9a3de5afb60359f>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, const :ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc>`& blockDesc);
		:ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getDims<doxid-class_inference_engine_1_1_tensor_desc_1aba4c616b6e9ba449da351066dbbf67f6>`();
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getDims<doxid-class_inference_engine_1_1_tensor_desc_1a6a6cdfbac8c8c9d2ee03e23ac53308ac>`() const;
		void :ref:`setDims<doxid-class_inference_engine_1_1_tensor_desc_1a9f6a5c51f2b402d68e5b96e2d2b9c7bf>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims);
		:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` :ref:`getLayout<doxid-class_inference_engine_1_1_tensor_desc_1a15364592fc9e6e5d6ddc82b8a9ec7c64>`() const;
		void :ref:`setLayout<doxid-class_inference_engine_1_1_tensor_desc_1a2a90e6c92d1c48929e0b968243a703ca>`(:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` l);
		const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& :ref:`getPrecision<doxid-class_inference_engine_1_1_tensor_desc_1aecf8293d63866dc29951153478501105>`() const;
		void :ref:`setPrecision<doxid-class_inference_engine_1_1_tensor_desc_1a5f081ecf18e54722d9b701f5d41bafa6>`(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& p);
		const :ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc>`& :ref:`getBlockingDesc<doxid-class_inference_engine_1_1_tensor_desc_1a0086970b9784561b1e6c63d834cf517f>`() const;
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_tensor_desc_1a1fcbcb2b622bfdba06b09a66962fe2ec>` (const TensorDesc& rhs) const;
		bool :ref:`operator !=<doxid-class_inference_engine_1_1_tensor_desc_1ac0efdfa6532d25e4fe144e59f6362b2b>` (const TensorDesc& rhs) const;
		size_t :ref:`offset<doxid-class_inference_engine_1_1_tensor_desc_1a2e972bd9cde8b2b92211ed2c8d6246cb>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& v) const;
		size_t :ref:`offset<doxid-class_inference_engine_1_1_tensor_desc_1ad32d47212c7c23e765af4a26a30a5d88>`(size_t l) const;
		static :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` :ref:`getLayoutByDims<doxid-class_inference_engine_1_1_tensor_desc_1a9d361162ecf211bbb86d2a380a9c8d5f>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims);
		static :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` :ref:`getLayoutByRank<doxid-class_inference_engine_1_1_tensor_desc_1a1a153659995bfa74cfbfda73e6d06938>`(size_t rank);
	};
.. _details-class_inference_engine_1_1_tensor_desc:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class defines Tensor description.

Construction
------------

.. _doxid-class_inference_engine_1_1_tensor_desc_1a0b0b4315449c446c83883797a9caba8e:
.. index:: pair: function; TensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TensorDesc(
		const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision,
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims,
		const :ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc>`& blockDesc
		)

The constructor creates the tensor descriptor using blocking descriptor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- precision

		- memory precision

	*
		- dims

		- memory dimensions

	*
		- blockDesc

		- blocking descriptor

.. _doxid-class_inference_engine_1_1_tensor_desc_1a5f7c5ff2bbc2426bc1630c7742fa1371:
.. index:: pair: function; TensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TensorDesc(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision, const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout)

The constructor creates the tensor descriptor using standard layout.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- precision

		- memory precision

	*
		- dims

		- memory dimensions

	*
		- layout

		- memory layout

.. _doxid-class_inference_engine_1_1_tensor_desc_1a4a5e8d74442f85f4dba492082776cd49:
.. index:: pair: function; TensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TensorDesc(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout)

The constructor creates the empty tensor descriptor with precision and layout.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- precision

		- memory precision

	*
		- layout

		- memory layout

.. _doxid-class_inference_engine_1_1_tensor_desc_1aad2ed6b2f8aaa60d5354a1b77c73b9d2:
.. index:: pair: function; TensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TensorDesc()

The default constructor which creates empty tensor descriptor.

Methods
-------

.. _doxid-class_inference_engine_1_1_tensor_desc_1a166e977b7416c755f1a7d6496fc04a7f:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reshape(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout = Layout::ANY)

Reshapes the tensor descriptor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- new dimensions

	*
		- layout

		- new layout if it is necessary

.. _doxid-class_inference_engine_1_1_tensor_desc_1a24c9df0c17f8dc01d9a3de5afb60359f:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reshape(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, const :ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc>`& blockDesc)

Reshapes the tensor descriptor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- new dimensions

	*
		- blockDesc

		- new blocking descriptor

.. _doxid-class_inference_engine_1_1_tensor_desc_1aba4c616b6e9ba449da351066dbbf67f6:
.. index:: pair: function; getDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getDims()

Returns the vector of dimensions.



.. rubric:: Returns:

dimensions

.. _doxid-class_inference_engine_1_1_tensor_desc_1a6a6cdfbac8c8c9d2ee03e23ac53308ac:
.. index:: pair: function; getDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getDims() const

Returns the constant vector of dimensions.



.. rubric:: Returns:

dimensions

.. _doxid-class_inference_engine_1_1_tensor_desc_1a9f6a5c51f2b402d68e5b96e2d2b9c7bf:
.. index:: pair: function; setDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDims(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims)

Sets dimensions.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- new dimensions

.. _doxid-class_inference_engine_1_1_tensor_desc_1a15364592fc9e6e5d6ddc82b8a9ec7c64:
.. index:: pair: function; getLayout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` getLayout() const

Returns the memory layout.



.. rubric:: Returns:

layout

.. _doxid-class_inference_engine_1_1_tensor_desc_1a2a90e6c92d1c48929e0b968243a703ca:
.. index:: pair: function; setLayout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLayout(:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` l)

Sets the layout.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- l

		- memory layout

.. _doxid-class_inference_engine_1_1_tensor_desc_1aecf8293d63866dc29951153478501105:
.. index:: pair: function; getPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& getPrecision() const

Returns the memory precision.



.. rubric:: Returns:

precision

.. _doxid-class_inference_engine_1_1_tensor_desc_1a5f081ecf18e54722d9b701f5d41bafa6:
.. index:: pair: function; setPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setPrecision(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& p)

Sets the memory precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- precision

.. _doxid-class_inference_engine_1_1_tensor_desc_1a0086970b9784561b1e6c63d834cf517f:
.. index:: pair: function; getBlockingDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`BlockingDesc<doxid-class_inference_engine_1_1_blocking_desc>`& getBlockingDesc() const

Returns the blocking descriptor.



.. rubric:: Returns:

blocking descriptor

.. _doxid-class_inference_engine_1_1_tensor_desc_1a1fcbcb2b622bfdba06b09a66962fe2ec:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const TensorDesc& rhs) const

The comparison operator for the :ref:`TensorDesc <doxid-class_inference_engine_1_1_tensor_desc>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rhs

		- object to compare



.. rubric:: Returns:

true if objects are equal

.. _doxid-class_inference_engine_1_1_tensor_desc_1ac0efdfa6532d25e4fe144e59f6362b2b:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const TensorDesc& rhs) const

The comparison operator for the :ref:`TensorDesc <doxid-class_inference_engine_1_1_tensor_desc>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rhs

		- object to compare



.. rubric:: Returns:

true if objects aren't equal

.. _doxid-class_inference_engine_1_1_tensor_desc_1a2e972bd9cde8b2b92211ed2c8d6246cb:
.. index:: pair: function; offset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t offset(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& v) const

Calculates offset for the vector of dimensions.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- v

		- vector of dimensions



.. rubric:: Returns:

offset

.. _doxid-class_inference_engine_1_1_tensor_desc_1ad32d47212c7c23e765af4a26a30a5d88:
.. index:: pair: function; offset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t offset(size_t l) const

Calculates offset for the local offset.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- l

		- local offset



.. rubric:: Returns:

offset

.. _doxid-class_inference_engine_1_1_tensor_desc_1a9d361162ecf211bbb86d2a380a9c8d5f:
.. index:: pair: function; getLayoutByDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` getLayoutByDims(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims)

Returns the standard layout for dimensions.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- the vector of dimensions



.. rubric:: Returns:

the standard memory layout

.. _doxid-class_inference_engine_1_1_tensor_desc_1a1a153659995bfa74cfbfda73e6d06938:
.. index:: pair: function; getLayoutByRank

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` getLayoutByRank(size_t rank)

Returns the standard layout for the specified tensor rank.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rank

		- of the requested layout



.. rubric:: Returns:

the standard memory layout


