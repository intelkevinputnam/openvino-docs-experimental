.. index:: pair: class; InferenceEngine::CNNLayer
.. _doxid-class_inference_engine_1_1_c_n_n_layer:

class InferenceEngine::CNNLayer
===============================



Overview
~~~~~~~~

This is a base abstraction Layer - all DNN Layers inherit from this class. :ref:`More...<details-class_inference_engine_1_1_c_n_n_layer>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	class CNNLayer
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<CNNLayer> :ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>`;

		// fields
	
		std::string :ref:`name<doxid-class_inference_engine_1_1_c_n_n_layer_1a20185b71c3006edeef34337660c63e50>`;
		std::string :ref:`type<doxid-class_inference_engine_1_1_c_n_n_layer_1ac212155e7134b88e70eb244ffb03d079>`;
		:ref:`Precision<doxid-class_inference_engine_1_1_precision>` :ref:`precision<doxid-class_inference_engine_1_1_c_n_n_layer_1a4e644a73e430f608faa8dc33c1ccab5b>`;
		std::vector<:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`> :ref:`outData<doxid-class_inference_engine_1_1_c_n_n_layer_1a6071e2163a4fef32de72c6ab22129224>`;
		std::vector<:ref:`DataWeakPtr<doxid-namespace_inference_engine_1af7e08b740f8da0ef826644aca39cb2ce>`> :ref:`insData<doxid-class_inference_engine_1_1_c_n_n_layer_1a1053f3f44f7492f79d755c8afe1e83b7>`;
		:ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>` :ref:`_fusedWith<doxid-class_inference_engine_1_1_c_n_n_layer_1ac25a960c7c95a63bdce49c935363c9c0>`;
		:ref:`UserValue<doxid-union_inference_engine_1_1_user_value>` :ref:`userValue<doxid-class_inference_engine_1_1_c_n_n_layer_1a62f7fc6af3a34b8b069025bfed12f37d>`;
		std::string :ref:`affinity<doxid-class_inference_engine_1_1_c_n_n_layer_1ae584c7bc3017655c20b7c5fb4501d5ab>`;
		std::map<std::string, std::string> :ref:`params<doxid-class_inference_engine_1_1_c_n_n_layer_1a06b085fdd9e498d9acde167efc2ad811>`;
		std::map<std::string, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`> :ref:`blobs<doxid-class_inference_engine_1_1_c_n_n_layer_1aeafc49f9cd3bcb98d7a3c7e66a4bf285>`;

		// construction
	
		:ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer_1a49576b4ff390822c0aa474cf7f542724>`(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& prms);
		:ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer_1ad5d08d211ac7bb10a79a1e4dc66551fa>`(const CNNLayer& other);

		// methods
	
		std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :ref:`getNode<doxid-class_inference_engine_1_1_c_n_n_layer_1a322989d3de69b2cc51c90bf1271968a9>`() const;
		void :ref:`fuse<doxid-class_inference_engine_1_1_c_n_n_layer_1a12aad4318ec1bab134f61c2b7c591cc6>`(:ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>`& layer);
		virtual const :ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>` :ref:`input<doxid-class_inference_engine_1_1_c_n_n_layer_1a864d9dcd5ec644df5794b0ac5f47af5f>`() const;
		void :ref:`parseParams<doxid-class_inference_engine_1_1_c_n_n_layer_1a8132f27c4963fa58ad131d6a6989c94e>`();
		float :ref:`GetParamAsFloat<doxid-class_inference_engine_1_1_c_n_n_layer_1a3891f1326149a9d2f1566bf2a851f643>`(const char \* param, float def) const;
		float :ref:`GetParamAsFloat<doxid-class_inference_engine_1_1_c_n_n_layer_1a42c3d84f598675eec55a6d28620b8e76>`(const char \* param) const;
		std::vector<float> :ref:`GetParamAsFloats<doxid-class_inference_engine_1_1_c_n_n_layer_1af9630456abcf9859a16a9517277fdd1f>`(const char \* param, std::vector<float> def) const;
		std::vector<float> :ref:`GetParamAsFloats<doxid-class_inference_engine_1_1_c_n_n_layer_1ae32218245c3bc781dc0a7a979bba2042>`(const char \* param) const;
		int :ref:`GetParamAsInt<doxid-class_inference_engine_1_1_c_n_n_layer_1af0340b5d83e0ca68dfbe9daa4d0d7f19>`(const char \* param, int def) const;
		int :ref:`GetParamAsInt<doxid-class_inference_engine_1_1_c_n_n_layer_1aea5ce11db18674d6b16cd57a974bca43>`(const char \* param) const;
		std::vector<int> :ref:`GetParamAsInts<doxid-class_inference_engine_1_1_c_n_n_layer_1ac6b05057bc37550e977d96f6b296dbed>`(const char \* param, std::vector<int> def) const;
		std::vector<int> :ref:`GetParamAsInts<doxid-class_inference_engine_1_1_c_n_n_layer_1a4e1abf89c200819f8988c4e6687d2c1b>`(const char \* param) const;
		unsigned int :ref:`GetParamAsUInt<doxid-class_inference_engine_1_1_c_n_n_layer_1a58afa0776016b852ec2d943d22627c69>`(const char \* param, unsigned int def) const;
		unsigned int :ref:`GetParamAsUInt<doxid-class_inference_engine_1_1_c_n_n_layer_1a95639231097406556bdca71eb92656a0>`(const char \* param) const;
		size_t :ref:`GetParamAsSizeT<doxid-class_inference_engine_1_1_c_n_n_layer_1a1e567514c1b6c26ebc2c6f5322c1e531>`(const char \* param, size_t def) const;
		size_t :ref:`GetParamAsSizeT<doxid-class_inference_engine_1_1_c_n_n_layer_1a704d80308a7a023a89c48eea2b439b3c>`(const char \* param) const;
	
		std::vector<unsigned int> :ref:`GetParamAsUInts<doxid-class_inference_engine_1_1_c_n_n_layer_1a3567558e080c9c25ca1414551d1c163e>`(
			const char \* param,
			std::vector<unsigned int> def
			) const;
	
		std::vector<unsigned int> :ref:`GetParamAsUInts<doxid-class_inference_engine_1_1_c_n_n_layer_1af6b6e33dea3e48a4ae2609bb7ad6d7b2>`(const char \* param) const;
		bool :ref:`GetParamAsBool<doxid-class_inference_engine_1_1_c_n_n_layer_1a3806906c9780ba527bb46651b01e1194>`(const char \* param, bool def) const;
		bool :ref:`GetParamAsBool<doxid-class_inference_engine_1_1_c_n_n_layer_1aa0fc4eec06f791d26dde3a47fca9dfb4>`(const char \* param) const;
		std::string :ref:`GetParamAsString<doxid-class_inference_engine_1_1_c_n_n_layer_1ae07e0a086ce4e02b5fb4600c34c4543e>`(const char \* param, const char \* def) const;
		bool :ref:`CheckParamPresence<doxid-class_inference_engine_1_1_c_n_n_layer_1a54353d851f4e017c3ea547ed12e4f73d>`(const char \* param) const;
		std::string :ref:`GetParamAsString<doxid-class_inference_engine_1_1_c_n_n_layer_1a69d26fd97bf9366d1d5028671e09b450>`(const char \* param) const;
		std::string :ref:`getBoolStrParamAsIntStr<doxid-class_inference_engine_1_1_c_n_n_layer_1a6ec29efe57d6a756efd660c9e5f8b688>`(const char \* param) const;
	
		std::vector<std::string> :ref:`GetParamAsStrings<doxid-class_inference_engine_1_1_c_n_n_layer_1a2cffea1440266959a91b6cee38e4fca0>`(
			const char \* param,
			std::vector<std::string> def
			) const;
	
		static float :ref:`ie_parse_float<doxid-class_inference_engine_1_1_c_n_n_layer_1a830772b08ab5b0f7f6defa7317e33783>`(const std::string& str);
		static std::string :ref:`ie_serialize_float<doxid-class_inference_engine_1_1_c_n_n_layer_1afe311c770dd17382996880052d303bc8>`(float value);
	};

	// direct descendants

	class :ref:`BatchToSpaceLayer<doxid-class_inference_engine_1_1_batch_to_space_layer>`;
	class :ref:`BroadcastLayer<doxid-class_inference_engine_1_1_broadcast_layer>`;
	class :ref:`BucketizeLayer<doxid-class_inference_engine_1_1_bucketize_layer>`;
	class :ref:`ClampLayer<doxid-class_inference_engine_1_1_clamp_layer>`;
	class :ref:`ConcatLayer<doxid-class_inference_engine_1_1_concat_layer>`;
	class :ref:`CropLayer<doxid-class_inference_engine_1_1_crop_layer>`;
	class :ref:`DepthToSpaceLayer<doxid-class_inference_engine_1_1_depth_to_space_layer>`;
	class :ref:`EltwiseLayer<doxid-class_inference_engine_1_1_eltwise_layer>`;
	class :ref:`ExperimentalDetectronGenerateProposalsSingleImageLayer<doxid-class_inference_engine_1_1_experimental_detectron_generate_proposals_single_image_layer>`;
	class :ref:`ExperimentalDetectronPriorGridGeneratorLayer<doxid-class_inference_engine_1_1_experimental_detectron_prior_grid_generator_layer>`;
	class :ref:`ExperimentalDetectronTopKROIs<doxid-class_inference_engine_1_1_experimental_detectron_top_k_r_o_is>`;
	class :ref:`ExperimentalSparseWeightedReduceLayer<doxid-class_inference_engine_1_1_experimental_sparse_weighted_reduce_layer>`;
	class :ref:`FillLayer<doxid-class_inference_engine_1_1_fill_layer>`;
	class :ref:`GatherLayer<doxid-class_inference_engine_1_1_gather_layer>`;
	class :ref:`GemmLayer<doxid-class_inference_engine_1_1_gemm_layer>`;
	class :ref:`GRNLayer<doxid-class_inference_engine_1_1_g_r_n_layer>`;
	class :ref:`MathLayer<doxid-class_inference_engine_1_1_math_layer>`;
	class :ref:`MVNLayer<doxid-class_inference_engine_1_1_m_v_n_layer>`;
	class :ref:`NonMaxSuppressionLayer<doxid-class_inference_engine_1_1_non_max_suppression_layer>`;
	class :ref:`NormLayer<doxid-class_inference_engine_1_1_norm_layer>`;
	class :ref:`OneHotLayer<doxid-class_inference_engine_1_1_one_hot_layer>`;
	class :ref:`PadLayer<doxid-class_inference_engine_1_1_pad_layer>`;
	class :ref:`PoolingLayer<doxid-class_inference_engine_1_1_pooling_layer>`;
	class :ref:`PowerLayer<doxid-class_inference_engine_1_1_power_layer>`;
	class :ref:`QuantizeLayer<doxid-class_inference_engine_1_1_quantize_layer>`;
	class :ref:`RangeLayer<doxid-class_inference_engine_1_1_range_layer>`;
	class :ref:`ReduceLayer<doxid-class_inference_engine_1_1_reduce_layer>`;
	class :ref:`ReLULayer<doxid-class_inference_engine_1_1_re_l_u_layer>`;
	class :ref:`ReshapeLayer<doxid-class_inference_engine_1_1_reshape_layer>`;
	class :ref:`ReverseSequenceLayer<doxid-class_inference_engine_1_1_reverse_sequence_layer>`;
	class :ref:`ScatterElementsUpdateLayer<doxid-class_inference_engine_1_1_scatter_elements_update_layer>`;
	class :ref:`ScatterUpdateLayer<doxid-class_inference_engine_1_1_scatter_update_layer>`;
	class :ref:`SelectLayer<doxid-class_inference_engine_1_1_select_layer>`;
	class :ref:`ShuffleChannelsLayer<doxid-class_inference_engine_1_1_shuffle_channels_layer>`;
	class :ref:`SoftMaxLayer<doxid-class_inference_engine_1_1_soft_max_layer>`;
	class :ref:`SpaceToBatchLayer<doxid-class_inference_engine_1_1_space_to_batch_layer>`;
	class :ref:`SpaceToDepthLayer<doxid-class_inference_engine_1_1_space_to_depth_layer>`;
	class :ref:`SparseFillEmptyRowsLayer<doxid-class_inference_engine_1_1_sparse_fill_empty_rows_layer>`;
	class :ref:`SparseSegmentReduceLayer<doxid-class_inference_engine_1_1_sparse_segment_reduce_layer>`;
	class :ref:`SparseToDenseLayer<doxid-class_inference_engine_1_1_sparse_to_dense_layer>`;
	class :ref:`SplitLayer<doxid-class_inference_engine_1_1_split_layer>`;
	class :ref:`StridedSliceLayer<doxid-class_inference_engine_1_1_strided_slice_layer>`;
	class :ref:`TensorIterator<doxid-class_inference_engine_1_1_tensor_iterator>`;
	class :ref:`TileLayer<doxid-class_inference_engine_1_1_tile_layer>`;
	class :ref:`TopKLayer<doxid-class_inference_engine_1_1_top_k_layer>`;
	class :ref:`UniqueLayer<doxid-class_inference_engine_1_1_unique_layer>`;
	class :ref:`WeightableLayer<doxid-class_inference_engine_1_1_weightable_layer>`;
.. _details-class_inference_engine_1_1_c_n_n_layer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is a base abstraction Layer - all DNN Layers inherit from this class.

Deprecated Migrate to IR v10 and work with :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` directly. The method will be removed in 2021.1

