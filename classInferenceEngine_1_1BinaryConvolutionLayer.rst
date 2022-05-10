.. index:: pair: class; InferenceEngine::BinaryConvolutionLayer
.. _doxid-class_inference_engine_1_1_binary_convolution_layer:

class InferenceEngine::BinaryConvolutionLayer
=============================================

.. toctree::
	:hidden:

	eBinaryConvolutionMode <enumInferenceEngine_1_1BinaryConvolutionLayer_1_1eBinaryConvolutionMode.rst>

Overview
~~~~~~~~

This class represents a standard binary convolution layer. :ref:`More...<details-class_inference_engine_1_1_binary_convolution_layer>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	class BinaryConvolutionLayer: public :ref:`InferenceEngine::WeightableLayer<doxid-class_inference_engine_1_1_weightable_layer>`
	{
	public:
		// enums
	
		enum :ref:`eBinaryConvolutionMode<doxid-class_inference_engine_1_1_binary_convolution_layer_1a62b4ca5b6db8a5fc8f06caac0503e6cd>`;

		// fields
	
		:ref:`eBinaryConvolutionMode<doxid-class_inference_engine_1_1_binary_convolution_layer_1a62b4ca5b6db8a5fc8f06caac0503e6cd>` :ref:`_mode<doxid-class_inference_engine_1_1_binary_convolution_layer_1ad6ddf090e531f2972774aade66bf0a9a>` = :ref:`xnor_popcount<doxid-class_inference_engine_1_1_binary_convolution_layer_1a62b4ca5b6db8a5fc8f06caac0503e6cdae1c5e2fcdba96e52f4ce0c01b3a180d5>`;
		unsigned int :ref:`_in_depth<doxid-class_inference_engine_1_1_binary_convolution_layer_1af7721d119590aa33b88eea9f41a433da>` = 0u;
		float :ref:`_pad_value<doxid-class_inference_engine_1_1_binary_convolution_layer_1a072cc6e1c87f30465c88991a5a9539f4>` = 0.0f;
		:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> :ref:`_kernel<doxid-class_inference_engine_1_1_binary_convolution_layer_1af172cb05dc9eacac7ce823e1a4a84f70>`;
		unsigned int& :target:`_kernel_x<doxid-class_inference_engine_1_1_binary_convolution_layer_1a40310ee3cf047deffd81557fd93ff68f>` =  :ref:`_kernel<doxid-class_inference_engine_1_1_binary_convolution_layer_1af172cb05dc9eacac7ce823e1a4a84f70>` .at(:ref:`X_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0a123219f421934427910f3c8080f76bcc>`);
		unsigned int& :target:`_kernel_y<doxid-class_inference_engine_1_1_binary_convolution_layer_1acc998e306cf33b319a14979f174aa416>` =  :ref:`_kernel<doxid-class_inference_engine_1_1_binary_convolution_layer_1af172cb05dc9eacac7ce823e1a4a84f70>` .at(:ref:`Y_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0aa5a4fe3bd008bfa81437359c246b0b24>`);
		:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> :ref:`_padding<doxid-class_inference_engine_1_1_binary_convolution_layer_1a32f6f87453d76c6d76cfa82ff965ea48>`;
		unsigned int& :target:`_padding_x<doxid-class_inference_engine_1_1_binary_convolution_layer_1a4843ac3cb3b431b1a74f4180994f5c61>` =  :ref:`_padding<doxid-class_inference_engine_1_1_binary_convolution_layer_1a32f6f87453d76c6d76cfa82ff965ea48>` .at(:ref:`X_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0a123219f421934427910f3c8080f76bcc>`);
		unsigned int& :target:`_padding_y<doxid-class_inference_engine_1_1_binary_convolution_layer_1a22e1df5a10b13bdbe5c656b821f63697>` =  :ref:`_padding<doxid-class_inference_engine_1_1_binary_convolution_layer_1a32f6f87453d76c6d76cfa82ff965ea48>` .at(:ref:`Y_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0aa5a4fe3bd008bfa81437359c246b0b24>`);
		:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> :ref:`_pads_end<doxid-class_inference_engine_1_1_binary_convolution_layer_1a4992be6c44eda6288e4f8e9828c80e00>`;
		:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> :ref:`_stride<doxid-class_inference_engine_1_1_binary_convolution_layer_1aacda5c3d6a9a2e783e32a7ad7a437da6>`;
		unsigned int& :target:`_stride_x<doxid-class_inference_engine_1_1_binary_convolution_layer_1a4f6eafff9f47e04cbab32e7cb50c14f8>` =  :ref:`_stride<doxid-class_inference_engine_1_1_binary_convolution_layer_1aacda5c3d6a9a2e783e32a7ad7a437da6>` .at(:ref:`X_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0a123219f421934427910f3c8080f76bcc>`);
		unsigned int& :target:`_stride_y<doxid-class_inference_engine_1_1_binary_convolution_layer_1af96a2868608717afa3218dbdd3790fb1>` =  :ref:`_stride<doxid-class_inference_engine_1_1_binary_convolution_layer_1aacda5c3d6a9a2e783e32a7ad7a437da6>` .at(:ref:`Y_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0aa5a4fe3bd008bfa81437359c246b0b24>`);
		:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> :ref:`_dilation<doxid-class_inference_engine_1_1_binary_convolution_layer_1a797a1069cd9e79f42778a9d372e19ee0>`;
		unsigned int& :target:`_dilation_x<doxid-class_inference_engine_1_1_binary_convolution_layer_1a24370e81b13a7246c31d31676e33e9dc>` =  :ref:`_dilation<doxid-class_inference_engine_1_1_binary_convolution_layer_1a797a1069cd9e79f42778a9d372e19ee0>` .at(:ref:`X_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0a123219f421934427910f3c8080f76bcc>`);
		unsigned int& :target:`_dilation_y<doxid-class_inference_engine_1_1_binary_convolution_layer_1a426c06b1838ef9d12dbaa782c4690b6b>` =  :ref:`_dilation<doxid-class_inference_engine_1_1_binary_convolution_layer_1a797a1069cd9e79f42778a9d372e19ee0>` .at(:ref:`Y_AXIS<doxid-namespace_inference_engine_1a699af6f18afedf57e765e099645728f0aa5a4fe3bd008bfa81437359c246b0b24>`);
		unsigned int :ref:`_out_depth<doxid-class_inference_engine_1_1_binary_convolution_layer_1a5c094f2788aae7b06f0f1debd847d217>` = 0u;
		unsigned int :ref:`_group<doxid-class_inference_engine_1_1_binary_convolution_layer_1adc7693b880bfe931b187d94707c5e844>` = 1u;
		std::string :ref:`_auto_pad<doxid-class_inference_engine_1_1_binary_convolution_layer_1aca4de0fa2f22bb3370e81908c7b96c4c>`;

		// construction
	
		:ref:`BinaryConvolutionLayer<doxid-class_inference_engine_1_1_binary_convolution_layer_1a8457cd5b871fb0aef480b38e81448d50>`(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& p);
		:ref:`BinaryConvolutionLayer<doxid-class_inference_engine_1_1_binary_convolution_layer_1a2a94a9ac8b79929663c0ce6d044419aa>`(const BinaryConvolutionLayer& that);
		:ref:`BinaryConvolutionLayer<doxid-class_inference_engine_1_1_binary_convolution_layer_1a4a3930440061c1da96b039245da023bd>`(BinaryConvolutionLayer&&);

		// methods
	
		BinaryConvolutionLayer& :ref:`operator =<doxid-class_inference_engine_1_1_binary_convolution_layer_1ade502d9a2b7bec9e7f839b6d417bca09>` (const BinaryConvolutionLayer& that);
	};

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
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`_weights<doxid-class_inference_engine_1_1_weightable_layer_1a5088fb7b2f358e3a89f6628e8e2f1e45>`;
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`_biases<doxid-class_inference_engine_1_1_weightable_layer_1a8bdb867bf51ee5ce94395ed0d5c8bc2c>`;

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
		:ref:`CNNLayer<doxid-class_inference_engine_1_1_weightable_layer_1a49576b4ff390822c0aa474cf7f542724>`(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& prms);
		:ref:`CNNLayer<doxid-class_inference_engine_1_1_weightable_layer_1ad5d08d211ac7bb10a79a1e4dc66551fa>`(const :ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer>`& other);

