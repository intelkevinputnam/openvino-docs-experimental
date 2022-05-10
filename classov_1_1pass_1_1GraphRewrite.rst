.. index:: pair: class; ov::pass::GraphRewrite
.. _doxid-classov_1_1pass_1_1_graph_rewrite:

class ov::pass::GraphRewrite
============================



Overview
~~~~~~~~

:ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` is a container for MatcherPasses that allows to run them on Function in efficient way. :ref:`More...<details-classov_1_1pass_1_1_graph_rewrite>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <graph_rewrite.hpp>
	
	class GraphRewrite: public :ref:`ov::pass::ModelPass<doxid-classov_1_1pass_1_1_model_pass>`
	{
	public:
		// construction
	
		:target:`GraphRewrite<doxid-classov_1_1pass_1_1_graph_rewrite_1a149751198a615c3ba5f2940b858e9771>`();
		:target:`GraphRewrite<doxid-classov_1_1pass_1_1_graph_rewrite_1a980d52131e8fa9518f521a1fd22dd3b1>`(const std::shared_ptr<:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`>& pass);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_graph_rewrite_1a90ee0a4c5a161722d738ab1971545167>`("ov::pass::GraphRewrite");
	
		template <
			typename T,
			bool Enabled = true,
			class... Args,
			typename std::enable_if<std::is_base_of<pass::MatcherPass, T>::value, bool>::type = true
			>
		std::shared_ptr<T> :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac>`(Args&&... args);
	
		template <
			typename T,
			class... Args,
			typename std::enable_if<std::is_base_of<pass::GraphRewrite, T>::value, bool>::type = true
			>
		void :ref:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1a826f4e2d1dfbf1a9905b97c5346010a6>`(Args&&... args);
	
		std::shared_ptr<:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`> :target:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1aa50614ed692bf256413fd8e7928871eb>`(const std::shared_ptr<:ref:`MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>`>& pass);
	
		void :target:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1af00561a5f69ca8657dde0dc550d67aa1>`(
			const std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`>& m,
			const :ref:`graph_rewrite_callback<doxid-namespaceov_1a5fe08faf69e9897c58d168a54359047e>`& callback,
			const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& property
			);
	
		void :target:`add_matcher<doxid-classov_1_1pass_1_1_graph_rewrite_1a1f1275df9bdc023c902114d3d2f1aa1c>`(
			const std::shared_ptr<:ref:`pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>`>& m,
			const :ref:`ov::graph_rewrite_callback<doxid-namespaceov_1a5fe08faf69e9897c58d168a54359047e>`& callback
			);
	
		virtual bool :target:`run_on_model<doxid-classov_1_1pass_1_1_graph_rewrite_1ad27ed8542330330ce9a524ff17564c21>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_graph_rewrite_1a97d000b54a0073754ca1dbc4516acbf2>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);
	};

	// direct descendants

	class :ref:`BidirectionalSequenceDecomposition<doxid-classngraph_1_1pass_1_1_bidirectional_sequence_decomposition>`;
	class :ref:`ConcatReduceFusion<doxid-classngraph_1_1pass_1_1_concat_reduce_fusion>`;
	class :ref:`ConvertConvolutions<doxid-classngraph_1_1pass_1_1_convert_convolutions>`;
	class :ref:`ConvertMatMulToFCorGemm<doxid-classngraph_1_1pass_1_1_convert_mat_mul_to_f_cor_gemm>`;
	class :ref:`ConvertMulOrAddFinally<doxid-classngraph_1_1pass_1_1_convert_mul_or_add_finally>`;
	class :ref:`ConvertNmsGatherPathToUnsigned<doxid-classngraph_1_1pass_1_1_convert_nms_gather_path_to_unsigned>`;
	class :ref:`ConvertReduceToPooling<doxid-classngraph_1_1pass_1_1_convert_reduce_to_pooling>`;
	class :ref:`ConvertSequenceToTensorIterator<doxid-classngraph_1_1pass_1_1_convert_sequence_to_tensor_iterator>`;
	class :ref:`ConvertTensorIteratorToSequence<doxid-classngraph_1_1pass_1_1_convert_tensor_iterator_to_sequence>`;
	class :ref:`ConvFusion<doxid-classngraph_1_1pass_1_1_conv_fusion>`;
	class :ref:`FuseFilteringBoxesBySize<doxid-classngraph_1_1pass_1_1_fuse_filtering_boxes_by_size>`;
	class :ref:`GeluFusion<doxid-classngraph_1_1pass_1_1_gelu_fusion>`;
	class :ref:`HSigmoidFusion<doxid-classngraph_1_1pass_1_1_h_sigmoid_fusion>`;
	class :ref:`HSwishFusion<doxid-classngraph_1_1pass_1_1_h_swish_fusion>`;
	class :ref:`InitMasks<doxid-classngraph_1_1pass_1_1_init_masks>`;
	class :ref:`LinOpSequenceFusion<doxid-classngraph_1_1pass_1_1_lin_op_sequence_fusion>`;
	class :ref:`TypeRelaxedReplacer<doxid-classngraph_1_1pass_1_1low__precision_1_1_type_relaxed_replacer>`;
	class :ref:`MVNFusion<doxid-classngraph_1_1pass_1_1_m_v_n_fusion>`;
	class :ref:`NopElimination<doxid-classngraph_1_1pass_1_1_nop_elimination>`;
	class :ref:`PadFusion<doxid-classngraph_1_1pass_1_1_pad_fusion>`;
	class :ref:`PReluFusion<doxid-classngraph_1_1pass_1_1_p_relu_fusion>`;
	class :ref:`PropagateMasks<doxid-classngraph_1_1pass_1_1_propagate_masks>`;
	class :ref:`Reshape1DOps<doxid-classngraph_1_1pass_1_1_reshape1_d_ops>`;
	class :ref:`SwishFusion<doxid-classngraph_1_1pass_1_1_swish_fusion>`;
	class :ref:`TransposeSinking<doxid-classngraph_1_1pass_1_1_transpose_sinking>`;
	class :ref:`BackwardGraphRewrite<doxid-classov_1_1pass_1_1_backward_graph_rewrite>`;
	class :ref:`CompressFloatConstants<doxid-classov_1_1pass_1_1_compress_float_constants>`;

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
		:ref:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_model_pass_1a718f43e809339887547f5c96b84ea00a>`("ov::pass::ModelPass");
		virtual bool :ref:`run_on_function<doxid-classov_1_1pass_1_1_model_pass_1a58cf259fa3f2d8b565e6929832656aa9>`(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> m);
		virtual bool :ref:`run_on_model<doxid-classov_1_1pass_1_1_model_pass_1afdce6ef577b36b5127115dd574b6615e>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);

.. _details-classov_1_1pass_1_1_graph_rewrite:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` is a container for MatcherPasses that allows to run them on Function in efficient way.

Graph rewrite pass is used for matcher passes execution on Function. To register :ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` use



.. rubric:: See also:

add_matcher<T>(args) method where T is a :ref:`MatcherPass <doxid-classov_1_1pass_1_1_matcher_pass>` class. As a default algorithm graph rewrite :ref:`pass <doxid-namespaceov_1_1pass>` traverse Function in topological order and applies registered matcher passes for each node. But if all registered matcher passes have type based root node in Matcher :ref:`pattern <doxid-namespaceov_1_1pass_1_1pattern>` then efficient mechanism is used to execute them. Matcher :ref:`pattern <doxid-namespaceov_1_1pass_1_1pattern>` root is type based if it' :ref:`s <doxid-ie__preprocess__gapi_8cpp_1afc7998e50661eed237070df8aab0f2d6>` operation from opset or :ref:`pattern::op::WrapType <doxid-classov_1_1pass_1_1pattern_1_1op_1_1_wrap_type>`. Note: when implementing :ref:`pattern <doxid-namespaceov_1_1pass_1_1pattern>` for Matcher make sure that root node is an operation from opset or has ov::pattern::op::WrapType. That will help :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` to execute matcher passes more efficient.

Methods
-------

.. _doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac:
.. index:: pair: function; add_matcher

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		bool Enabled = true,
		class... Args,
		typename std::enable_if<std::is_base_of<pass::MatcherPass, T>::value, bool>::type = true
		>
	std::shared_ptr<T> add_matcher(Args&&... args)

Register given transformation class type to :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` execution list All registered transformations will be executed in a single graph traversal. Example below show the basic usage of :ref:`pass::GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>`.

.. code-block:: cpp

	pass::Manager manager;
	auto anchor = manager.register_pass<GraphRewrite>();
	anchor->add_matcher<MatcherPassA>();
	anchor->add_matcher<MatcherPassB>();
	anchor->set_name("CommonMatchers");
	manager.run_passes(f);

For some purposes transformation can be registered and disabled by default.

.. code-block:: cpp

	anchor->add_matcher<MatcherPassB, false>();



.. rubric:: Returns:

shared_ptr to the transformation instance

.. _doxid-classov_1_1pass_1_1_graph_rewrite_1a826f4e2d1dfbf1a9905b97c5346010a6:
.. index:: pair: function; add_matcher

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		class... Args,
		typename std::enable_if<std::is_base_of<pass::GraphRewrite, T>::value, bool>::type = true
		>
	void add_matcher(Args&&... args)

Register passes from :ref:`GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` class that contains sequence of matcher passes registered in its ctor. For example:

class ov::pass::LinFusions: public :ref:`ov::pass::GraphRewrite <doxid-classov_1_1pass_1_1_graph_rewrite>` { public: OPENVINO_RTTI("LinFusion"); Fusions() {:ref:`add_matcher\<ov::pass::AddFusion>() <doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac>`; :ref:`add_matcher\<ov::pass::MulFusion>() <doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac>`; } };

:ref:`pass::Manager <doxid-classov_1_1pass_1_1_manager>` manager; auto anchor = manager.register_pass<GraphRewrite>(); anchor-> :ref:`add_matcher\<LinFusions>() <doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac>`; anchor-> :ref:`add_matcher\<OtherFusions>() <doxid-classov_1_1pass_1_1_graph_rewrite_1aa51d9ab71470eb93e0e8ce8f59c44eac>`; anchor->set_name("CommonFusions"); manager.run_passes(f);

In this case all matcher passes from LinFusions pass will be united with other registered matchers.

.. _doxid-classov_1_1pass_1_1_graph_rewrite_1a97d000b54a0073754ca1dbc4516acbf2:
.. index:: pair: function; set_pass_config

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_pass_config(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config)

Set :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` for particular transformation instance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pass_config

		- is a :ref:`PassConfig <doxid-classov_1_1pass_1_1_pass_config>` shared_ptr


