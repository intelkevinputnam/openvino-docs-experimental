.. index:: pair: class; InferenceEngine::ClampLayer
.. _doxid-class_inference_engine_1_1_clamp_layer:

class InferenceEngine::ClampLayer
=================================



Overview
~~~~~~~~

This class represents a Clamp activation layer. :ref:`More...<details-class_inference_engine_1_1_clamp_layer>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	class ClampLayer: public :ref:`InferenceEngine::CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer>`
	{
	public:
		// fields
	
		float :ref:`min_value<doxid-class_inference_engine_1_1_clamp_layer_1a7bc1451ca7c2185567e27d919a8ebd54>` = 0.0f;
		float :ref:`max_value<doxid-class_inference_engine_1_1_clamp_layer_1a94a54430abcb0eff0ff7b73d89fbd76f>` = 1.0f;

		// methods
	
		:ref:`CNNLayer<doxid-class_inference_engine_1_1_clamp_layer_1a49576b4ff390822c0aa474cf7f542724>`(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& prms);
		:ref:`CNNLayer<doxid-class_inference_engine_1_1_clamp_layer_1ad5d08d211ac7bb10a79a1e4dc66551fa>`(const :ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer>`& other);
	};

	// direct descendants

	class :ref:`ReLU6Layer<doxid-class_inference_engine_1_1_re_l_u6_layer>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer>`> :ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>`;

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

.. _details-class_inference_engine_1_1_clamp_layer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents a Clamp activation layer.

Deprecated Migrate to IR v10 and work with :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` directly. The method will be removed in 2021.1

Clamps all tensor elements into the range [min_value, max_value]

Fields
------

.. _doxid-class_inference_engine_1_1_clamp_layer_1a7bc1451ca7c2185567e27d919a8ebd54:
.. index:: pair: variable; min_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float min_value = 0.0f

A minimum value.

.. _doxid-class_inference_engine_1_1_clamp_layer_1a94a54430abcb0eff0ff7b73d89fbd76f:
.. index:: pair: variable; max_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float max_value = 1.0f

A maximum value.

Methods
-------

.. _doxid-class_inference_engine_1_1_clamp_layer_1a49576b4ff390822c0aa474cf7f542724:
.. index:: pair: function; CNNLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNLayer(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& prms)

Creates a new :ref:`ClampLayer <doxid-class_inference_engine_1_1_clamp_layer>` instance.

.. _doxid-class_inference_engine_1_1_clamp_layer_1ad5d08d211ac7bb10a79a1e4dc66551fa:
.. index:: pair: function; CNNLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNNLayer(const :ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer>`& other)

Creates a new :ref:`ClampLayer <doxid-class_inference_engine_1_1_clamp_layer>` instance.