.. _details-class_inference_engine_1_1_binary_convolution_layer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents a standard binary convolution layer.

Deprecated Migrate to IR v10 and work with :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` directly. The method will be removed in 2021.1

Fields
------

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1ad6ddf090e531f2972774aade66bf0a9a:
.. index:: pair: variable; _mode

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`eBinaryConvolutionMode<doxid-class_inference_engine_1_1_binary_convolution_layer_1a62b4ca5b6db8a5fc8f06caac0503e6cd>` _mode = :ref:`xnor_popcount<doxid-class_inference_engine_1_1_binary_convolution_layer_1a62b4ca5b6db8a5fc8f06caac0503e6cdae1c5e2fcdba96e52f4ce0c01b3a180d5>`

Mode of binary convolution operation.

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1af7721d119590aa33b88eea9f41a433da:
.. index:: pair: variable; _in_depth

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int _in_depth = 0u

A number of input feature maps (size) generating the 3'rd input dimension.

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a072cc6e1c87f30465c88991a5a9539f4:
.. index:: pair: variable; _pad_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float _pad_value = 0.0f

A pad value which is used to fill pad area.

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1af172cb05dc9eacac7ce823e1a4a84f70:
.. index:: pair: variable; _kernel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> _kernel

A convolution kernel array [X, Y, Z, ...].

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a32f6f87453d76c6d76cfa82ff965ea48:
.. index:: pair: variable; _padding

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> _padding

A convolution paddings begin array [X, Y, Z, ...].

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a4992be6c44eda6288e4f8e9828c80e00:
.. index:: pair: variable; _pads_end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> _pads_end

A convolution paddings end array [X, Y, Z, ...].

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1aacda5c3d6a9a2e783e32a7ad7a437da6:
.. index:: pair: variable; _stride

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> _stride

A convolution strides array [X, Y, Z, ...].

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a797a1069cd9e79f42778a9d372e19ee0:
.. index:: pair: variable; _dilation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PropertyVector<doxid-class_inference_engine_1_1_property_vector>`<unsigned int> _dilation

