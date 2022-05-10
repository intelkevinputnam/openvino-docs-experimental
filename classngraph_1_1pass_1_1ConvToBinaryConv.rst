.. index:: pair: class; ngraph::pass::ConvToBinaryConv
.. _doxid-classngraph_1_1pass_1_1_conv_to_binary_conv:

class ngraph::pass::ConvToBinaryConv
====================================



Overview
~~~~~~~~

This transformation converts Convolution to BinaryConvolution under following conditions: :ref:`More...<details-classngraph_1_1pass_1_1_conv_to_binary_conv>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <conv_to_binary_conv.hpp>
	
	class ConvToBinaryConv: public :ref:`ov::pass::MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`
	{
	public:
		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1pass_1_1_conv_to_binary_conv_1acb6044f4e8f9208b01c9e7dd3d53449f>`("ConvToBinaryConv", "0");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`;

		// methods
	
		bool :ref:`get_property<doxid-classov_1_1pass_1_1_pass_base_1a3107964f6c4d4bf1d3fbc2bf97ccc0b8>`(const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& prop_mask) const;
		void :ref:`set_name<doxid-classov_1_1pass_1_1_pass_base_1a78ddde2a8770041d2f23ce59af908f5d>`(const std::string& name);
		std::string :ref:`get_name<doxid-classov_1_1pass_1_1_pass_base_1a6cd527d2176f1350dd999dc4632a576b>`() const;
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_base_1a6a56827a1cf76be99289bab703982869>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_pass_base_1abe74bba4b563ad367f2fdc7836016391>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);
		std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> :ref:`get_pass_config<doxid-classov_1_1pass_1_1_pass_base_1a4902f6ed9322e0fd38810d701f4409df>`();
		bool :ref:`m_transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1a568e5b1f0e01f221d36dffabbf156b3d>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		bool :ref:`transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		virtual const :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`& :ref:`get_type_info<doxid-classov_1_1pass_1_1_pass_base_1ab7020db2fcebc9b6e0741a451778fb0c>`() const = 0;
		:ref:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_matcher_pass_1a525c64de11717629f6599042761eb844>`("ov::pass::MatcherPass");
		:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`& :ref:`operator =<doxid-classov_1_1pass_1_1_matcher_pass_1ae003cfdc27f2418f603f12b4f031ba3c>` (const :ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`&);
		bool :ref:`apply<doxid-classov_1_1pass_1_1_matcher_pass_1afe5e71b978b3dc8274ea93bb6e7dcc23>`(std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> node);
	
		template <typename T, class... Args>
		std::shared_ptr<T> :ref:`register_new_node<doxid-classov_1_1pass_1_1_matcher_pass_1a6e14fcb5d87373bab47d5778ea39ba55>`(Args&&... args);
	
		template <typename T>
		std::shared_ptr<T> :ref:`register_new_node<doxid-classov_1_1pass_1_1_matcher_pass_1acb4756e168d3130377473123783c16fa>`(const std::shared_ptr<T>& node);
	
		std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`register_new_node_<doxid-classov_1_1pass_1_1_matcher_pass_1ae343beb91a81a3a6b43670726c7e7abe>`(const std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>& node);
		const std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>>& :ref:`get_new_nodes<doxid-classov_1_1pass_1_1_matcher_pass_1abf2e6b740f5e27a13589f19b47e934af>`();
		void :ref:`clear_new_nodes<doxid-classov_1_1pass_1_1_matcher_pass_1a9a3abba77cc94f47e1cdc4e064544d6a>`();
		std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`> :ref:`get_matcher<doxid-classov_1_1pass_1_1_matcher_pass_1a69329c064bb3cb7268ae397f374648e8>`();

.. _details-classngraph_1_1pass_1_1_conv_to_binary_conv:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This transformation converts Convolution to BinaryConvolution under following conditions:

* first input to Convolution is a FakeQuantize with levels==2 with output low,high being either (0, 1) or (-1, 1)

* second input (weights) is a constant with values -1 or 1 The transformation also converts weights to binary Constant (with 'u1' type) For example, when output_low is equal to 0 and output_high is equal to 1, following graph
  
  .. code-block:: cpp
  
  	.... ....  out_low   out_high
  	  |    |      |         |
  	 +--------------------------+           +-------------------------------------+
  	 | FakeQuantize (levels==2) |           |               Constant              |
  	 |     (on activations)     |           | (weights containing -1 or 1 values) |
  	 +--------------------------+           +-------------------------------------+
  	               |                                      |
  	               |                                      |
  	               -----------------    -------------------
  	                               |    |
  	                               v    v
  	                          +-------------+
  	                          | Convolution |
  	                          +-------------+
  	                                 |
  	                                 v
  
  is transformed to:
  
  .. code-block:: cpp
  
  	.... ....  out_low   out_high
  	  |    |      |         |
  	 +--------------------------+           +---------------------------------+
  	 | FakeQuantize (levels==2) |           |     Constant (with u1 type)     |
  	 |     (on activations)     |           | (with u1 type - binary weights) |
  	 +--------------------------+           +---------------------------------+
  	               |                                      |
  	               |                                      |
  	               -----------------    -------------------
  	                               |    |
  	                               v    v
  	                       +-------------------+
  	                       | BinaryConvolution |
  	                       +-------------------+
  	                                 |
  	                                 v
  	                          +------------+     +----------------------------------------------------+
  	                          |            |     |                   Constant                         |
  	                          |     Add    | <---|          (weights from original graph,             |
  	                          |            |     |  sum-reduced over [1,..., len(weights.shape)] axes |
  	                          +------------+     +----------------------------------------------------+
  	                                 |
  	                                 v
  	                          +------------+     +-----+
  	                          |  Multiply  | <---| 0.5 |
  	                          +------------+     +-----+
  	                                 |
  	                                 v


