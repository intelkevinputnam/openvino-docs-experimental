.. index:: pair: class; InferenceEngine::Data
.. _doxid-class_inference_engine_1_1_data:

class InferenceEngine::Data
===========================



Overview
~~~~~~~~

This class represents the main :ref:`Data <doxid-class_inference_engine_1_1_data>` representation node. :ref:`More...<details-class_inference_engine_1_1_data>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_data.h>
	
	class Data
	{
	public:
		// construction
	
		:ref:`Data<doxid-class_inference_engine_1_1_data_1ae1caca206b49e0a12d910b411b3b21bf>`(const std::string& name, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` _precision, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout = :ref:`NCHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ad6021da38189a289671c55a105a5ffbf>`);
		:ref:`Data<doxid-class_inference_engine_1_1_data_1a35d33c241c6bc1b0cf756fe94fc9e77e>`(const std::string& name, const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc);
		:ref:`Data<doxid-class_inference_engine_1_1_data_1a3e0f1f540578fcb32a31182e5b35f63d>`(const Data& data);

		// methods
	
		Data& :ref:`operator =<doxid-class_inference_engine_1_1_data_1a7147b1956712cbf05aa606769e926ba0>` (const Data& data);
		bool :ref:`isInitialized<doxid-class_inference_engine_1_1_data_1ae306efbe9612f9908fa2e3bf581b0607>`() const;
		void :ref:`setDims<doxid-class_inference_engine_1_1_data_1ae04e2471c0bb9052ebc240ecf4452c48>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& a_dims);
		void :ref:`setLayout<doxid-class_inference_engine_1_1_data_1a141c32d0ccd90173289a86e860035edc>`(:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout);
		void :ref:`reshape<doxid-class_inference_engine_1_1_data_1a2292c0006218a73fd5c5f47f62e2d746>`(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout);
		void :ref:`reshape<doxid-class_inference_engine_1_1_data_1abaf4dede294e598b7e8c5f1822ce860f>`(const std::initializer_list<size_t>& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout);
		:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` :ref:`getLayout<doxid-class_inference_engine_1_1_data_1a21f0e64bac899e582ae53bb724256cec>`() const;
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& :ref:`getTensorDesc<doxid-class_inference_engine_1_1_data_1a945094e6ff29ea0bbcb5fcbe2ef5d4bb>`() const;
		const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& :ref:`getPrecision<doxid-class_inference_engine_1_1_data_1a385ca58fa66dd27a573b00bb3fbb6909>`() const;
		void :ref:`setPrecision<doxid-class_inference_engine_1_1_data_1ac2fb64fdb6f5891c946a9b6200fc8a3e>`(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision);
		const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& :ref:`getDims<doxid-class_inference_engine_1_1_data_1afb164ba11a7d23143f0fe56620e3e1ad>`() const;
		const std::string& :ref:`getName<doxid-class_inference_engine_1_1_data_1a2d9b571389fc77e659f7583cd2436d21>`() const;
		void :ref:`setName<doxid-class_inference_engine_1_1_data_1a2e3373a63cbb27493d18b9561728671c>`(const std::string& newName);
		const :ref:`UserValue<doxid-union_inference_engine_1_1_user_value>`& :ref:`getUserObject<doxid-class_inference_engine_1_1_data_1a81716bfbcb5ad4221ad7c9be8a616570>`() const;
	};
.. _details-class_inference_engine_1_1_data:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents the main :ref:`Data <doxid-class_inference_engine_1_1_data>` representation node.

The NN graphs are di-graphs consisting of data nodes and layer nodes.

Construction
------------

