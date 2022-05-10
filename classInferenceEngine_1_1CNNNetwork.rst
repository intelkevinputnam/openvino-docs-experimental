.. index:: pair: class; InferenceEngine::CNNNetwork
.. _doxid-class_inference_engine_1_1_c_n_n_network:

class InferenceEngine::CNNNetwork
=================================



Overview
~~~~~~~~

This class contains all the information about the Neural Network and the related binary information. :ref:`More...<details-class_inference_engine_1_1_c_n_n_network>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_cnn_network.h>
	
	class CNNNetwork
	{
	public:
		// construction
	
		:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network_1a15a61ce775290533173d4cf80df17695>`();
		:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network_1a65d11914bffbce3db04dc42ac0b373dd>`(std::shared_ptr<:ref:`ICNNNetwork<doxid-class_inference_engine_1_1_i_c_n_n_network>`> network);
	
		:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network_1a91cb51f2ace7cf855e01197fd074ee84>`(
			const std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& network,
			const std::vector<std::shared_ptr<:ref:`IExtension<doxid-class_inference_engine_1_1_i_extension>`>>& exts = {}
			);

		// methods
	
		:ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>` :ref:`getOutputsInfo<doxid-class_inference_engine_1_1_c_n_n_network_1af8a6200f549b15a895e2cfefd304a9c2>`() const;
		:ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>` :ref:`getInputsInfo<doxid-class_inference_engine_1_1_c_n_n_network_1a76de2a6101fe8276f56b0dc0f99c7ff7>`() const;
		size_t :ref:`layerCount<doxid-class_inference_engine_1_1_c_n_n_network_1a5d309251fd922e4fb487101a9c1054af>`() const;
		const std::string& :ref:`getName<doxid-class_inference_engine_1_1_c_n_n_network_1a958c0aeee2e7571d200d470cb3ea6d8c>`() const;
		void :ref:`setBatchSize<doxid-class_inference_engine_1_1_c_n_n_network_1a8e9d19270a48aab50cb5b1c43eecb8e9>`(const size_t size);
		size_t :ref:`getBatchSize<doxid-class_inference_engine_1_1_c_n_n_network_1a5dae69fc7fc2fc6ae4305fb2b3634941>`() const;
		:ref:`operator ICNNNetwork::Ptr<doxid-class_inference_engine_1_1_c_n_n_network_1a1c3489090ce7f3a0e2be88325d835776>` ();
		:ref:`operator ICNNNetwork &<doxid-class_inference_engine_1_1_c_n_n_network_1ab037f4b0efb1f76e9821d808327ae77e>` ();
		:ref:`operator const ICNNNetwork &<doxid-class_inference_engine_1_1_c_n_n_network_1aeb37a0d25c851bf29caa6dcb76f5aaf6>` () const;
		std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`getFunction<doxid-class_inference_engine_1_1_c_n_n_network_1a7246c6936dfc1ebfa2c776e97972f539>`();
		std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`getFunction<doxid-class_inference_engine_1_1_c_n_n_network_1a32eddfb395e909c7e2bc7f174ead4279>`() const;
		void :ref:`addOutput<doxid-class_inference_engine_1_1_c_n_n_network_1a82aab37cdb789cff0e1f96178bb4dcd3>`(const std::string& layerName, size_t outputIndex = 0);
		:ref:`ICNNNetwork::InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>` :ref:`getInputShapes<doxid-class_inference_engine_1_1_c_n_n_network_1a826b8c6d282bcb8dfd283da58fb22c31>`() const;
		void :ref:`reshape<doxid-class_inference_engine_1_1_c_n_n_network_1abaa4311b783beb2f7bd2ff103589816c>`(const :ref:`ICNNNetwork::InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>`& inputShapes);
		void :ref:`serialize<doxid-class_inference_engine_1_1_c_n_n_network_1a29d6fdf1a6fa1e9ee5dc33608536da77>`(const std::string& xmlPath, const std::string& binPath = {}) const;
		void :ref:`serialize<doxid-class_inference_engine_1_1_c_n_n_network_1a996d736712eaca9d0f1ed2326dcc7922>`(std::ostream& xmlBuf, std::ostream& binBuf) const;
		void :ref:`serialize<doxid-class_inference_engine_1_1_c_n_n_network_1a0640278923e6f6793ab068f9b3f8c06c>`(std::ostream& xmlBuf, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& binBlob) const;
		std::string :ref:`getOVNameForTensor<doxid-class_inference_engine_1_1_c_n_n_network_1a367dddf7cf51fe547d985aac77efa05a>`(const std::string& orig_name) const;
	};
