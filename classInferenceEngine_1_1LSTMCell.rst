.. index:: pair: class; InferenceEngine::LSTMCell
.. _doxid-class_inference_engine_1_1_l_s_t_m_cell:

class InferenceEngine::LSTMCell
===============================



Overview
~~~~~~~~

LSTM Cell layer. :ref:`More...<details-class_inference_engine_1_1_l_s_t_m_cell>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	class LSTMCell: public :ref:`InferenceEngine::RNNCellBase<doxid-class_inference_engine_1_1_r_n_n_cell_base>`
	{
	public:
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`CNNLayer<doxid-class_inference_engine_1_1_c_n_n_layer>`> :ref:`Ptr<doxid-class_inference_engine_1_1_c_n_n_layer_1ae6c5b3bbb31997571de2ff36ea4dfee3>`;

		// enums
	
		enum :ref:`CellType<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3>`;

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
		:ref:`CellType<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3>` :ref:`cellType<doxid-class_inference_engine_1_1_r_n_n_cell_base_1a9cb69322ce7d3504c5211350fe198f5b>` = :ref:`LSTM<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a910000de786e7fcdc257fbd01a0559a8>`;
		int :ref:`hidden_size<doxid-class_inference_engine_1_1_r_n_n_cell_base_1a372a96b7faf1fed6f166ebb75e1b3a8b>` = 0;
		float :ref:`clip<doxid-class_inference_engine_1_1_r_n_n_cell_base_1a85730fb0fbeb104f992996d41f30fb34>` = 0.0f;
		std::vector<std::string> :ref:`activations<doxid-class_inference_engine_1_1_r_n_n_cell_base_1a33312ada8536f75beed320bf48dbd7fb>`;
		std::vector<float> :ref:`activation_alpha<doxid-class_inference_engine_1_1_r_n_n_cell_base_1abe001666ce9d23ec26e83c43a89b9d5c>`;
		std::vector<float> :ref:`activation_beta<doxid-class_inference_engine_1_1_r_n_n_cell_base_1a4249f3eb74394ea297808e0437ee5e5c>`;

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
		:ref:`WeightableLayer<doxid-class_inference_engine_1_1_r_n_n_cell_base_1a30d257b68499e9a5ab472989958c67b1>`(const :ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params>`& prms);

.. _details-class_inference_engine_1_1_l_s_t_m_cell:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

LSTM Cell layer.

Deprecated Migrate to IR v10 and work with :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` directly. The method will be removed in 2021.1

:ref:`G <doxid-namespace_inference_engine_1_1_g>` - number of gates (=4) N - batch size S - state size (=hidden_size)

Inputs: [N,D] Xt - input data [N,S] Ht-1 - initial hidden state [N,S] Ct-1 - initial cell state

Outputs: [N,S] Ht - out hidden state [N,S] Ct - out cell state

Weights:

* weights [:ref:`G <doxid-namespace_inference_engine_1_1_g>`,S,D+S]

* biases [:ref:`G <doxid-namespace_inference_engine_1_1_g>`,S] NB! gates order is FICO {forget, input, candidate, output}

activations is {_f, _g, _h} default: {_f=sigm, _g=tanh, _h=tanh}

Equations:

* - matrix mult (.) - eltwise mult [,] - concatenation

ft = _f(Wf\*[Ht-1, Xt] + Bf)

* it = _f(Wi\*[Ht-1, Xt] + Bi)

* ct = _g(Wc\*[Ht-1, Xt] + Bc)

* ot = _f(Wo\*[Ht-1, Xt] + Bo)

* Ct = ft (.) Ct-1 + it (.) ct

* Ht = ot (.) _h(Ct)