A convolution dilations array [X, Y, Z, ...].

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a5c094f2788aae7b06f0f1debd847d217:
.. index:: pair: variable; _out_depth

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int _out_depth = 0u

A number of output feature maps (size) generating the 3'rd output dimension.

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1adc7693b880bfe931b187d94707c5e844:
.. index:: pair: variable; _group

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int _group = 1u

Number of groups.

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1aca4de0fa2f22bb3370e81908c7b96c4c:
.. index:: pair: variable; _auto_pad

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string _auto_pad

Auto padding type.

Construction
------------

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a8457cd5b871fb0aef480b38e81448d50:
.. index:: pair: function; BinaryConvolutionLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BinaryConvolutionLayer(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& p)

Creates a new :ref:`BinaryConvolutionLayer <doxid-class_inference_engine_1_1_binary_convolution_layer>` instance.

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a2a94a9ac8b79929663c0ce6d044419aa:
.. index:: pair: function; BinaryConvolutionLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BinaryConvolutionLayer(const BinaryConvolutionLayer& that)

copy constructor

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1a4a3930440061c1da96b039245da023bd:
.. index:: pair: function; BinaryConvolutionLayer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BinaryConvolutionLayer(BinaryConvolutionLayer&&)

move constructor

Methods
-------

.. _doxid-class_inference_engine_1_1_binary_convolution_layer_1ade502d9a2b7bec9e7f839b6d417bca09:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BinaryConvolutionLayer& operator = (const BinaryConvolutionLayer& that)

assignment operator