.. _details-class_inference_engine_1_1_c_n_n_network:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class contains all the information about the Neural Network and the related binary information.

Construction
------------

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a15a61ce775290533173d4cf80df17695:
.. index:: pair: function; CNNNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNNetwork()

A default constructor.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a65d11914bffbce3db04dc42ac0b373dd:
.. index:: pair: function; CNNNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNNetwork(std::shared_ptr<:ref:`ICNNNetwork<doxid-class_inference_engine_1_1_i_c_n_n_network>`> network)

Allows helper class to manage lifetime of network object.

Deprecated Don't use this constructor. It will be removed soon



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- Pointer to the network object

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a91cb51f2ace7cf855e01197fd074ee84:
.. index:: pair: function; CNNNetwork

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNNetwork(
		const std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& network,
		const std::vector<std::shared_ptr<:ref:`IExtension<doxid-class_inference_engine_1_1_i_extension>`>>& exts = {}
		)

A constructor from :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` object This constructor wraps existing :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` If you want to avoid modification of original Function, please create a copy.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- network

		- Pointer to the :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` object

	*
		- exts

		- Vector of pointers to IE extension objects

Methods
-------

.. _doxid-class_inference_engine_1_1_c_n_n_network_1af8a6200f549b15a895e2cfefd304a9c2:
.. index:: pair: function; getOutputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>` getOutputsInfo() const

Gets the network output :ref:`Data <doxid-class_inference_engine_1_1_data>` node information. The received info is stored in the given :ref:`Data <doxid-class_inference_engine_1_1_data>` node.

For single and multiple outputs networks.

This method need to be called to find out OpenVINO output names for using them later when calling :ref:`InferenceEngine::InferRequest::GetBlob <doxid-class_inference_engine_1_1_infer_request_1a9601a4cda3f309181af34feedf1b914c>` or :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`

If you want to use framework names, you can use :ref:`InferenceEngine::CNNNetwork::getOVNameForTensor <doxid-class_inference_engine_1_1_c_n_n_network_1a367dddf7cf51fe547d985aac77efa05a>` method to map framework names to OpenVINO names



.. rubric:: Returns:

the :ref:`InferenceEngine::OutputsDataMap <doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>` object

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a76de2a6101fe8276f56b0dc0f99c7ff7:
.. index:: pair: function; getInputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>` getInputsInfo() const

Gets the network input :ref:`Data <doxid-class_inference_engine_1_1_data>` node information. The received info is stored in the given InputsDataMap object.

