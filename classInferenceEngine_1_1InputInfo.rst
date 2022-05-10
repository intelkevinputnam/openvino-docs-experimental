.. index:: pair: class; InferenceEngine::InputInfo
.. _doxid-class_inference_engine_1_1_input_info:

class InferenceEngine::InputInfo
================================



Overview
~~~~~~~~

This class contains information about each input of the network. :ref:`More...<details-class_inference_engine_1_1_input_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_input_info.hpp>
	
	class InputInfo
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<InputInfo> :ref:`Ptr<doxid-class_inference_engine_1_1_input_info_1a607e9d454a48136c3cae731cc5a140d2>`;
		typedef std::shared_ptr<const InputInfo> :ref:`CPtr<doxid-class_inference_engine_1_1_input_info_1a2e6948807fd857682e1384c1e882a6d4>`;

		// methods
	
		:ref:`Precision<doxid-class_inference_engine_1_1_precision>` :ref:`getPrecision<doxid-class_inference_engine_1_1_input_info_1a91fce5e01a9601edddb3d1cfe25376b8>`() const;
		void :ref:`setPrecision<doxid-class_inference_engine_1_1_input_info_1adf907f3c369602287d96e9732b541752>`(:ref:`Precision<doxid-class_inference_engine_1_1_precision>` p);
		:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` :ref:`getLayout<doxid-class_inference_engine_1_1_input_info_1a150439ea99908a822fca3c068e76b44a>`();
		void :ref:`setLayout<doxid-class_inference_engine_1_1_input_info_1ae201671bc62fced623fe4b800ff5bcb2>`(:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` l);
		const std::string& :ref:`name<doxid-class_inference_engine_1_1_input_info_1af6f3075557eca26973d228b03a9bdda0>`() const;
		:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>` :ref:`getInputData<doxid-class_inference_engine_1_1_input_info_1a66d2b4718f7d693535f4e723edf1d681>`() const;
		void :ref:`setInputData<doxid-class_inference_engine_1_1_input_info_1aa4e516d5ab5da581b6e2ff8f48b73023>`(:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>` inputPtr);
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& :ref:`getTensorDesc<doxid-class_inference_engine_1_1_input_info_1a65c4a49509159dd42cc2de2b49ad2aaf>`() const;
		:ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& :ref:`getPreProcess<doxid-class_inference_engine_1_1_input_info_1a83d3f56e7b16bce1022d6c5364347e1d>`();
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& :ref:`getPreProcess<doxid-class_inference_engine_1_1_input_info_1a543e135dde50c5136fd734892d23df5f>`() const;
	};
.. _details-class_inference_engine_1_1_input_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class contains information about each input of the network.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_input_info_1a607e9d454a48136c3cae731cc5a140d2:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<InputInfo> Ptr

A smart pointer to the :ref:`InputInfo <doxid-class_inference_engine_1_1_input_info>` instance.

.. _doxid-class_inference_engine_1_1_input_info_1a2e6948807fd857682e1384c1e882a6d4:
.. index:: pair: typedef; CPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<const InputInfo> CPtr

A smart pointer to the constant :ref:`InputInfo <doxid-class_inference_engine_1_1_input_info>` instance.

Methods
-------

.. _doxid-class_inference_engine_1_1_input_info_1a91fce5e01a9601edddb3d1cfe25376b8:
.. index:: pair: function; getPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Precision<doxid-class_inference_engine_1_1_precision>` getPrecision() const

Gets a precision of the input data provided by user.

By default it matches the layers precision, but there are exceptions of this rule For Q78 precision networks the input is expected in I16 by default For FP16 precision networks the input is expected in FP32 by default The default input precision might be changed preferred one using :ref:`InputInfo::setPrecision() <doxid-class_inference_engine_1_1_input_info_1adf907f3c369602287d96e9732b541752>` function. For example, for a Q78 precision network you can pass FP32 input data



.. rubric:: Returns:

The precision used for input blob creation

.. _doxid-class_inference_engine_1_1_input_info_1adf907f3c369602287d96e9732b541752:
.. index:: pair: function; setPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setPrecision(:ref:`Precision<doxid-class_inference_engine_1_1_precision>` p)

Changes the precision of the input data provided by the user.

This function should be called before loading the network to the plugin



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- A new precision of the input data to set

.. _doxid-class_inference_engine_1_1_input_info_1a150439ea99908a822fca3c068e76b44a:
.. index:: pair: function; getLayout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` getLayout()

Gets a layout of the input data provided by user.

By default it matches the layers precision and depends on number of its dimensions: C - for 1-dimensional, NC - for 2-dimensional, CHW - for 3-dimensional, NCHW - for 4-dimensional NCDHW - for 5-dimensional The default input layout might be changed preferred one using :ref:`setLayout() <doxid-class_inference_engine_1_1_input_info_1ae201671bc62fced623fe4b800ff5bcb2>` function.



.. rubric:: Returns:

The precision used for input blob creation

.. _doxid-class_inference_engine_1_1_input_info_1ae201671bc62fced623fe4b800ff5bcb2:
.. index:: pair: function; setLayout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLayout(:ref:`Layout<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>` l)

Changes the layout of the input data provided by the user.

This function should be called before loading the network to the plugin



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- l

		- A new layout of the input data to set

.. _doxid-class_inference_engine_1_1_input_info_1af6f3075557eca26973d228b03a9bdda0:
.. index:: pair: function; name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& name() const

Gets the name of the input.



.. rubric:: Returns:

A string - the name of the input

.. _doxid-class_inference_engine_1_1_input_info_1a66d2b4718f7d693535f4e723edf1d681:
.. index:: pair: function; getInputData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>` getInputData() const

Gets the input data.



.. rubric:: Returns:

A smart pointer to the input data

.. _doxid-class_inference_engine_1_1_input_info_1aa4e516d5ab5da581b6e2ff8f48b73023:
.. index:: pair: function; setInputData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setInputData(:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>` inputPtr)

Initializes the pointer to the input data that stores the main input parameters like dims, etc.

This method initializes the precision with the information from the inputPtr if it was not set explicitly through :ref:`InputInfo::setPrecision <doxid-class_inference_engine_1_1_input_info_1adf907f3c369602287d96e9732b541752>`. If :ref:`InputInfo::setPrecision <doxid-class_inference_engine_1_1_input_info_1adf907f3c369602287d96e9732b541752>` is called, this method does not overwrite the precision.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputPtr

		- Pointer to the input data to set

.. _doxid-class_inference_engine_1_1_input_info_1a65c4a49509159dd42cc2de2b49ad2aaf:
.. index:: pair: function; getTensorDesc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& getTensorDesc() const

Returns the tensor descriptor.



.. rubric:: Returns:

A const reference to a tensor descriptor

.. _doxid-class_inference_engine_1_1_input_info_1a83d3f56e7b16bce1022d6c5364347e1d:
.. index:: pair: function; getPreProcess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& getPreProcess()

Gets pre-process info for the input.



.. rubric:: Returns:

A reference to the :ref:`PreProcessInfo <doxid-class_inference_engine_1_1_pre_process_info>` instance that contains pre-process info for this input

.. _doxid-class_inference_engine_1_1_input_info_1a543e135dde50c5136fd734892d23df5f:
.. index:: pair: function; getPreProcess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& getPreProcess() const

Gets pre-process info for the input.



.. rubric:: Returns:

A reference to the :ref:`PreProcessInfo <doxid-class_inference_engine_1_1_pre_process_info>` instance that contains pre-process info for this input


