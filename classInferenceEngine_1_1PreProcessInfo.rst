.. index:: pair: class; InferenceEngine::PreProcessInfo
.. _doxid-class_inference_engine_1_1_pre_process_info:

class InferenceEngine::PreProcessInfo
=====================================



Overview
~~~~~~~~

This class stores pre-process information for the input. :ref:`More...<details-class_inference_engine_1_1_pre_process_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess.hpp>
	
	class PreProcessInfo
	{
	public:
		// methods
	
		:ref:`PreProcessChannel::Ptr<doxid-struct_inference_engine_1_1_pre_process_channel_1abde989b919c44225ea30dbacb64f34b2>`& :ref:`operator []<doxid-class_inference_engine_1_1_pre_process_info_1a635c9b36ff4281fd13804508c4ecf933>` (size_t index);
		const :ref:`PreProcessChannel::Ptr<doxid-struct_inference_engine_1_1_pre_process_channel_1abde989b919c44225ea30dbacb64f34b2>`& :ref:`operator []<doxid-class_inference_engine_1_1_pre_process_info_1a96d4b00b1e7355f836fa2b47539ef29e>` (size_t index) const;
		size_t :ref:`getNumberOfChannels<doxid-class_inference_engine_1_1_pre_process_info_1a753abdd56c2918eff9eeafdd7a105c11>`() const;
		void :ref:`init<doxid-class_inference_engine_1_1_pre_process_info_1a064ac8a3065908e633ccf7ade268e194>`(const size_t numberOfChannels);
		void :ref:`setMeanImage<doxid-class_inference_engine_1_1_pre_process_info_1a517cea4e7efa30c17b95a68c6f5242ac>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& meanImage);
		void :ref:`setMeanImageForChannel<doxid-class_inference_engine_1_1_pre_process_info_1aafe4d2b5e1bee8765897ced0f138c5d4>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& meanImage, const size_t channel);
		void :ref:`setVariant<doxid-class_inference_engine_1_1_pre_process_info_1acea34efcbf883b854627e89dabd62441>`(const :ref:`MeanVariant<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161>`& variant);
		:ref:`MeanVariant<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161>` :ref:`getMeanVariant<doxid-class_inference_engine_1_1_pre_process_info_1aa9e2b45a3cd4f47dcebe8afe4e9331ae>`() const;
		void :ref:`setResizeAlgorithm<doxid-class_inference_engine_1_1_pre_process_info_1a0c083c43d01c53c327f09095e3e3f004>`(const :ref:`ResizeAlgorithm<doxid-namespace_inference_engine_1a805a09efb0e7b327ffa078f8d02222e9>`& alg);
		:ref:`ResizeAlgorithm<doxid-namespace_inference_engine_1a805a09efb0e7b327ffa078f8d02222e9>` :ref:`getResizeAlgorithm<doxid-class_inference_engine_1_1_pre_process_info_1a278b115ef810716b4a328733a5c1329a>`() const;
		void :ref:`setColorFormat<doxid-class_inference_engine_1_1_pre_process_info_1a3a10ba0d562a2268fe584d4d2db94cac>`(:ref:`ColorFormat<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a>` fmt);
		:ref:`ColorFormat<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a>` :ref:`getColorFormat<doxid-class_inference_engine_1_1_pre_process_info_1a259085aba02d149edac544323fdf33f2>`() const;
	};
.. _details-class_inference_engine_1_1_pre_process_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class stores pre-process information for the input.

Methods
-------

.. _doxid-class_inference_engine_1_1_pre_process_info_1a635c9b36ff4281fd13804508c4ecf933:
.. index:: pair: function; operator[]

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PreProcessChannel::Ptr<doxid-struct_inference_engine_1_1_pre_process_channel_1abde989b919c44225ea30dbacb64f34b2>`& operator [] (size_t index)

Overloaded [] operator to safely get the channel by an index.

Throws an exception if channels are empty



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- Index of the channel to get



.. rubric:: Returns:

The pre-process channel instance

