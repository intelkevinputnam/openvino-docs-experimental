.. index:: pair: class; ov::op::v0::Constant
.. _doxid-classov_1_1op_1_1v0_1_1_constant:

class ov::op::v0::Constant
==========================



Overview
~~~~~~~~

Class for constants. :ref:`More...<details-classov_1_1op_1_1v0_1_1_constant>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <constant.hpp>
	
	class Constant: public :ref:`ov::op::Op<doxid-classov_1_1op_1_1_op>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1op_1_1v0_1_1_constant_1a9c14cdd2b72875812e1cecdac8164250>`;

		// construction
	
		:target:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a5c88dbfc494539a5d20c60877d29adc6>`();
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a0393a8c803c2a1d3776a8ca680762678>`(const std::shared_ptr<:ref:`ngraph::runtime::Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`>& tensor);
	
		template <typename T>
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a7af762c62d55701338b0f07c3d18808a>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const std::vector<T>& values
			);
	
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a78a214385cfba4bf6d42f65375f35c9a>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
	
		template <class T, class = typename std::enable_if<std::is_fundamental<T>::value>::type>
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a1288b3903e9adaf504cd0875630c3d1d>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			T value
			);
	
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a5e78fa47231a20338cc74a257c24c3c1>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const std::vector<std::string>& values
			);
	
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a382a08450ee95849374f9665bf6bfe07>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape, const void \* data);
	
		template <typename T>
		:ref:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a3614fa4e39f41a2fa01ef8a3bb13334b>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			std::shared_ptr<:ref:`ngraph::runtime::SharedBuffer<doxid-classngraph_1_1runtime_1_1_shared_buffer>`<T>> data
			);
	
		:target:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1a4d308f5a6ff3bd53064085d3b6ecc179>`(const Constant& other);
		:target:`Constant<doxid-classov_1_1op_1_1v0_1_1_constant_1ac9ff59b01813af340cdfc2d69c837e21>`(const Constant& other, const :ref:`Shape<doxid-classov_1_1_shape>`& new_shape);

		// methods
	
		:target:`OPENVINO_OP<doxid-classov_1_1op_1_1v0_1_1_constant_1a859f2b8379adde92ee3f176562727f47>`("Constant", "opset1");
	
		template <typename T>
		void :target:`fill_data<doxid-classov_1_1op_1_1v0_1_1_constant_1a8c240ba07ca1fd58eb69987e3b84b4ad>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type, T value);
	
		Constant& :target:`operator =<doxid-classov_1_1op_1_1v0_1_1_constant_1aeab3dd9bdeba09495ba075bd569508f7>` (const Constant&);
		virtual void :ref:`validate_and_infer_types<doxid-classov_1_1op_1_1v0_1_1_constant_1a55dd482843c7b4717624dae96d6c1956>`();
		virtual bool :target:`visit_attributes<doxid-classov_1_1op_1_1v0_1_1_constant_1ac0b40a12bbc39c64dae2fdcf3b9de261>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` bool :ref:`evaluate<doxid-classov_1_1op_1_1v0_1_1_constant_1a6f62fc2408d8e663ce258ee6d998e087>`(
			const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_values,
			const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_values
			) const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool :ref:`has_evaluate<doxid-classov_1_1op_1_1v0_1_1_constant_1ab69e6632b3573b2a1fd7022736594105>`() const;
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` bool :target:`evaluate_lower<doxid-classov_1_1op_1_1v0_1_1_constant_1af7183cea7907c5333db9f13869364d71>`(const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& outputs) const;
		virtual bool :target:`evaluate_upper<doxid-classov_1_1op_1_1v0_1_1_constant_1afe7adf6d5412402edb75aca4df4023e2>`(const :ref:`HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& outputs) const;
	
		virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool :target:`constant_fold<doxid-classov_1_1op_1_1v0_1_1_constant_1a67547e6a872d6b0aaa04d679cbe36046>`(
			:ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& outputs,
			const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs
			);
	
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`get_shape_val<doxid-classov_1_1op_1_1v0_1_1_constant_1ad5c359a0f3bde246ec7462dc6b4fe111>`() const;
		:ref:`Strides<doxid-classov_1_1_strides>` :ref:`get_strides_val<doxid-classov_1_1op_1_1v0_1_1_constant_1a0aed3d127309d7c9065d3f653ceead34>`() const;
		:ref:`Coordinate<doxid-classov_1_1_coordinate>` :ref:`get_coordinate_val<doxid-classov_1_1op_1_1v0_1_1_constant_1ac5feb281a38b4569a056e8bb3453cb12>`() const;
		:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>` :ref:`get_coordinate_diff_val<doxid-classov_1_1op_1_1v0_1_1_constant_1af774b06fe106c32c9f0da920c8a269cc>`() const;
		:ref:`AxisVector<doxid-classov_1_1_axis_vector>` :ref:`get_axis_vector_val<doxid-classov_1_1op_1_1v0_1_1_constant_1a21387d37bbb14791fba765e86cdbd1c0>`() const;
		:ref:`AxisSet<doxid-classov_1_1_axis_set>` :ref:`get_axis_set_val<doxid-classov_1_1op_1_1v0_1_1_constant_1a9bb2cff30b5c25ae35ed54e0bdb7b247>`() const;
		void :ref:`set_data_shape<doxid-classov_1_1op_1_1v0_1_1_constant_1a8800b88fd610af80749ba715654f157a>`(const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
		size_t :ref:`get_byte_size<doxid-classov_1_1op_1_1v0_1_1_constant_1a6a80bd52b75e981e087cb300faa86d24>`() const;
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_with_new_inputs<doxid-classov_1_1op_1_1v0_1_1_constant_1a5459a42c8b48c705f7f101de4b253b4e>`(const :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& new_args) const;
		std::vector<std::string> :ref:`get_value_strings<doxid-classov_1_1op_1_1v0_1_1_constant_1a3fc03d7d8f853464671833b83b61e9d6>`() const;
	
		template <typename T>
		std::vector<T> :target:`get_vector<doxid-classov_1_1op_1_1v0_1_1_constant_1ad7df5f4de69d05d168e12b0df79d3ed9>`() const;
	
		template <typename T>
		std::vector<T> :ref:`cast_vector<doxid-classov_1_1op_1_1v0_1_1_constant_1abd4d166d19ef4f7204abb53ec5247ce3>`() const;
	
		const void \* :target:`get_data_ptr<doxid-classov_1_1op_1_1v0_1_1_constant_1a79fa84a4d8fb977708e1f64aaf94d2de>`() const;
	
		template <typename T>
		const T \* :target:`get_data_ptr<doxid-classov_1_1op_1_1v0_1_1_constant_1ac6c73d901e4ae8368c6ef18bb373bf20>`() const;
	
		template <element::Type_t ET>
		const :ref:`element_type_traits<doxid-structov_1_1element__type__traits>`<ET>::value_type \* :target:`get_data_ptr<doxid-classov_1_1op_1_1v0_1_1_constant_1aa69b554075f081322f9c89019ff8fbf4>`() const;
	
		bool :target:`get_all_data_elements_bitwise_identical<doxid-classov_1_1op_1_1v0_1_1_constant_1a53e90c24ef5334a632b634773528d04b>`() const;
		std::string :target:`convert_value_to_string<doxid-classov_1_1op_1_1v0_1_1_constant_1af4c13a4e2115b2031384c8bcc1f73ea9>`(size_t index) const;
	
		template <typename T>
		static std::shared_ptr<Constant> :ref:`create<doxid-classov_1_1op_1_1v0_1_1_constant_1aded3f3d661b74d480aa1e20c81a66c09>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const std::vector<T>& values
			);
	
		template <typename T>
		static std::shared_ptr<Constant> :ref:`create<doxid-classov_1_1op_1_1v0_1_1_constant_1ab834a9774972682a5b9d718c6bb21899>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			std::initializer_list<T> values
			);
	
		static std::shared_ptr<Constant> :ref:`create<doxid-classov_1_1op_1_1v0_1_1_constant_1a4b02934a0557311027edfd7c81821669>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const void \* memory
			);
	};

	// direct descendants

	template :ref:`Scalar<doxid-classngraph_1_1snippets_1_1op_1_1_scalar>`;

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

