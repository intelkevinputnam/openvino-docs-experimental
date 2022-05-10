.. index:: pair: class; ov::op::v8::MaxPool
.. _doxid-classov_1_1op_1_1v8_1_1_max_pool:

class ov::op::v8::MaxPool
=========================



Overview
~~~~~~~~

MaxPooling operation with values and indices calculated as individual outputs. :ref:`More...<details-classov_1_1op_1_1v8_1_1_max_pool>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <max_pool.hpp>
	
	class MaxPool: public :ref:`ov::op::util::MaxPoolBase<doxid-classov_1_1op_1_1util_1_1_max_pool_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a98fcf3714b62b05d50a68140753245c4>`;

		// construction
	
		:ref:`MaxPool<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a0eb71b46eabd6f9deb7e66c7d1ada253>`();
	
		:ref:`MaxPool<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a2e3f14731f675545e866934e833ca393>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg,
			const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
			const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
			const :ref:`Shape<doxid-classov_1_1_shape>`& pads_begin,
			const :ref:`Shape<doxid-classov_1_1_shape>`& pads_end,
			const :ref:`Shape<doxid-classov_1_1_shape>`& kernel,
			const :ref:`op::RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>` rounding_type = :ref:`op::RoundingType::FLOOR<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6a56c1e354d36beb85b0d881c5b2e24cbe>`,
			const :ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>` auto_pad = op::PadType::EXPLICIT,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` index_element_type = :ref:`element::i64<doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>`,
			const int64_t axis = 0
			);

		// methods
	
		:target:`OPENVINO_OP<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a56edc64e45b919fe275fe2790bf1617c>`("MaxPool", "opset8", :ref:`op::util::MaxPoolBase<doxid-classov_1_1op_1_1util_1_1_max_pool_base>`);
		virtual bool :target:`visit_attributes<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a1d766bd360ae705fe47b2524932e6fbe>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1op_1_1v8_1_1_max_pool_1ae369afefadb70662bfb54451b36a6818>`();
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_with_new_inputs<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a7e8c78f9fdcc23efd6d7a2cb739eed84>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& new_args) const;
		const :ref:`Strides<doxid-classov_1_1_strides>`& :ref:`get_dilations<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a115c5cb91d423257e745299b65c74338>`() const;
		void :target:`set_dilations<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a00bcec025358d11fc5893a4a5aecde70>`(const :ref:`Strides<doxid-classov_1_1_strides>`& dilations);
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :ref:`get_index_element_type<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a5ba07a1edaebf48bd98fe955ff344fe1>`() const;
		void :target:`set_index_element_type<doxid-classov_1_1op_1_1v8_1_1_max_pool_1aacc8ab1f776beea35f577837e9a4bdf1>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` index_element_type);
		int64_t :target:`get_axis<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a681779fe759e6fefb17c31ea4e969da6>`() const;
		void :target:`set_axis<doxid-classov_1_1op_1_1v8_1_1_max_pool_1a90a140049353f3147e95157d28d1bb3b>`(const int64_t axis);
		virtual bool :ref:`has_evaluate<doxid-classov_1_1op_1_1v8_1_1_max_pool_1af47f95f94b7795d0d72562099f234792>`() const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` bool :ref:`evaluate<doxid-classov_1_1op_1_1v8_1_1_max_pool_1ad7f88f6450aa69086bb7b35bdb59d50d>`(
			const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values
			) const;
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
		:ref:`OPENVINO_OP<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a90879f88dd5988c5eb66aaf6c0dea80e>`("MaxPoolBase", "util");
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a9b4a8dc40b42f0309e57fda3c9f1071f>`();
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_kernel<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a822fe7d784b476d7cf3746c0c24248fb>`() const;
		void :ref:`set_kernel<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1aefe05f5df31acc94acc3651b6777f7e1>`(const :ref:`Shape<doxid-classov_1_1_shape>`& kernel);
		const :ref:`Strides<doxid-classov_1_1_strides>`& :ref:`get_strides<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a1a6fddda17552e80723abd3ef82d942a>`() const;
		void :ref:`set_strides<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a743846d2abdb826534e650e908520966>`(const :ref:`Strides<doxid-classov_1_1_strides>`& strides);
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_pads_begin<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a10abf7c8d00e83ae3e992340cf1f1a52>`() const;
		void :ref:`set_pads_begin<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1ad1409ae96e9a076742f9647320c21801>`(const :ref:`Shape<doxid-classov_1_1_shape>`& pads_begin);
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_pads_end<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1adcc88b81a3607756bb2fff7b23685641>`() const;
		void :ref:`set_adding_above<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1ae7651c19572454e34ff859c7db6fce63>`(const :ref:`Shape<doxid-classov_1_1_shape>`& pads_end);
		:ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>` :ref:`get_auto_pad<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a455ba184af424629cd3ea536c258da67>`() const;
		void :ref:`set_auto_pad<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a9cf56d6477945f45f03905f0598fcf1d>`(const :ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>` auto_pad);
		:ref:`op::RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>` :ref:`get_rounding_type<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1a2a6a87306dc24fc3523c9656109506b8>`() const;
		void :ref:`set_rounding_type<doxid-classov_1_1op_1_1util_1_1_max_pool_base_1aab9d9643bfd0b1a8b6b329627add4cbb>`(:ref:`op::RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>` rounding_type);

.. _details-classov_1_1op_1_1v8_1_1_max_pool:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

MaxPooling operation with values and indices calculated as individual outputs.

Construction
------------

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1a0eb71b46eabd6f9deb7e66c7d1ada253:
.. index:: pair: function; MaxPool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MaxPool()

Constructs an empty :ref:`MaxPool <doxid-classov_1_1op_1_1v8_1_1_max_pool>` operation.

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1a2e3f14731f675545e866934e833ca393:
.. index:: pair: function; MaxPool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MaxPool(
		const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& arg,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides,
		const :ref:`Strides<doxid-classov_1_1_strides>`& dilations,
		const :ref:`Shape<doxid-classov_1_1_shape>`& pads_begin,
		const :ref:`Shape<doxid-classov_1_1_shape>`& pads_end,
		const :ref:`Shape<doxid-classov_1_1_shape>`& kernel,
		const :ref:`op::RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>` rounding_type = :ref:`op::RoundingType::FLOOR<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6a56c1e354d36beb85b0d881c5b2e24cbe>`,
		const :ref:`PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>` auto_pad = op::PadType::EXPLICIT,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` index_element_type = :ref:`element::i64<doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>`,
		const int64_t axis = 0
		)