Typedefs
--------

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<CNNLayer> Ptr

A shared pointer to :ref:`CNNLayer <doxid-class_inference_engine_1_1_c_n_n_layer>`.

Fields
------

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a20185b71c3006edeef34337660c63e50:
.. index:: pair: variable; name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string name

Layer name.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ac212155e7134b88e70eb244ffb03d079:
.. index:: pair: variable; type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string type

Layer type.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a4e644a73e430f608faa8dc33c1ccab5b:
.. index:: pair: variable; precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Precision<doxid-class_inference_engine_1_1_precision>` precision

Layer base operating precision.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a6071e2163a4fef32de72c6ab22129224:
.. index:: pair: variable; outData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>`> outData

A vector of pointers to the output data elements of this layer in the di-graph (order matters)

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a1053f3f44f7492f79d755c8afe1e83b7:
.. index:: pair: variable; insData

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`DataWeakPtr<doxid-namespace_inference_engine_1af7e08b740f8da0ef826644aca39cb2ce>`> insData

A vector of weak pointers to the input data elements of this layer in the di-graph (order matters)

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ac25a960c7c95a63bdce49c935363c9c0:
.. index:: pair: variable; _fusedWith

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>` _fusedWith

If suggested to fuse - a pointer to the layer which needs to be fused with this layer.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a62f7fc6af3a34b8b069025bfed12f37d:
.. index:: pair: variable; userValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`UserValue<doxid-union_inference_engine_1_1_user_value>` userValue

Convenience user values to store in this object as extra data.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ae584c7bc3017655c20b7c5fb4501d5ab:
.. index:: pair: variable; affinity

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string affinity

Layer affinity set by user.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a06b085fdd9e498d9acde167efc2ad811:
.. index:: pair: variable; params

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, std::string> params

Map of pairs: (parameter name, parameter value)

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1aeafc49f9cd3bcb98d7a3c7e66a4bf285:
.. index:: pair: variable; blobs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`> blobs

