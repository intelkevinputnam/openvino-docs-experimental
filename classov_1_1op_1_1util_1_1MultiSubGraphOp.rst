.. index:: pair: class; ov::op::util::MultiSubGraphOp
.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op:

class ov::op::util::MultiSubGraphOp
===================================

.. toctree::
	:hidden:

	BodyOutputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1BodyOutputDescription.rst>
	ConcatOutputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1ConcatOutputDescription.rst>
	InputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1InputDescription.rst>
	InvariantInputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1InvariantInputDescription.rst>
	MergedInputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1MergedInputDescription.rst>
	OutputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1OutputDescription.rst>
	SliceInputDescription <classov_1_1op_1_1util_1_1MultiSubGraphOp_1_1SliceInputDescription.rst>

Overview
~~~~~~~~

Abstract base class for sub-graph based ops, i.e ops that have some sub-graphs. :ref:`More...<details-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	class MultiSubGraphOp: public :ref:`ov::op::Op<doxid-classov_1_1op_1_1_op>`
	{
	public:
		// typedefs
	
		typedef std::vector<:ref:`MultiSubGraphOp::InputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description_1a750d0d553f8c4d59c87775f8ba335568>`> :target:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`;
		typedef std::vector<:ref:`MultiSubGraphOp::OutputDescription::Ptr<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description_1a53043b195b0af5f636fc35d5c8a501bc>`> :target:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`;

		// classes
	
		class :ref:`BodyOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_body_output_description>`;
		class :ref:`ConcatOutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_concat_output_description>`;
		class :ref:`InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`;
		class :ref:`InvariantInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_invariant_input_description>`;
		class :ref:`MergedInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_merged_input_description>`;
		class :ref:`OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`;
		class :ref:`SliceInputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_slice_input_description>`;

		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a25fc5f8a5409478c347dd7e09d3ca44b>`;

		// construction
	
		:target:`MultiSubGraphOp<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2d731c1b45bd91069a7b7702767b53e2>`(const MultiSubGraphOp&);
		:target:`MultiSubGraphOp<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1afe350f23e39a50427388e718a6e6a607>`(MultiSubGraphOp&&);

		// methods
	
		:target:`OPENVINO_OP<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1af50bd9dcd2cd1120811e3f0fc2e1e705>`("MultiSubGraphOp", "util");
		virtual const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& :ref:`get_function<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aa595b8721cc97756a936915304131430>`(int index) const;
		virtual void :ref:`set_function<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a1b6a38b68b1a44d0a27a9bd025dcc9e9>`(int index, const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& func);
		const :ref:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`& :ref:`get_input_descriptions<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1af134e5188ac3af0ffc16e3e1500bd4c5>`(int index) const;
		:ref:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`& :ref:`get_input_descriptions<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aa02ef5f4e62d8e8feb79d2df553b02e2>`(int index);
		const :ref:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`& :ref:`get_output_descriptions<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2f3af59f6d2b121e883c20db11469a31>`(int index) const;
		:ref:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`& :ref:`get_output_descriptions<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1ae7b32ec93a813d119536809a4ba64365>`(int index);
	
		void :ref:`set_input_descriptions<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a32b3e75ae66fd104ae7d926846b8b807>`(
			int index,
			const :ref:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`& inputs
			);
	
		void :ref:`set_output_descriptions<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1ae09c8bac7d7c9dd2391c64aef386a032>`(
			int index,
			const :ref:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`& outputs
			);
	
		virtual void :ref:`set_invariant_inputs<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2ff734dc98083d2e8003e2658aebc7da>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& bodies_parameters
			);
	
		virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`set_body_outputs<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aaac66fd7c89375c64e1fb86ce866e341>`(const :ref:`ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& bodies_results);
		virtual size_t :ref:`get_internal_subgraphs_size<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2c6d60a90adc7096a7d4d9f3b687cf7d>`() const;
		virtual size_t :ref:`get_input_descriptions_size<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aeaecc1e8af9b2a4fa09c1488dc2f6f49>`() const;
		virtual size_t :ref:`get_output_descriptions_size<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aefb4387c3f6992800cd769bc0166d1d3>`() const;
		MultiSubGraphOp& :target:`operator =<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1afbe03304f6bc5195824a98cb1dd75301>` (const MultiSubGraphOp&);
		MultiSubGraphOp& :target:`operator =<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a37aca5eaff75f68bd35c61f059516bad>` (MultiSubGraphOp&&);
	};

	// direct descendants

	class :ref:`SubGraphOp<doxid-classov_1_1op_1_1util_1_1_sub_graph_op>`;
	class :ref:`If<doxid-classov_1_1op_1_1v8_1_1_if>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`;
		typedef std::map<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`;

		// methods
	
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1_node_1ac5224b5be848ec670d2078d9816d12e7>`();
		void :ref:`constructor_validate_and_infer_types<doxid-classov_1_1_node_1aab98e14f28ac255819dfa4118174ece3>`();
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_node_1a9743b56d352970486d17dae2416d958e>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		virtual const :ref:`ov::op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& :ref:`get_autob<doxid-classov_1_1_node_1a2b4875877f138f9cc7ee51a207268b73>`() const;
		virtual bool :ref:`has_evaluate<doxid-classov_1_1_node_1a606a47a0c2d39dcc4032b985c04c209e>`() const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1acfb82acc8349d7138aeaa05217c7014e>`(
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values
			) const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1afe8b36f599d5f2f1f8b4ef0f1a56a65c>`(
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values,
			const :ref:`EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`& evaluationContext
			) const;
	
		virtual bool :ref:`evaluate_lower<doxid-classov_1_1_node_1a214ae74aa0de1eeaadeafb719e6ff260>`(const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values) const;
		virtual bool :ref:`evaluate_upper<doxid-classov_1_1_node_1ab509aeccf31f20473fa742df915f67e5>`(const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values) const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1a6096b644f59b1a7d1a1bf6bafe140472>`(
			:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values,
			const :ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& input_values
			) const;
	
		virtual bool :ref:`evaluate<doxid-classov_1_1_node_1af17129ce66b7273dfe9328ef21e61494>`(
			:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values,
			const :ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& input_values,
			const :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`& evaluationContext
			) const;
	
		virtual bool :ref:`evaluate_lower<doxid-classov_1_1_node_1aed425e8df8114daefbfe2b90b6ccde59>`(:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values) const;
		virtual bool :ref:`evaluate_upper<doxid-classov_1_1_node_1a191a82c8acc6016e2991a2dff3c626f8>`(:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_values) const;
		virtual bool :ref:`evaluate_label<doxid-classov_1_1_node_1a5ac5781812584d5bec31381fa513cb75>`(:ref:`TensorLabelVector<doxid-namespaceov_1aa5b856e58283417ceeace7343237b623>`& output_labels) const;
	
		virtual bool :ref:`constant_fold<doxid-classov_1_1_node_1a54e3bc84a49870563abf07e0fdd92de9>`(
			:ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& output_values,
			const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs_values
			);
	
		virtual :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :ref:`decompose_op<doxid-classov_1_1_node_1add7ebde1542aef560a5d5135e8fe7b67>`() const;
		virtual const :ref:`type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& :ref:`get_type_info<doxid-classov_1_1_node_1a09d7370d5fa57c28880598760fd9c893>`() const = 0;
		const char \* :ref:`get_type_name<doxid-classov_1_1_node_1a312ad4b62537167e5e5c784df8b03ff3>`() const;
		void :ref:`set_arguments<doxid-classov_1_1_node_1a939c896986f4c0cfc9e47895d698b051>`(const :ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& arguments);
		void :ref:`set_arguments<doxid-classov_1_1_node_1a9476f10de4bf8eaffbc3bc54abbd67bc>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& arguments);
		void :ref:`set_argument<doxid-classov_1_1_node_1ab90cfad02a35d49500c1773dca71d09a>`(size_t position, const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& argument);
	
		void :ref:`set_output_type<doxid-classov_1_1_node_1affde9025d41a4b200d726bee750b20e4>`(
			size_t i,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& pshape
			);
	
		void :ref:`set_output_size<doxid-classov_1_1_node_1a27a4363bf01e836006ef0ff0ad1fb7e0>`(size_t output_size);
		void :ref:`invalidate_values<doxid-classov_1_1_node_1af4f961268c306511c2c28ee66bc81639>`();
		virtual void :ref:`revalidate_and_infer_types<doxid-classov_1_1_node_1a474ccc02e97cb12224a339b843e30615>`();
		virtual std::string :ref:`description<doxid-classov_1_1_node_1abb0f7c0a63ff520f7955378ec52b98d3>`() const;
		const std::string& :ref:`get_name<doxid-classov_1_1_node_1a82d9842d00beff82932b5baac3e723a3>`() const;
		void :ref:`set_friendly_name<doxid-classov_1_1_node_1a7980b10e7fa641adb972bbfc27e94dc4>`(const std::string& name);
		const std::string& :ref:`get_friendly_name<doxid-classov_1_1_node_1a613bbf08ebce8c05c63dacabbc341080>`() const;
		virtual bool :ref:`is_dynamic<doxid-classov_1_1_node_1a55033c8479e6c6e51a6d2cf47cc0575b>`() const;
		size_t :ref:`get_instance_id<doxid-classov_1_1_node_1a97150e2017a476ce1b75580e084244d8>`() const;
		virtual std::ostream& :ref:`write_description<doxid-classov_1_1_node_1a7fcbf2c087273dfb0b7fc153c677dbbb>`(std::ostream& os, uint32_t depth = 0) const;
		const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& :ref:`get_control_dependencies<doxid-classov_1_1_node_1af66774ea3f8ec0699612ee69980de776>`() const;
		const std::vector<:ref:`Node<doxid-classov_1_1_node>` \*>& :ref:`get_control_dependents<doxid-classov_1_1_node_1a464cd8dfcf5f771974ce06bb7e6ec62f>`() const;
		void :ref:`add_control_dependency<doxid-classov_1_1_node_1a47d1a4fb855f1156614846a477f69adb>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		void :ref:`remove_control_dependency<doxid-classov_1_1_node_1a1037a77a8f0220d586b790906b6af488>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		void :ref:`clear_control_dependencies<doxid-classov_1_1_node_1a97cf3538584ac88d8121c38c45fd3820>`();
		void :ref:`clear_control_dependents<doxid-classov_1_1_node_1a08a2dd9069a63d69b6d1ebc7ac3d4921>`();
		void :ref:`add_node_control_dependencies<doxid-classov_1_1_node_1a5aeb2ec8bde867868c391a01dafc1870>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> source_node);
		void :ref:`add_node_control_dependents<doxid-classov_1_1_node_1a54474d9cdeb16624f1fd488c88ecf2ca>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> source_node);
		void :ref:`transfer_control_dependents<doxid-classov_1_1_node_1af0593c95b56ff9723fa748325868db22>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> replacement);
		size_t :ref:`get_output_size<doxid-classov_1_1_node_1ac8706eab0c33f0effa522a6bbed8437e>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_output_element_type<doxid-classov_1_1_node_1af54b4c4728f6fe535e00979c04181926>`(size_t i) const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1_node_1a5f04dfdfeafb4f47afa279f1fab8041f>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_output_shape<doxid-classov_1_1_node_1a9be808628e89171b222165ae2f4b71d5>`(size_t i) const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_output_partial_shape<doxid-classov_1_1_node_1a5002b656c4e79d19e3914f3d28195833>`(size_t i) const;
		:ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`get_default_output<doxid-classov_1_1_node_1aee8da8b622e352e9e21270b7f381e2b1>`() const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_default_output<doxid-classov_1_1_node_1a0a49fd568aea74a68baa2161e4f7df85>`();
		virtual size_t :ref:`get_default_output_index<doxid-classov_1_1_node_1a0d31de32156b3afd0c6db698d888575a>`() const;
		size_t :ref:`no_default_index<doxid-classov_1_1_node_1ad0035c4860b08e05b3e100966a570118>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1_node_1a0e635bd6c9dab32258beb74813a86fa2>`() const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_output_tensor<doxid-classov_1_1_node_1acdba65c4711078f39814267e953f9b26>`(size_t i) const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_input_tensor<doxid-classov_1_1_node_1a1f11abc6a67540cf165cff35c569474e>`(size_t i) const;
		const std::string& :ref:`get_output_tensor_name<doxid-classov_1_1_node_1a4917773db5557c76721e61dd086e2fed>`(size_t i) const;
		std::set<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`get_output_target_inputs<doxid-classov_1_1_node_1af4458f6b74c68754dd5e38b0562aed4c>`(size_t i) const;
		size_t :ref:`get_input_size<doxid-classov_1_1_node_1a19356bfdc8759abdb34f4269bbc6f821>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_input_element_type<doxid-classov_1_1_node_1a376e413971f30898cc2f9552cb80b525>`(size_t i) const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_input_shape<doxid-classov_1_1_node_1a34bd30fb200ea5432351e7495eca3aba>`(size_t i) const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_input_partial_shape<doxid-classov_1_1_node_1a1e506b8cb3d40b6cb096d26627a3227b>`(size_t i) const;
		const std::string& :ref:`get_input_tensor_name<doxid-classov_1_1_node_1a45607918c100cd66492aeb897927fd4c>`(size_t i) const;
		:ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_input_node_ptr<doxid-classov_1_1_node_1a8358ec5a06b653eb8f5a4c7895cb0bec>`(size_t index) const;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input_node_shared_ptr<doxid-classov_1_1_node_1a794272a6a64575a43b55f3854cf5da52>`(size_t index) const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input_source_output<doxid-classov_1_1_node_1aae6163287ddf09da421da058e2375ee2>`(size_t i) const;
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`clone_with_new_inputs<doxid-classov_1_1_node_1a177d1a61e81d506d190ee18818ff851f>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs) const = 0;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`copy_with_new_inputs<doxid-classov_1_1_node_1a71b79a703b6cb65796b3eab14d7f669b>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& new_args) const;
	
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`copy_with_new_inputs<doxid-classov_1_1_node_1aea49595d14777748fe215ce1b0b4f976>`(
			const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs,
			const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& control_dependencies
			) const;
	
		bool :ref:`has_same_type<doxid-classov_1_1_node_1aa0d6ac1b94265535fd6604f504f24bc0>`(std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`> node) const;
		:ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`& :ref:`get_rt_info<doxid-classov_1_1_node_1a5c73794fbc47e510198261d61682fe79>`();
		const :ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`& :ref:`get_rt_info<doxid-classov_1_1_node_1a6b70cf8118b8eb0f499e75e8c59e3dda>`() const;
		:ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>` :ref:`get_users<doxid-classov_1_1_node_1ac91febe368510da62e45d591255a4c6e>`(bool check_is_used = false) const;
		virtual size_t :ref:`get_version<doxid-classov_1_1_node_1a09b3d13897b7cadcc7a9967f7a5a41f9>`() const;
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_default_value<doxid-classov_1_1_node_1a829ba04609ff698e5297f86a79eef103>`() const;
		bool :ref:`operator <<doxid-classov_1_1_node_1a041846b4bc1cf064f6bc3f6770a947cf>` (const :ref:`Node<doxid-classov_1_1_node>`& other) const;
		std::vector<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`inputs<doxid-classov_1_1_node_1aae7545fcb3386ab6dbdebdbda409d747>`();
		std::vector<:ref:`Input<doxid-classov_1_1_input>`<const :ref:`Node<doxid-classov_1_1_node>`>> :ref:`inputs<doxid-classov_1_1_node_1a02b7bc6696e0b8aa0bcb2d04d99bc2f1>`() const;
		std::vector<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`input_values<doxid-classov_1_1_node_1a5861ceeb81e573a7eaaf3d036fe5c23a>`() const;
		std::vector<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`outputs<doxid-classov_1_1_node_1aa6d74a054cf5302244978c9c6f9e338d>`();
		std::vector<:ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`>> :ref:`outputs<doxid-classov_1_1_node_1a0d79f0cbc914a3b411869e56a6cb1f94>`() const;
		:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_node_1a2e956e69b0de757004efe88f31f83720>`(size_t input_index);
		:ref:`Input<doxid-classov_1_1_input>`<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`input<doxid-classov_1_1_node_1a414bd1a9899c4f1f96286fb2b0ac585b>`(size_t input_index) const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`input_value<doxid-classov_1_1_node_1a0309b251e1dc8722d0cf144199cb1de9>`(size_t input_index) const;
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_node_1a24dc2a2bac789d34d8e1959249b6347d>`(size_t output_index);
		:ref:`Output<doxid-classov_1_1_output>`<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`output<doxid-classov_1_1_node_1afbd386f7c799f4f05393336232b43144>`(size_t output_index) const;
		:ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` void :ref:`set_op_annotations<doxid-classov_1_1_node_1a9d8680c016917426085ce1e18977428f>`(std::shared_ptr<ngraph::op::util::OpAnnotations> op_annotations);
		std::shared_ptr<ngraph::op::util::OpAnnotations> :ref:`get_op_annotations<doxid-classov_1_1_node_1ab396069426f5eabed56e2c8fc3c840d0>`() const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool :ref:`match_value<doxid-classov_1_1_node_1a91d357857f994496c0bfb62f840fa273>`(
			:ref:`ov::pass::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>` \* matcher,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& pattern_value,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value
			);
	
		virtual bool :ref:`match_node<doxid-classov_1_1_node_1abdd7772bf5673526b64ddd6d310bb2f9>`(
			:ref:`ov::pass::pattern::Matcher<doxid-classov_1_1pass_1_1pattern_1_1_matcher>` \* matcher,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& graph_value
			);
	
		static _OPENVINO_HIDDEN_METHODconst :::ref:`ov::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& :ref:`get_type_info_static<doxid-classov_1_1op_1_1_op_1a236ae4310a12e8b9ee7115af2154c489>`();
		virtual const :::ref:`ov::Node::type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`& :ref:`get_type_info<doxid-classov_1_1op_1_1_op_1ae930efe3e70276acfd9d349aa58dabb7>`() const;

.. _details-classov_1_1op_1_1util_1_1_multi_sub_graph_op:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Abstract base class for sub-graph based ops, i.e ops that have some sub-graphs.

Methods
-------

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aa595b8721cc97756a936915304131430:
.. index:: pair: function; get_function

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& get_function(int index) const

Gets internal sub-graph by index in :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- sub-graph's index in op



.. rubric:: Returns:

pointer to :ref:`Model <doxid-classov_1_1_model>` with sub-graph

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a1b6a38b68b1a44d0a27a9bd025dcc9e9:
.. index:: pair: function; set_function

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_function(int index, const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& func)

Adds sub-graph to :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of new sub-graph

	*
		- func

		- func new sub_graph as :ref:`Model <doxid-classov_1_1_model>`

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1af134e5188ac3af0ffc16e3e1500bd4c5:
.. index:: pair: function; get_input_descriptions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`& get_input_descriptions(int index) const

Gets vector with connections beewtwen operation inputs and internal sub-graph parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of internal sub-graph



.. rubric:: Returns:

vector of input descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aa02ef5f4e62d8e8feb79d2df553b02e2:
.. index:: pair: function; get_input_descriptions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`& get_input_descriptions(int index)

Gets vector with connections beewtwen operation inputs and internal sub-graph parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of internal sub-graph



.. rubric:: Returns:

vector of input descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2f3af59f6d2b121e883c20db11469a31:
.. index:: pair: function; get_output_descriptions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`& get_output_descriptions(int index) const

Gets vector with connections beewtwen operation outputs and internal sub-graph results.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of internal sub-graph



.. rubric:: Returns:

vector of output descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1ae7b32ec93a813d119536809a4ba64365:
.. index:: pair: function; get_output_descriptions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`& get_output_descriptions(int index)

Gets vector with connections beewtwen operation outputs and internal sub-graph results.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of internal sub-graph



.. rubric:: Returns:

vector of output descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a32b3e75ae66fd104ae7d926846b8b807:
.. index:: pair: function; set_input_descriptions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_input_descriptions(
		int index,
		const :ref:`MultiSubgraphInputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a5028ab6cafca3b1d4e3261985ad5fba7>`& inputs
		)

Sets vector with connections beewtwen operation inputs and internal sub-graph parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of internal sub-graph

	*
		- inputs

		- vector of input descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1ae09c8bac7d7c9dd2391c64aef386a032:
.. index:: pair: function; set_output_descriptions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_output_descriptions(
		int index,
		const :ref:`MultiSubgraphOutputDescriptionVector<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a0e6ef5f5e92c95ba9e7f760ef94493cc>`& outputs
		)

Sets vector with connections beewtwen operation outputs and internal sub-graph results.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- index of internal sub-graph

	*
		- outputs

		- vector of input descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2ff734dc98083d2e8003e2658aebc7da:
.. index:: pair: function; set_invariant_inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_invariant_inputs(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value,
		const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& bodies_parameters
		)

Set input decriptions for :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` input.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The value supplied as an input to the block.

	*
		- bodies_parameters

		- vector of bodies parameters.

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aaac66fd7c89375c64e1fb86ce866e341:
.. index:: pair: function; set_body_outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> set_body_outputs(const :ref:`ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& bodies_results)

Set output decriptions for :ref:`MultiSubGraphOp <doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op>` output.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bodies_results

		- vector of bodies results for one output.



.. rubric:: Returns:

value :ref:`Output <doxid-classov_1_1_output>` node for bodies_results.

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1a2c6d60a90adc7096a7d4d9f3b687cf7d:
.. index:: pair: function; get_internal_subgraphs_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_internal_subgraphs_size() const

Get number of internal sub-graphs.



.. rubric:: Returns:

Number of sub-graphs.

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aeaecc1e8af9b2a4fa09c1488dc2f6f49:
.. index:: pair: function; get_input_descriptions_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_input_descriptions_size() const

Get number of input descriptions.



.. rubric:: Returns:

Number of input descriptions

.. _doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1aefb4387c3f6992800cd769bc0166d1d3:
.. index:: pair: function; get_output_descriptions_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_output_descriptions_size() const

Get number of output descriptions.



.. rubric:: Returns:

Number of output descriptions