.. _doxid-class_inference_engine_1_1_pre_process_info_1a96d4b00b1e7355f836fa2b47539ef29e:
.. index:: pair: function; operator[]

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PreProcessChannel::Ptr<doxid-struct_inference_engine_1_1_pre_process_channel_1abde989b919c44225ea30dbacb64f34b2>`& operator [] (size_t index) const

operator [] to safely get the channel preprocessing information by index.

Throws exception if channels are empty or index is out of border



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- Index of the channel to get



.. rubric:: Returns:

The const preprocess channel instance

.. _doxid-class_inference_engine_1_1_pre_process_info_1a753abdd56c2918eff9eeafdd7a105c11:
.. index:: pair: function; getNumberOfChannels

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getNumberOfChannels() const

Returns a number of channels to preprocess.



.. rubric:: Returns:

The number of channels

.. _doxid-class_inference_engine_1_1_pre_process_info_1a064ac8a3065908e633ccf7ade268e194:
.. index:: pair: function; init

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void init(const size_t numberOfChannels)

Initializes with given number of channels.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- numberOfChannels

		- Number of channels to initialize

.. _doxid-class_inference_engine_1_1_pre_process_info_1a517cea4e7efa30c17b95a68c6f5242ac:
.. index:: pair: function; setMeanImage

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMeanImage(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& meanImage)

Sets mean image values if operation is applicable.

Also sets the mean type to MEAN_IMAGE for all channels



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- meanImage

		- :ref:`Blob <doxid-class_inference_engine_1_1_blob>` with a mean image

.. _doxid-class_inference_engine_1_1_pre_process_info_1aafe4d2b5e1bee8765897ced0f138c5d4:
.. index:: pair: function; setMeanImageForChannel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMeanImageForChannel(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& meanImage, const size_t channel)

Sets mean image values if operation is applicable.

Also sets the mean type to MEAN_IMAGE for a particular channel



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- meanImage

		- :ref:`Blob <doxid-class_inference_engine_1_1_blob>` with a mean image

	*
		- channel

		- Index of a particular channel

.. _doxid-class_inference_engine_1_1_pre_process_info_1acea34efcbf883b854627e89dabd62441:
.. index:: pair: function; setVariant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setVariant(const :ref:`MeanVariant<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161>`& variant)

Sets a type of mean operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variant

		- Type of mean operation to set

.. _doxid-class_inference_engine_1_1_pre_process_info_1aa9e2b45a3cd4f47dcebe8afe4e9331ae:
.. index:: pair: function; getMeanVariant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`MeanVariant<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161>` getMeanVariant() const

Gets a type of mean operation.



.. rubric:: Returns:

The type of mean operation

.. _doxid-class_inference_engine_1_1_pre_process_info_1a0c083c43d01c53c327f09095e3e3f004:
.. index:: pair: function; setResizeAlgorithm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setResizeAlgorithm(const :ref:`ResizeAlgorithm<doxid-namespace_inference_engine_1a805a09efb0e7b327ffa078f8d02222e9>`& alg)

Sets resize algorithm to be used during pre-processing.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- alg

		- Resize algorithm

.. _doxid-class_inference_engine_1_1_pre_process_info_1a278b115ef810716b4a328733a5c1329a:
.. index:: pair: function; getResizeAlgorithm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ResizeAlgorithm<doxid-namespace_inference_engine_1a805a09efb0e7b327ffa078f8d02222e9>` getResizeAlgorithm() const

Gets preconfigured resize algorithm.



.. rubric:: Returns:

Resize algorithm

.. _doxid-class_inference_engine_1_1_pre_process_info_1a3a10ba0d562a2268fe584d4d2db94cac:
.. index:: pair: function; setColorFormat

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setColorFormat(:ref:`ColorFormat<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a>` fmt)

Changes the color format of the input data provided by the user.

This function should be called before loading the network to the plugin Setting color format different from ColorFormat::RAW enables automatic color conversion (as a part of built-in preprocessing routine)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- fmt

		- A new color format associated with the input

.. _doxid-class_inference_engine_1_1_pre_process_info_1a259085aba02d149edac544323fdf33f2:
.. index:: pair: function; getColorFormat

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ColorFormat<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a>` getColorFormat() const

Gets a color format associated with the input.

By default, the color format is ColorFormat::RAW meaning there is no particular color format assigned to the input



.. rubric:: Returns:

Color format.