Map of pairs: (name, weights/biases blob)

Construction
------------

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a49576b4ff390822c0aa474cf7f542724:
.. index:: pair: function; CNNLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNLayer(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& prms)

A constructor. Creates a new :ref:`CNNLayer <doxid-class_inference_engine_1_1_c_n_n_layer>` instance and initializes layer parameters with the given values.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prms

		- Basic common parsing parameters

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ad5d08d211ac7bb10a79a1e4dc66551fa:
.. index:: pair: function; CNNLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNLayer(const CNNLayer& other)

A copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- An object to copy

Methods
-------

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a322989d3de69b2cc51c90bf1271968a9:
.. index:: pair: function; getNode

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> getNode() const

Returns the original nGraph op.



.. rubric:: Returns:

A smart pointer to nGraph op

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a12aad4318ec1bab134f61c2b7c591cc6:
.. index:: pair: function; fuse

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void fuse(:ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>`& layer)

Sets a layer to be fused with.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layer

		- Reference to the layer to be fused with

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a864d9dcd5ec644df5794b0ac5f47af5f:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`DataPtr<doxid-namespace_inference_engine_1a91f97c826d2753815815c119ba383e63>` input() const

Returns the first element of the input data for this layer.



.. rubric:: Returns:

A smart pointer to the input data element

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a8132f27c4963fa58ad131d6a6989c94e:
.. index:: pair: function; parseParams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void parseParams()

Checks if the input data and layer data are legitimate.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a3891f1326149a9d2f1566bf2a851f643:
.. index:: pair: function; GetParamAsFloat

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float GetParamAsFloat(const char \* param, float def) const

Gets float value for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- name of the parameter to find

	*
		- def

		- default value of the parameter if not found



.. rubric:: Returns:

float value

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a42c3d84f598675eec55a6d28620b8e76:
.. index:: pair: function; GetParamAsFloat

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float GetParamAsFloat(const char \* param) const

Returns a float value for the given layer parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

A float value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1af9630456abcf9859a16a9517277fdd1f:
.. index:: pair: function; GetParamAsFloats

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<float> GetParamAsFloats(const char \* param, std::vector<float> def) const

Returns a vector of float values for the given parameter or returns the default value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

vector of float values

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ae32218245c3bc781dc0a7a979bba2042:
.. index:: pair: function; GetParamAsFloats

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<float> GetParamAsFloats(const char \* param) const

Returns a vector of float values for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

vector of float values

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1af0340b5d83e0ca68dfbe9daa4d0d7f19:
.. index:: pair: function; GetParamAsInt

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int GetParamAsInt(const char \* param, int def) const

Returns an integer value for the given parameter or returns the default value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

An int value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1aea5ce11db18674d6b16cd57a974bca43:
.. index:: pair: function; GetParamAsInt

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int GetParamAsInt(const char \* param) const

Returns an integer value for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

An int value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ac6b05057bc37550e977d96f6b296dbed:
.. index:: pair: function; GetParamAsInts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> GetParamAsInts(const char \* param, std::vector<int> def) const

Returns a vector of int values for the given parameter or returns the default value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

vector of int values

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a4e1abf89c200819f8988c4e6687d2c1b:
.. index:: pair: function; GetParamAsInts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> GetParamAsInts(const char \* param) const

Returns a vector of int values for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

vector of int values

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a58afa0776016b852ec2d943d22627c69:
.. index:: pair: function; GetParamAsUInt

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int GetParamAsUInt(const char \* param, unsigned int def) const

Returns an unsigned integer value for the given parameter or returns the default value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

An unsigned integer value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a95639231097406556bdca71eb92656a0:
.. index:: pair: function; GetParamAsUInt

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int GetParamAsUInt(const char \* param) const

Returns an unsigned integer value for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

An unsigned integer value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a1e567514c1b6c26ebc2c6f5322c1e531:
.. index:: pair: function; GetParamAsSizeT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t GetParamAsSizeT(const char \* param, size_t def) const

Returns an size_t value for the given parameter or returns the default value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

An size_t value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a704d80308a7a023a89c48eea2b439b3c:
.. index:: pair: function; GetParamAsSizeT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t GetParamAsSizeT(const char \* param) const

Returns an size_t value for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

An size_t value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a3567558e080c9c25ca1414551d1c163e:
.. index:: pair: function; GetParamAsUInts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<unsigned int> GetParamAsUInts(
		const char \* param,
		std::vector<unsigned int> def
		) const

Returns a vector of unsigned int values for the given parameter or returns the default value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

vector of unsigned int values

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1af6b6e33dea3e48a4ae2609bb7ad6d7b2:
.. index:: pair: function; GetParamAsUInts

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<unsigned int> GetParamAsUInts(const char \* param) const

Returns a vector of unsigned int values for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

vector of unsigned int values

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a3806906c9780ba527bb46651b01e1194:
.. index:: pair: function; GetParamAsBool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool GetParamAsBool(const char \* param, bool def) const

Returns a boolean value for the given parameter.

The valid values are (true, false, 1, 0).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

A bool value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1aa0fc4eec06f791d26dde3a47fca9dfb4:
.. index:: pair: function; GetParamAsBool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool GetParamAsBool(const char \* param) const

Returns a boolean value for the given parameter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

A bool value for the specified parameter

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1ae07e0a086ce4e02b5fb4600c34c4543e:
.. index:: pair: function; GetParamAsString

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string GetParamAsString(const char \* param, const char \* def) const

Returns a string value for the given parameter or returns the default one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter

	*
		- def

		- Default value of the parameter if not found



.. rubric:: Returns:

A string value

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a54353d851f4e017c3ea547ed12e4f73d:
.. index:: pair: function; CheckParamPresence

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool CheckParamPresence(const char \* param) const

Checks the param presence in the layer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

a bool depending param presence

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a69d26fd97bf9366d1d5028671e09b450:
.. index:: pair: function; GetParamAsString

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string GetParamAsString(const char \* param) const

Returns a string value for the given parameter.

Throws exception if parameter was not found.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

A string value

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a6ec29efe57d6a756efd660c9e5f8b688:
.. index:: pair: function; getBoolStrParamAsIntStr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getBoolStrParamAsIntStr(const char \* param) const

Returns a string containing an integer if parameters value was "true" or "false".



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Name of the layer parameter



.. rubric:: Returns:

A string containing an integer or the parameter as string

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a2cffea1440266959a91b6cee38e4fca0:
.. index:: pair: function; GetParamAsStrings

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> GetParamAsStrings(
		const char \* param,
		std::vector<std::string> def
		) const

Gets the parameter as a std::vector<std::string>



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- The parameter name

	*
		- def

		- The default values if case of parameter is not found



.. rubric:: Returns:

The parameter as strings.

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1a830772b08ab5b0f7f6defa7317e33783:
.. index:: pair: function; ie_parse_float

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static float ie_parse_float(const std::string& str)

Parse string with float in accordance with IE rules.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- str

		- input string with float value

	*
		- :ref:`Exception <doxid-struct_inference_engine_1_1_exception>`

		- in case of parsing error



.. rubric:: Returns:

float value if parsing was successful

.. _doxid-class_inference_engine_1_1_c_n_n_layer_1afe311c770dd17382996880052d303bc8:
.. index:: pair: function; ie_serialize_float

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::string ie_serialize_float(float value)

serialize float with c_locale formating used for default values serializing