.. _details-classov_1_1op_1_1v0_1_1_constant:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class for constants.

Construction
------------

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a0393a8c803c2a1d3776a8ca680762678:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Constant(const std::shared_ptr<:ref:`ngraph::runtime::Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`>& tensor)

Initialize a constant from tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- The tensor with data

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a7af762c62d55701338b0f07c3d18808a:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	Constant(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const std::vector<T>& values
		)

Constructs a tensor constant.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- values

		- A vector of literals for initializing the tensor constant. The size of values must match the size of the shape.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a78a214385cfba4bf6d42f65375f35c9a:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Constant(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

Create uninitialized constant.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a1288b3903e9adaf504cd0875630c3d1d:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T, class = typename std::enable_if<std::is_fundamental<T>::value>::type>
	Constant(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		T value
		)

Constructs a uniform tensor constant.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- value

		- A scalar for initializing the uniform tensor constant. The value is broadcast to the specified shape.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a5e78fa47231a20338cc74a257c24c3c1:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Constant(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const std::vector<std::string>& values
		)

Constructs a tensor constant This constructor is mainly to support deserialization of constants.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- values

		- A list of string values to use as the constant data.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a382a08450ee95849374f9665bf6bfe07:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Constant(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape, const void \* data)

Constructs a tensor constant with the supplied data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- data

		- A void\* to constant data.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a3614fa4e39f41a2fa01ef8a3bb13334b:
.. index:: pair: function; Constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	Constant(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		std::shared_ptr<:ref:`ngraph::runtime::SharedBuffer<doxid-classngraph_1_1runtime_1_1_shared_buffer>`<T>> data
		)

Constructs a tensor constant with the supplied data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- data

		- A pointer to pre-allocated shared data.

Methods
-------

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a55dd482843c7b4717624dae96d6c1956:
.. index:: pair: function; validate_and_infer_types

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void validate_and_infer_types()

Verifies that attributes and inputs are consistent and computes output shapes and element types. Must be implemented by concrete child classes so that it can be run any number of times.

Throws if the node is invalid.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a6f62fc2408d8e663ce258ee6d998e087:
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

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1ab69e6632b3573b2a1fd7022736594105:
.. index:: pair: function; has_evaluate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool has_evaluate() const

Allows to get information about availability of evaluate method for the current operation.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1ad5c359a0f3bde246ec7462dc6b4fe111:
.. index:: pair: function; get_shape_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Shape<doxid-classov_1_1_shape>` get_shape_val() const

Returns the value of the constant node as a :ref:`Shape <doxid-classov_1_1_shape>` object Can only be used on :ref:`element::i64 <doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>` nodes and interprets negative values as zeros.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a0aed3d127309d7c9065d3f653ceead34:
.. index:: pair: function; get_strides_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Strides<doxid-classov_1_1_strides>` get_strides_val() const

Returns the value of the constant node as a :ref:`Strides <doxid-classov_1_1_strides>` object Can only be used on :ref:`element::i64 <doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>` nodes and interprets negative values as zeros.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1ac5feb281a38b4569a056e8bb3453cb12:
.. index:: pair: function; get_coordinate_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Coordinate<doxid-classov_1_1_coordinate>` get_coordinate_val() const

Returns the value of the constant node as a :ref:`Coordinate <doxid-classov_1_1_coordinate>` object Can only be used on :ref:`element::i64 <doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>` nodes and interprets negative values as zeros.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1af774b06fe106c32c9f0da920c8a269cc:
.. index:: pair: function; get_coordinate_diff_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>` get_coordinate_diff_val() const

Returns the value of the constant node as a :ref:`CoordinateDiff <doxid-classov_1_1_coordinate_diff>` object Can only be used on :ref:`element::i64 <doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>` nodes.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a21387d37bbb14791fba765e86cdbd1c0:
.. index:: pair: function; get_axis_vector_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`AxisVector<doxid-classov_1_1_axis_vector>` get_axis_vector_val() const

Returns the value of the constant node as an :ref:`AxisVector <doxid-classov_1_1_axis_vector>` object Can only be used on :ref:`element::i64 <doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>` nodes and interprets negative values as zeros.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a9bb2cff30b5c25ae35ed54e0bdb7b247:
.. index:: pair: function; get_axis_set_val

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`AxisSet<doxid-classov_1_1_axis_set>` get_axis_set_val() const

Returns the value of the constant node as an :ref:`AxisSet <doxid-classov_1_1_axis_set>` object Can only be used on :ref:`element::i64 <doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>` nodes and interprets negative values as zeros. Repeated values are allowed.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a8800b88fd610af80749ba715654f157a:
.. index:: pair: function; set_data_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_data_shape(const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

Update :ref:`Constant <doxid-classov_1_1op_1_1v0_1_1_constant>` shape. New shape size must equal to the data elements count.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- shape

		- The shape of the tensor constant.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a6a80bd52b75e981e087cb300faa86d24:
.. index:: pair: function; get_byte_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_byte_size() const

Return data size in bytes.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a3fc03d7d8f853464671833b83b61e9d6:
.. index:: pair: function; get_value_strings

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> get_value_strings() const



.. rubric:: Returns:

The initialization literals for the tensor constant.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1abd4d166d19ef4f7204abb53ec5247ce3:
.. index:: pair: function; cast_vector

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	std::vector<T> cast_vector() const

Return the :ref:`Constant <doxid-classov_1_1op_1_1v0_1_1_constant>` 's value as a vector cast to type T.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to which data vector's entries will be cast.



.. rubric:: Returns:

:ref:`Constant <doxid-classov_1_1op_1_1v0_1_1_constant>` 's data vector.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1aded3f3d661b74d480aa1e20c81a66c09:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static std::shared_ptr<Constant> create(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const std::vector<T>& values
		)

Wrapper around constructing a shared_ptr of a :ref:`Constant <doxid-classov_1_1op_1_1v0_1_1_constant>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- values

		- A vector of values to use as the constant data.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1ab834a9774972682a5b9d718c6bb21899:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static std::shared_ptr<Constant> create(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		std::initializer_list<T> values
		)

Wrapper around constructing a shared_ptr of a :ref:`Constant <doxid-classov_1_1op_1_1v0_1_1_constant>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- values

		- An initializer_list of values to use as the constant data.

.. _doxid-classov_1_1op_1_1v0_1_1_constant_1a4b02934a0557311027edfd7c81821669:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::shared_ptr<Constant> create(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const void \* memory
		)

Wrapper around constructing a shared_ptr of a :ref:`Constant <doxid-classov_1_1op_1_1v0_1_1_constant>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- The element type of the tensor constant.

	*
		- shape

		- The shape of the tensor constant.

	*
		- memory

		- An continues memory chunk which contains the constant data.


