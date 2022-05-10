.. index:: pair: class; ov::op::v1::LogicalXor
.. _doxid-classov_1_1op_1_1v1_1_1_logical_xor:

class ov::op::v1::LogicalXor
============================



Overview
~~~~~~~~

Elementwise logical-xor operation. :ref:`More...<details-classov_1_1op_1_1v1_1_1_logical_xor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <logical_xor.hpp>
	
	class LogicalXor: public :ref:`ov::op::util::BinaryElementwiseLogical<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1a1336c4f7d257ef9f74089c8c27011fa1>`;

		// construction
	
		:target:`LogicalXor<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1abf382cf3a9d43b98ec8ba0ff694e43fb>`();
	
		:ref:`LogicalXor<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1ac4557b4875498ed15d34f380c1012cf1>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg0,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg1,
			const :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& auto_broadcast = :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`(:ref:`AutoBroadcastType::NUMPY<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219acead677ba7339dd3c0243cd3257b80be8f5>`)
			);

		// methods
	
		:target:`OPENVINO_OP<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1a1860e8a9d4a15f023aac94006514dc60>`("LogicalXor", "opset2", :ref:`util::BinaryElementwiseLogical<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical>`, 1);
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_with_new_inputs<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1adea17b197c8d9a9f1a2bf93ff653ee8f>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& new_args) const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` bool :ref:`evaluate<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1abb43658044e17d4a28fe81a85786af9f>`(
			const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values
			) const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool :ref:`has_evaluate<doxid-classov_1_1op_1_1v1_1_1_logical_xor_1a253bd706fb7e556b26c527d2024d98eb>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1_node_1af929e4dd70a66e0116a9d076753a2569>`;
		typedef std::map<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`RTMap<doxid-classov_1_1_node_1ab5856aecf96a9989fa1bafb97e4be2aa>`;

		// fields
	
		 :ref:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical_1a0e681a54fc91939fe1b30a2b46ba1c87>`;

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
		:ref:`OPENVINO_OP<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical_1a85f1a179f45d2c64828f58e45d33208f>`("BinaryElementwiseLogical", "util");
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical_1ad4f804b67b4e8a42a4b574d600d96b2f>`();
		virtual const :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& :ref:`get_autob<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical_1a12012d64e699c61afd0c2f6817f2c00c>`() const;
		void :ref:`set_autob<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical_1a52e8c3cf933d6c938d6788b639072dd8>`(const :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1op_1_1util_1_1_binary_elementwise_logical_1a564b95cc518b3404d6c765eb49477c6d>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);

.. _details-classov_1_1op_1_1v1_1_1_logical_xor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Elementwise logical-xor operation.

Construction
------------

.. _doxid-classov_1_1op_1_1v1_1_1_logical_xor_1ac4557b4875498ed15d34f380c1012cf1:
.. index:: pair: function; LogicalXor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LogicalXor(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg0,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg1,
		const :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& auto_broadcast = :ref:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`(:ref:`AutoBroadcastType::NUMPY<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219acead677ba7339dd3c0243cd3257b80be8f5>`)
		)

Constructs a logical-xor operation.

:ref:`Output <doxid-classov_1_1_output>` ``[d0, ...]``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- arg0

		- 
		  :ref:`Node <doxid-classov_1_1_node>` that produces the first input tensor.
		  
		  ``[d0, ...]``

	*
		- arg1

		- 
		  :ref:`Node <doxid-classov_1_1_node>` that produces the second input tensor.
		  
		  ``[d0, ...]``

	*
		- auto_broadcast

		- Auto broadcast specification

Methods
-------

.. _doxid-classov_1_1op_1_1v1_1_1_logical_xor_1abb43658044e17d4a28fe81a85786af9f:
.. index:: pair: function; evaluate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` bool evaluate(
		const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
		const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values
		) const

Evaluates the op on input_values putting results in output_values.

Deprecated Use evaluate with :ref:`ov::Tensor <doxid-classov_1_1_tensor>` instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_values

		- Tensors for the outputs to compute. One for each result

	*
		- input_values

		- Tensors for the inputs. One for each inputs.



.. rubric:: Returns:

true if successful

.. _doxid-classov_1_1op_1_1v1_1_1_logical_xor_1a253bd706fb7e556b26c527d2024d98eb:
.. index:: pair: function; has_evaluate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool has_evaluate() const

Allows to get information about availability of evaluate method for the current operation.


