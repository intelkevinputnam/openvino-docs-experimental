.. index:: pair: class; ov::op::v6::CTCGreedyDecoderSeqLen
.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len:

class ov::op::v6::CTCGreedyDecoderSeqLen
========================================



Overview
~~~~~~~~

Operator performing CTCGreedyDecoder. :ref:`More...<details-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ctc_greedy_decoder_seq_len.hpp>
	
	class CTCGreedyDecoderSeqLen: public :ref:`ov::op::Op<doxid-classov_1_1op_1_1_op>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1aa1c92c561b78783e869ec6f5c3473aa4>`;

		// construction
	
		:target:`CTCGreedyDecoderSeqLen<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1adf030aa6abb9cf131137ef14b9ba4fc3>`();
	
		:ref:`CTCGreedyDecoderSeqLen<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a875812b42e5ee6f4d6e228cd60509f2f>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& seq_len,
			const bool merge_repeated = true,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& classes_index_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& sequence_length_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`
			);
	
		:ref:`CTCGreedyDecoderSeqLen<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a2ec6699a1af7fb51919174665b743bb4>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& seq_len,
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& blank_index,
			const bool merge_repeated = true,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& classes_index_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& sequence_length_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`
			);

		// methods
	
		:target:`OPENVINO_OP<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a8f785539bbe3ea05ae4c64ca67a788d3>`("CTCGreedyDecoderSeqLen", "opset6", :ref:`op::Op<doxid-classov_1_1op_1_1_op>`, 6);
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a65ce5da4e59e8b3e55da3a050e5f43a1>`();
		virtual bool :target:`visit_attributes<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1aaf13005542acb896de515239e57033d8>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_with_new_inputs<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1afc6f3f8bfb5634a7369d67f634b09124>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& new_args) const;
		bool :ref:`get_merge_repeated<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1ae90b879b56405cccc010aa8f54e759dc>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_classes_index_type<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a28ae84485d9d9019b3721d5acd8e72ac>`() const;
		void :ref:`set_classes_index_type<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a8273554153e5804a0bf8486a243b1169>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& classes_index_type);
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_sequence_length_type<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1acea73c6f802c6c2cebad60c1d9f1c429>`() const;
		void :ref:`set_sequence_length_type<doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a1fe0573d14c1e8a3f77d80e492fdf4ad>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& sequence_length_type);
	};

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

.. _details-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Operator performing CTCGreedyDecoder.

Construction
------------

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a875812b42e5ee6f4d6e228cd60509f2f:
.. index:: pair: function; CTCGreedyDecoderSeqLen

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CTCGreedyDecoderSeqLen(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& seq_len,
		const bool merge_repeated = true,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& classes_index_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& sequence_length_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`
		)

Constructs a :ref:`CTCGreedyDecoderSeqLen <doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len>` operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input

		- 3-D tensor of logits on which greedy decoding is performed

	*
		- seq_len

		- 1-D tensor of sequence lengths

	*
		- merge_repeated

		- Whether to merge repeated labels

	*
		- classes_index_type

		- Specifies the output classes_index tensor type

	*
		- sequence_length_type

		- Specifies the output sequence_length tensor type

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a2ec6699a1af7fb51919174665b743bb4:
.. index:: pair: function; CTCGreedyDecoderSeqLen

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CTCGreedyDecoderSeqLen(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& input,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& seq_len,
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& blank_index,
		const bool merge_repeated = true,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& classes_index_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& sequence_length_type = :ref:`element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`
		)

Constructs a :ref:`CTCGreedyDecoderSeqLen <doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len>` operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input

		- 3-D tensor of logits on which greedy decoding is performed

	*
		- seq_len

		- 1-D tensor of sequence lengths

	*
		- blank_index

		- Scalar or 1-D tensor with 1 element used to mark a blank index

	*
		- merge_repeated

		- Whether to merge repeated labels

	*
		- classes_index_type

		- Specifies the output classes_index tensor type

	*
		- sequence_length_type

		- Specifies the output sequence_length tensor type

Methods
-------

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a65ce5da4e59e8b3e55da3a050e5f43a1:
.. index:: pair: function; validate_and_infer_types

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void validate_and_infer_types()

Verifies that attributes and inputs are consistent and computes output shapes and element types. Must be implemented by concrete child classes so that it can be run any number of times.

Throws if the node is invalid.

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1ae90b879b56405cccc010aa8f54e759dc:
.. index:: pair: function; get_merge_repeated

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_merge_repeated() const

Get merge_repeated attribute.



.. rubric:: Returns:

Current value of merge_repeated attribute

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a28ae84485d9d9019b3721d5acd8e72ac:
.. index:: pair: function; get_classes_index_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_classes_index_type() const

Get classes_index_type attribute.



.. rubric:: Returns:

Current value of classes_index_type attribute

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a8273554153e5804a0bf8486a243b1169:
.. index:: pair: function; set_classes_index_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_classes_index_type(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& classes_index_type)

Set classes_index_type attribute.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- classes_index_type

		- Type of classes_index

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1acea73c6f802c6c2cebad60c1d9f1c429:
.. index:: pair: function; get_sequence_length_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_sequence_length_type() const

Get sequence_length_type attribute.



.. rubric:: Returns:

Current value of sequence_length_type attribute

.. _doxid-classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len_1a1fe0573d14c1e8a3f77d80e492fdf4ad:
.. index:: pair: function; set_sequence_length_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_sequence_length_type(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& sequence_length_type)

Set sequence_length_type attribute.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- sequence_length_type

		- Type of sequence length


