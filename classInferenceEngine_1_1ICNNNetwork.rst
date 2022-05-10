.. index:: pair: interface; InferenceEngine::ICNNNetwork
.. _doxid-class_inference_engine_1_1_i_c_n_n_network:

interface InferenceEngine::ICNNNetwork
======================================



Overview
~~~~~~~~

This is the main interface to describe the NN topology. :ref:`More...<details-class_inference_engine_1_1_i_c_n_n_network>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_icnn_network.hpp>
	
	template ICNNNetwork: public std::enable_shared_from_this< ICNNNetwork >
	{
		// typedefs
	
		typedef std::shared_ptr<ICNNNetwork> :ref:`Ptr<doxid-class_inference_engine_1_1_i_c_n_n_network_1a05b6f650d23e571e03da46a3a89db633>`;
		typedef std::map<std::string, :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`> :ref:`InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>`;

		// methods
	
		virtual std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`getFunction<doxid-class_inference_engine_1_1_i_c_n_n_network_1ace8fe66eb55229bd517576e01d1a5f90>`() = 0;
		virtual std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> :ref:`getFunction<doxid-class_inference_engine_1_1_i_c_n_n_network_1a1abddf86b53ec3faffd4ee27175ddbc0>`() const = 0;
		virtual void :ref:`getOutputsInfo<doxid-class_inference_engine_1_1_i_c_n_n_network_1a67b659f1a8fd1574bb1939ea3f672fad>`(:ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& out) const = 0;
		virtual void :ref:`getInputsInfo<doxid-class_inference_engine_1_1_i_c_n_n_network_1ac0d904dcfd039972e04923f1e0befbdd>`(:ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& inputs) const = 0;
		virtual :ref:`InputInfo::Ptr<doxid-class_inference_engine_1_1_input_info_1a607e9d454a48136c3cae731cc5a140d2>` :ref:`getInput<doxid-class_inference_engine_1_1_i_c_n_n_network_1ae952db225b323f5c809ded22c30da4ed>`(const std::string& inputName) const = 0;
		virtual const std::string& :ref:`getName<doxid-class_inference_engine_1_1_i_c_n_n_network_1a5cb3d873dd395d2537cbafce612f5a44>`() const = 0;
		virtual size_t :ref:`layerCount<doxid-class_inference_engine_1_1_i_c_n_n_network_1ae6205636e448fe10f860012910f50ffd>`() const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`addOutput<doxid-class_inference_engine_1_1_i_c_n_n_network_1a07f2f7ada6d7208710ae3dc144347df8>`(
			const std::string& layerName,
			size_t outputIndex = 0,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp = nullptr
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`setBatchSize<doxid-class_inference_engine_1_1_i_c_n_n_network_1ac29fc798d8a318f380624bd350b28501>`(size_t size, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* responseDesc) = 0;
		virtual size_t :ref:`getBatchSize<doxid-class_inference_engine_1_1_i_c_n_n_network_1a42a783cf372dca11b615c6f28d5456cb>`() const = 0;
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`reshape<doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf>`(const :ref:`InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>`& inputShapes, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp);
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`reshape<doxid-class_inference_engine_1_1_i_c_n_n_network_1a91791651378668551ea48040b30b7459>`(
			const std::map<std::string, :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`>& partialShapes,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			);
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`serialize<doxid-class_inference_engine_1_1_i_c_n_n_network_1acd12b5e9b9c6881ce33230a77b3031cf>`(
			const std::string& xmlPath,
			const std::string& binPath,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`serialize<doxid-class_inference_engine_1_1_i_c_n_n_network_1a07dfb4ea0bcd5a3008fdc82535969d97>`(
			std::ostream& xmlStream,
			std::ostream& binStream,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`serialize<doxid-class_inference_engine_1_1_i_c_n_n_network_1a1e678ce338cdfd9b0a056a55acb402ba>`(
			std::ostream& xmlStream,
			:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& binData,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`getOVNameForTensor<doxid-class_inference_engine_1_1_i_c_n_n_network_1a9909922d0ba2139f1e6315d8d19f33e0>`(
			std::string& ov_name,
			const std::string& orig_name,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) const;

	protected:
	};
.. _details-class_inference_engine_1_1_i_c_n_n_network:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is the main interface to describe the NN topology.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a05b6f650d23e571e03da46a3a89db633:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ICNNNetwork> Ptr

A shared pointer to a :ref:`ICNNNetwork <doxid-class_inference_engine_1_1_i_c_n_n_network>` interface.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d:
.. index:: pair: typedef; InputShapes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::map<std::string, :ref:`SizeVector<doxid-namespace_inference_engine_1a9400de686d3d0f48c30cd73d40e48576>`> InputShapes

Map of pairs: name of corresponding data and its dimension.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead

Methods
-------

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1ace8fe66eb55229bd517576e01d1a5f90:
.. index:: pair: function; getFunction

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> getFunction() = 0

Returns nGraph function.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Returns:

nGraph function

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a1abddf86b53ec3faffd4ee27175ddbc0:
.. index:: pair: function; getFunction

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<const :ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`> getFunction() const = 0

Returns constant nGraph function.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Returns:

constant nGraph function

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a67b659f1a8fd1574bb1939ea3f672fad:
.. index:: pair: function; getOutputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void getOutputsInfo(:ref:`OutputsDataMap<doxid-namespace_inference_engine_1a76ce999f68455cf962a473718deb500c>`& out) const = 0

Gets the network output :ref:`Data <doxid-class_inference_engine_1_1_data>` node information. The received info is stored in the given :ref:`Data <doxid-class_inference_engine_1_1_data>` node.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead

For single and multiple outputs networks.

This method need to be called to find out OpenVINO output names for using them later when calling :ref:`InferenceEngine::InferRequest::GetBlob <doxid-class_inference_engine_1_1_infer_request_1a9601a4cda3f309181af34feedf1b914c>` or :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`

If you want to use framework names, you can use :ref:`InferenceEngine::ICNNNetwork::getOVNameForTensor <doxid-class_inference_engine_1_1_i_c_n_n_network_1a9909922d0ba2139f1e6315d8d19f33e0>` method to map framework names to OpenVINO names



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- out

		- Reference to the OutputsDataMap object

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1ac0d904dcfd039972e04923f1e0befbdd:
.. index:: pair: function; getInputsInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void getInputsInfo(:ref:`InputsDataMap<doxid-namespace_inference_engine_1a08270747275eb79985154365aa782a2a>`& inputs) const = 0

Gets the network input :ref:`Data <doxid-class_inference_engine_1_1_data>` node information. The received info is stored in the given InputsDataMap object.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead

For single and multiple inputs networks. This method need to be called to find out OpenVINO input names for using them later when calling :ref:`InferenceEngine::InferRequest::SetBlob <doxid-class_inference_engine_1_1_infer_request_1a27fb179e3bae652d76076965fd2a5653>`

If you want to use framework names, you can use :ref:`InferenceEngine::ICNNNetwork::getOVNameForTensor <doxid-class_inference_engine_1_1_i_c_n_n_network_1a9909922d0ba2139f1e6315d8d19f33e0>` method to map framework names to OpenVINO names



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- Reference to InputsDataMap object.

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1ae952db225b323f5c809ded22c30da4ed:
.. index:: pair: function; getInput

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`InputInfo::Ptr<doxid-class_inference_engine_1_1_input_info_1a607e9d454a48136c3cae731cc5a140d2>` getInput(const std::string& inputName) const = 0

Returns information on certain input pointed by inputName.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputName

		- Name of input layer to get info on



.. rubric:: Returns:

A smart pointer to the input information

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a5cb3d873dd395d2537cbafce612f5a44:
.. index:: pair: function; getName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getName() const = 0

Returns the network name.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Returns:

Network name

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1ae6205636e448fe10f860012910f50ffd:
.. index:: pair: function; layerCount

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t layerCount() const = 0

Returns the number of layers in the network as an integer value.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Returns:

The number of layers as an integer value

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a07f2f7ada6d7208710ae3dc144347df8:
.. index:: pair: function; addOutput

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` addOutput(
		const std::string& layerName,
		size_t outputIndex = 0,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp = nullptr
		) = 0

Adds output to the layer.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layerName

		- Name of the layer

	*
		- outputIndex

		- Index of the output

	*
		- resp

		- Response message



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1ac29fc798d8a318f380624bd350b28501:
.. index:: pair: function; setBatchSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` setBatchSize(size_t size, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* responseDesc) = 0

Changes the inference batch size.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead

There are several limitations and it's not recommended to use it. Set batch to the input shape and call :ref:`ICNNNetwork::reshape <doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf>`.

Current implementation of the function sets batch size to the first dimension of all layers in the networks. Before calling it make sure that all your layers have batch in the first dimension, otherwise the method works incorrectly. This limitation is resolved via shape inference feature by using :ref:`InferenceEngine::ICNNNetwork::reshape <doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf>` method. To read more refer to the Shape Inference section in documentation

Current implementation of the function sets batch size to the first dimension of all layers in the networks. Before calling it make sure that all your layers have batch in the first dimension, otherwise the method works incorrectly. This limitation is resolved via shape inference feature by using :ref:`InferenceEngine::ICNNNetwork::reshape <doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf>` method. To read more refer to the Shape Inference section in documentation



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size

		- Size of batch to set

	*
		- responseDesc

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a42a783cf372dca11b615c6f28d5456cb:
.. index:: pair: function; getBatchSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getBatchSize() const = 0

Gets the inference batch size.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Returns:

The size of batch as a size_t value

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1abcfd19bd3e69cbf69ed77285f748b1cf:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` reshape(const :ref:`InputShapes<doxid-class_inference_engine_1_1_i_c_n_n_network_1a8bcef7f638f6588a672a32080047ff1d>`& inputShapes, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp)

Run shape inference with new input shapes for the network.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputShapes

		- - map of pairs: name of corresponding data and its dimension.

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a91791651378668551ea48040b30b7459:
.. index:: pair: function; reshape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` reshape(
		const std::map<std::string, :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`>& partialShapes,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		)

Run shape inference with new input shapes for the network.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- partialShapes

		- - map of pairs: name of corresponding data and its dimension.

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1acd12b5e9b9c6881ce33230a77b3031cf:
.. index:: pair: function; serialize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` serialize(
		const std::string& xmlPath,
		const std::string& binPath,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Serialize network to IR and weights files.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlPath

		- Path to output IR file.

	*
		- binPath

		- Path to output weights file.

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a07dfb4ea0bcd5a3008fdc82535969d97:
.. index:: pair: function; serialize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` serialize(
		std::ostream& xmlStream,
		std::ostream& binStream,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Serialize network to IR and weights files.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlStream

		- A stream for xml content (.xml file)

	*
		- binStream

		- A stream for weights content (.bin file)

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a1e678ce338cdfd9b0a056a55acb402ba:
.. index:: pair: function; serialize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` serialize(
		std::ostream& xmlStream,
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& binData,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const = 0

Serialize network to IR and weights files.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xmlStream

		- A stream for xml content (.xml file)

	*
		- binData

		- A blob for weights content (.bin file)

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation

.. _doxid-class_inference_engine_1_1_i_c_n_n_network_1a9909922d0ba2139f1e6315d8d19f33e0:
.. index:: pair: function; getOVNameForTensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` getOVNameForTensor(
		std::string& ov_name,
		const std::string& orig_name,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) const

Methods maps framework tensor name to OpenVINO name.

Deprecated Use :ref:`InferenceEngine::CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>` wrapper instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ov_name

		- OpenVINO name

	*
		- orig_name

		- Framework tensor name

	*
		- resp

		- Pointer to the response message that holds a description of an error if any occurred



.. rubric:: Returns:

Status code of the operation