.. _doxid-class_inference_engine_1_1_data_1ae1caca206b49e0a12d910b411b3b21bf:
.. index:: pair: function; Data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Data(const std::string& name, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` _precision, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout = :ref:`NCHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ad6021da38189a289671c55a105a5ffbf>`)

An empty constructor (dimensionless)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of the data node

	*
		- _precision

		- :ref:`Precision <doxid-class_inference_engine_1_1_precision>` of the data

	*
		- layout

		- :ref:`Data <doxid-class_inference_engine_1_1_data>` layout

.. _doxid-class_inference_engine_1_1_data_1a35d33c241c6bc1b0cf756fe94fc9e77e:
.. index:: pair: function; Data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Data(const std::string& name, const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc)

A constructor with tensor descriptor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of the data node

	*
		- desc

		- Tensor descriptor

.. _doxid-class_inference_engine_1_1_data_1a3e0f1f540578fcb32a31182e5b35f63d:
.. index:: pair: function; Data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Data(const Data& data)

A copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- data

		- A data object to copy from

Methods
-------

.. _doxid-class_inference_engine_1_1_data_1a7147b1956712cbf05aa606769e926ba0:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Data& operator = (const Data& data)

An assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- data

		- A data object to copy from



.. rubric:: Returns:

An assigned object

.. _doxid-class_inference_engine_1_1_data_1ae306efbe9612f9908fa2e3bf581b0607:
.. index:: pair: function; isInitialized

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isInitialized() const

Checks if the current node is resolved.



.. rubric:: Returns:

true if resolved, false otherwise.

.. _doxid-class_inference_engine_1_1_data_1ae04e2471c0bb9052ebc240ecf4452c48:
.. index:: pair: function; setDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDims(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& a_dims)

Sets the data dimensions.

After the current node is marked as resolved.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- a_dims

		- Tensor dimensions to set

.. _doxid-class_inference_engine_1_1_data_1a141c32d0ccd90173289a86e860035edc:
.. index:: pair: function; setLayout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLayout(:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout)

Sets the layout value for this :ref:`Data <doxid-class_inference_engine_1_1_data>` instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layout

		- Layout value to set

.. _doxid-class_inference_engine_1_1_data_1a2292c0006218a73fd5c5f47f62e2d746:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reshape(const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout)

changes dims and layout at same time



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- new dimensions

	*
		- layout

		- new layout

.. _doxid-class_inference_engine_1_1_data_1abaf4dede294e598b7e8c5f1822ce860f:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reshape(const std::initializer_list<size_t>& dims, :ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` layout)

changes dims and layout at same time

Deprecated Use :ref:`InferenceEngine::Data::reshape(const SizeVector&, Layout) <doxid-class_inference_engine_1_1_data_1a2292c0006218a73fd5c5f47f62e2d746>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- new dimensions

	*
		- layout

		- new layout

.. _doxid-class_inference_engine_1_1_data_1a21f0e64bac899e582ae53bb724256cec:
.. index:: pair: function; getLayout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` getLayout() const

Gets the layout value for this :ref:`Data <doxid-class_inference_engine_1_1_data>` instance.



.. rubric:: Returns:

Layout

.. _doxid-class_inference_engine_1_1_data_1a945094e6ff29ea0bbcb5fcbe2ef5d4bb:
.. index:: pair: function; getTensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& getTensorDesc() const

Gets Tensor descriptor reference.



.. rubric:: Returns:

reference to :ref:`TensorDesc <doxid-class_inference_engine_1_1_tensor_desc>`

.. _doxid-class_inference_engine_1_1_data_1a385ca58fa66dd27a573b00bb3fbb6909:
.. index:: pair: function; getPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& getPrecision() const

Gets a precision type of this :ref:`Data <doxid-class_inference_engine_1_1_data>` instance.



.. rubric:: Returns:

:ref:`Precision <doxid-class_inference_engine_1_1_precision>` type

.. _doxid-class_inference_engine_1_1_data_1ac2fb64fdb6f5891c946a9b6200fc8a3e:
.. index:: pair: function; setPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setPrecision(const :ref:`Precision<doxid-class_inference_engine_1_1_precision>`& precision)

Sets a precision type of this :ref:`Data <doxid-class_inference_engine_1_1_data>` instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- precision

		- :ref:`Precision <doxid-class_inference_engine_1_1_precision>` of the data

.. _doxid-class_inference_engine_1_1_data_1afb164ba11a7d23143f0fe56620e3e1ad:
.. index:: pair: function; getDims

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`& getDims() const



.. rubric:: Returns:

data dimensions

.. _doxid-class_inference_engine_1_1_data_1a2d9b571389fc77e659f7583cd2436d21:
.. index:: pair: function; getName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& getName() const



.. rubric:: Returns:

name of the data object

.. _doxid-class_inference_engine_1_1_data_1a2e3373a63cbb27493d18b9561728671c:
.. index:: pair: function; setName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setName(const std::string& newName)

Sets a name the :ref:`Data <doxid-class_inference_engine_1_1_data>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- newName

		- Name of the data node

.. _doxid-class_inference_engine_1_1_data_1a81716bfbcb5ad4221ad7c9be8a616570:
.. index:: pair: function; getUserObject

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`UserValue<doxid-union_inference_engine_1_1_user_value>`& getUserObject() const



.. rubric:: Returns:

convenient arbitrary user data holder