Constructs a parametrized :ref:`MaxPool <doxid-classov_1_1op_1_1v8_1_1_max_pool>` operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- arg

		- :ref:`Output <doxid-classov_1_1_output>` of a node producing the feature tensor to be pooled.

	*
		- strides

		- The strides of the pooling filter.

	*
		- dilations

		- The dilations of the pooling filter.

	*
		- pads_begin

		- Paddings at the beginning of each spatial axis.

	*
		- pads_end

		- Paddings at the end of each spatial axis.

	*
		- kernel

		- The kernel shape.

	*
		- rounding_type

		- Whether to use ceiling or floor rounding type while computing the output shape.

	*
		- auto_pad

		- The pad type for automatic calculation of the padding sizes.

	*
		- index_element_type

		- The data type used by the second output tensor containing the selected indices.

	*
		- axis

		- Indicates a dimension in the input data shape which should be used as a starting point for calculation of the upper bound of allowed values of the indices output.

Methods
-------

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1ae369afefadb70662bfb54451b36a6818:
.. index:: pair: function; validate_and_infer_types

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void validate_and_infer_types()

Verifies that attributes and inputs are consistent and computes output shapes and element types. Must be implemented by concrete child classes so that it can be run any number of times.

Throws if the node is invalid.

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1a115c5cb91d423257e745299b65c74338:
.. index:: pair: function; get_dilations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Strides<doxid-classov_1_1_strides>`& get_dilations() const



.. rubric:: Returns:

The pooling filter's dilations.

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1a5ba07a1edaebf48bd98fe955ff344fe1:
.. index:: pair: function; get_index_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`element::Type<doxid-classov_1_1element_1_1_type>` get_index_element_type() const



.. rubric:: Returns:

The data type of the second output tensor (indices).

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1af47f95f94b7795d0d72562099f234792:
.. index:: pair: function; has_evaluate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool has_evaluate() const

Allows to get information about availability of evaluate method for the current operation.

.. _doxid-classov_1_1op_1_1v8_1_1_max_pool_1ad7f88f6450aa69086bb7b35bdb59d50d:
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