For single and multiple inputs networks. This method need to be called to find out OpenVINO input names for using them later when calling :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`

If you want to use framework names, you can use :ref:`InferenceEngine::ICNNNetwork::getOVNameForTensor <doxid-class_inference_engine_1_1_i_c_n_n_network_1a9909922d0ba2139f1e6315d8d19f33e0>` method to map framework names to OpenVINO names



.. rubric:: Returns:

The :ref:`InferenceEngine::InputsDataMap <doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>` object.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a5d309251fd922e4fb487101a9c1054af:
.. index:: pair: function; layerCount

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t layerCount() const

Returns the number of layers in the network as an integer value.



.. rubric:: Returns:

The number of layers as an integer value

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a958c0aeee2e7571d200d470cb3ea6d8c:
.. index:: pair: function; getName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& getName() const

Returns the network name.



.. rubric:: Returns:

Network name

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a8e9d19270a48aab50cb5b1c43eecb8e9:
.. index:: pair: function; setBatchSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setBatchSize(const size_t size)

Changes the inference batch size.

There are several limitations and it's not recommended to use it. Set batch to the input shape and call :ref:`InferenceEngine::CNNNetwork::reshape <doxid-class_inference_engine_1_1_c_n_n_network_1abaa4311b783beb2f7bd2ff103589816c>`.

Current implementation of the function sets batch size to the first dimension of all layers in the networks. Before calling it make sure that all your layers have batch in the first dimension, otherwise the method works incorrectly. This limitation is resolved via shape inference feature by using :ref:`InferenceEngine::ICNNNetwork::reshape <doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf>` method. To read more refer to the Shape Inference section in documentation

Current implementation of the function sets batch size to the first dimension of all layers in the networks. Before calling it make sure that all your layers have batch in the first dimension, otherwise the method works incorrectly. This limitation is resolved via shape inference feature by using :ref:`InferenceEngine::ICNNNetwork::reshape <doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf>` method. To read more refer to the Shape Inference section in documentation



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size

		- Size of batch to set

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a5dae69fc7fc2fc6ae4305fb2b3634941:
.. index:: pair: function; getBatchSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getBatchSize() const

Gets the inference batch size.



.. rubric:: Returns:

The size of batch as a size_t value

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a1c3489090ce7f3a0e2be88325d835776:
.. index:: pair: function; operator ICNNNetwork::Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator ICNNNetwork::Ptr ()

An overloaded operator cast to get pointer on current network.

Deprecated :ref:`InferenceEngine::ICNNNetwork <doxid-class_inference_engine_1_1_i_c_n_n_network>` interface is deprecated



.. rubric:: Returns:

A shared pointer of the current network

.. _doxid-class_inference_engine_1_1_c_n_n_network_1ab037f4b0efb1f76e9821d808327ae77e:
.. index:: pair: function; operator ICNNNetwork &

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator ICNNNetwork & ()

An overloaded operator & to get current network.

Deprecated :ref:`InferenceEngine::ICNNNetwork <doxid-class_inference_engine_1_1_i_c_n_n_network>` interface is deprecated



.. rubric:: Returns:

An instance of the current network

.. _doxid-class_inference_engine_1_1_c_n_n_network_1aeb37a0d25c851bf29caa6dcb76f5aaf6:
.. index:: pair: function; operator const ICNNNetwork &

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator const ICNNNetwork & () const

An overloaded operator & to get current network.

Deprecated :ref:`InferenceEngine::ICNNNetwork <doxid-class_inference_engine_1_1_i_c_n_n_network>` interface is deprecated



.. rubric:: Returns:

A const reference of the current network

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a7246c6936dfc1ebfa2c776e97972f539:
.. index:: pair: function; getFunction

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> getFunction()

Returns constant nGraph function.



.. rubric:: Returns:

constant nGraph function

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a32eddfb395e909c7e2bc7f174ead4279:
.. index:: pair: function; getFunction

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> getFunction() const

Returns constant nGraph function.



.. rubric:: Returns:

constant nGraph function

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a82aab37cdb789cff0e1f96178bb4dcd3:
.. index:: pair: function; addOutput

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void addOutput(const std::string& layerName, size_t outputIndex = 0)

Adds output to the layer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layerName

		- Name of the layer

	*
		- outputIndex

		- Index of the output

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a826b8c6d282bcb8dfd283da58fb22c31:
.. index:: pair: function; getInputShapes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ICNNNetwork::InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>` getInputShapes() const

Helper method to get collect all input shapes with names of corresponding :ref:`Data <doxid-class_inference_engine_1_1_data>` objects.



.. rubric:: Returns:

Map of pairs: input name and its dimension.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1abaa4311b783beb2f7bd2ff103589816c:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reshape(const :ref:`ICNNNetwork::InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>`& inputShapes)

Run shape inference with new input shapes for the network.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputShapes

		- A map of pairs: name of corresponding data and its dimension.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a29d6fdf1a6fa1e9ee5dc33608536da77:
.. index:: pair: function; serialize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void serialize(const std::string& xmlPath, const std::string& binPath = {}) const

Serialize network to IR and weights files.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlPath

		- Path to output IR file.

	*
		- binPath

		- Path to output weights file. The parameter is skipped in case of executable graph info serialization.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a996d736712eaca9d0f1ed2326dcc7922:
.. index:: pair: function; serialize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void serialize(std::ostream& xmlBuf, std::ostream& binBuf) const

Serialize network to IR and weights streams.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlBuf

		- output IR stream.

	*
		- binBuf

		- output weights stream.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a0640278923e6f6793ab068f9b3f8c06c:
.. index:: pair: function; serialize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void serialize(std::ostream& xmlBuf, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& binBlob) const

Serialize network to IR stream and weights :ref:`Blob::Ptr <doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlBuf

		- output IR stream.

	*
		- binBlob

		- output weights :ref:`Blob::Ptr <doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`.

.. _doxid-class_inference_engine_1_1_c_n_n_network_1a367dddf7cf51fe547d985aac77efa05a:
.. index:: pair: function; getOVNameForTensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getOVNameForTensor(const std::string& orig_name) const

Method maps framework tensor name to OpenVINO name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- orig_name

		- Framework tensor name



.. rubric:: Returns:

OpenVINO name


