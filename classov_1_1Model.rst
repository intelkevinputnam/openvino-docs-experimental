.. index:: pair: class; ov::Model
.. _doxid-classov_1_1_model:

class ov::Model
===============



Overview
~~~~~~~~

A user-defined model. :ref:`More...<details-classov_1_1_model>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <model.hpp>
	
	class Model: public std::enable_shared_from_this< Model >
	{
	public:
		// typedefs
	
		typedef std::function<std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>>(const std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>>&root_nodes)> :target:`topological_sort_t<doxid-classov_1_1_model_1a2e2918a54565b98fdd3d075783a4be10>`;

		// fields
	
		static const :ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :target:`type_info<doxid-classov_1_1_model_1ab2dd3101fa5b7c16f3b4c142fad0d111>`;

		// construction
	
		:target:`Model<doxid-classov_1_1_model_1a34412328546ca6960265c8b1923bf2c5>`(
			const :ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& results,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1a95cac8876a1ab29e3051cad2c3bc220d>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1a7b73d36066acb45bddaead13dd17a081>`(
			const std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>& result,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1a0d68585358a7d6b418b24f1d50c6e8b8>`(
			const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& results,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1abe204375d9a6504b54829721263a7599>`(
			const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& results,
			const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1a569171d9bd3409e5989f1507c7dbb770>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results,
			const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1a75f83a92bed5649081892741f0bc02e6>`(
			const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& results,
			const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& variables,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1aade633790d14265488e9cb84684e16bb>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results,
			const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& variables,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1aeb255a47f503950f9aedd2a031f13272>`(
			const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& results,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& variables,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1af11ce9c602c700693af7959cd9d68329>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results,
			const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& parameters,
			const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& variables,
			const std::string& name = ""
			);
	
		:ref:`Model<doxid-classov_1_1_model_1a7a622cfc1950e80081771d54226dbcc9>`(const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results, const std::string& name = "");
	
		:ref:`Model<doxid-classov_1_1_model_1a0a13212ea1dfea183e99dece6cea169c>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results,
			const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks,
			const std::string& name = ""
			);
	
		:target:`Model<doxid-classov_1_1_model_1a2c42fa59fb6de52bf94e6dad9d021ba4>`(const Model&);
		:target:`Model<doxid-classov_1_1_model_1ac290c034ac5edff7f76bc1aa501f9012>`(Model&&);

		// methods
	
		static _OPENVINO_HIDDEN_METHODconst :::ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info_static<doxid-classov_1_1_model_1a3e1e2c4fdd257e6bd5f27601a326557f>`();
		const :::ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info<doxid-classov_1_1_model_1a208ba36c3a1a23d70c6fb4b37e59dd71>`() const;
		size_t :ref:`get_output_size<doxid-classov_1_1_model_1a495378df3029c9b36522bbb16f9287cc>`() const;
		std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`get_output_op<doxid-classov_1_1_model_1a45aab1fcda019daee294caa8b14f3699>`(size_t i) const;
		std::shared_ptr<ov::Model> :ref:`clone<doxid-classov_1_1_model_1a6837448bf09d8658e38e79fd4349037a>`() const;
		std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>> :ref:`outputs<doxid-classov_1_1_model_1a89c629856666f1064cf0418c432004f0>`();
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`output<doxid-classov_1_1_model_1a77b209dd9632a199c20fd48b0e5cab62>`();
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`output<doxid-classov_1_1_model_1a6a5739e3dabb97d6ebffff4cf00286f9>`(size_t i);
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`output<doxid-classov_1_1_model_1a00202f65d5b9da2b58421770d4ff0b1a>`(const std::string& tensor_name);
		std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>> :target:`outputs<doxid-classov_1_1_model_1ab09f86a7d7dc86788adc5ca780976829>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :target:`output<doxid-classov_1_1_model_1a37278f5332585f1f14a16ab779335548>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :target:`output<doxid-classov_1_1_model_1abe0ffba063e7507d58847130e5148e0c>`(size_t i) const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :target:`output<doxid-classov_1_1_model_1a453358c0840601e83dc49149211f5a2f>`(const std::string& tensor_name) const;
		std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>> :ref:`inputs<doxid-classov_1_1_model_1a7121b50a2990b63eb6a73945f0cae089>`();
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`input<doxid-classov_1_1_model_1a9bf0166a1f9005222cb9a2f68a3b9a4c>`();
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`input<doxid-classov_1_1_model_1ae97dfe56bd509cce144d1903c43fde51>`(size_t i);
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`input<doxid-classov_1_1_model_1a8bd3f633d51d6c08b5d820e779e4ee1c>`(const std::string& tensor_name);
		std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>> :target:`inputs<doxid-classov_1_1_model_1a0965ecca76fd9aa7c72a7f48d5f50b49>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :target:`input<doxid-classov_1_1_model_1a5103de2f45aa06f40d9975e3be981f86>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :target:`input<doxid-classov_1_1_model_1ae442b7c52bc92f660c5dedd5a38bfbe9>`(size_t i) const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`> :target:`input<doxid-classov_1_1_model_1a62c13c01a08017749a6070f56bea081a>`(const std::string& tensor_name) const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`add_output<doxid-classov_1_1_model_1a812b8153ecf214f28f741761acfb2de9>`(const std::string& tensor_name);
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`add_output<doxid-classov_1_1_model_1ac37f54a727a7edd27ec3b405f2d7998f>`(const std::string& op_name, size_t output_idx);
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`> :target:`add_output<doxid-classov_1_1_model_1a75c2cc44dae796e6772918ddab99c0c8>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& port);
		void :target:`reshape<doxid-classov_1_1_model_1aa21aff80598d5089d591888a4c7f33ae>`(const :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& partial_shape);
		void :target:`reshape<doxid-classov_1_1_model_1a72bffbdd00f3947d44ef42f1ca477d3e>`(const std::map<size_t, :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& partial_shapes);
		void :target:`reshape<doxid-classov_1_1_model_1a519e773c76d218e7c755f52e9a3ad196>`(const std::map<std::string, :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& partial_shapes);
		void :target:`reshape<doxid-classov_1_1_model_1a700b8bfcf5596b5f2b8fdc942f0b30f1>`(const std::map<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>, :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`>& partial_shapes);
		const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_output_element_type<doxid-classov_1_1_model_1ad00c1d863d5d1175f9b53ecd4ee79bef>`(size_t i) const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_output_shape<doxid-classov_1_1_model_1af197bf031e7e69c21d191593bc96027a>`(size_t i) const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_output_partial_shape<doxid-classov_1_1_model_1a12f48699294215965a4bf1ea9c70ea93>`(size_t i) const;
		std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> :ref:`get_result<doxid-classov_1_1_model_1ae67fa23e41fc5117d81c4aea2e3a84a4>`() const;
		const std::string& :ref:`get_name<doxid-classov_1_1_model_1abeca2ccc5f53e96e1423b5d1dcdcba26>`() const;
		void :ref:`set_friendly_name<doxid-classov_1_1_model_1ae2b870ed7c5f4c369980b366b7e7b44c>`(const std::string& name);
		const std::string& :ref:`get_friendly_name<doxid-classov_1_1_model_1a7f981f85e9f95dce670b82cfc673368c>`() const;
		std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>> :target:`get_ops<doxid-classov_1_1_model_1aa59b85f01b9660f69d9616f2ca40c3ef>`() const;
		std::vector<std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>> :target:`get_ordered_ops<doxid-classov_1_1_model_1a5324fa9ea3897161a8879f21ba6d5192>`() const;
		void :target:`map_unordered_ops<doxid-classov_1_1_model_1a0a70e480ccac6b4f23b091a386a6b08e>`(std::function<void(:ref:`ov::Node<doxid-classov_1_1_node>` \*)> f) const;
		void :target:`replace_node<doxid-classov_1_1_model_1a65e6503e85ead090c930adedaf7c3787>`(std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> old, std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> repl);
		void :target:`validate_nodes_and_infer_types<doxid-classov_1_1_model_1aa9869a9fe1854587894881e452252c82>`() const;
		size_t :ref:`get_graph_size<doxid-classov_1_1_model_1acee6b571b65a11843476616db6ec6a66>`() const;
		bool :ref:`is_dynamic<doxid-classov_1_1_model_1ace78bc92f1046ac2ba8207029b1206fc>`() const;
	
		void :ref:`replace_parameter<doxid-classov_1_1_model_1a4bcc29f28fc5eaa7caee849491887fb0>`(
			size_t parameter_index,
			const std::shared_ptr<:ref:`ov::op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>& parameter
			);
	
		void :target:`set_topological_sort<doxid-classov_1_1_model_1a0922f33917d4023509ef49677736f032>`(:ref:`topological_sort_t<doxid-classov_1_1_model_1a2e2918a54565b98fdd3d075783a4be10>`);
		virtual bool :target:`visit_attributes<doxid-classov_1_1_model_1a6d8f02f26c90ade902ee5df33e939304>`(:ref:`ov::AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& :ref:`get_parameters<doxid-classov_1_1_model_1a035279c6d62ab4e2d58606f24ad312f4>`() const;
		const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& :ref:`get_results<doxid-classov_1_1_model_1ae062eb2a6b7729b3ab398af05effda8a>`() const;
		int64_t :ref:`get_parameter_index<doxid-classov_1_1_model_1aa34cf485058100fde1329e24a91c7440>`(const std::shared_ptr<:ref:`ov::op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>& parameter) const;
		int64_t :ref:`get_result_index<doxid-classov_1_1_model_1abccf7a86adf919a60cc4206684b8236f>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& value) const;
		int64_t :ref:`get_result_index<doxid-classov_1_1_model_1a090cb5854c213eec5bfdfcc57d89fa53>`(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& value) const;
	
		bool :ref:`evaluate<doxid-classov_1_1_model_1ac1e725aeeb2d68dd7f7fd696534e11fa>`(
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_tensors,
			const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_tensors,
			:ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>` evaluation_context = :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`()
			) const;
	
		bool :ref:`evaluate<doxid-classov_1_1_model_1abe8c8f16f5bb35f5e935070a194eeed0>`(
			:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_tensors,
			const :ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& input_tensors,
			:ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>` evaluation_context = :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`()
			) const;
	
		const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& :ref:`get_sinks<doxid-classov_1_1_model_1a5ed86622a021261b8483ea2635f31034>`() const;
		void :ref:`add_sinks<doxid-classov_1_1_model_1a2050d478ff2fd7e665c64bcde4e842fa>`(const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks);
		void :ref:`remove_sink<doxid-classov_1_1_model_1a19f4bdecb589fc466c746368bd1b5bfd>`(const std::shared_ptr<:ref:`ov::op::Sink<doxid-classov_1_1op_1_1_sink>`>& sink);
		void :ref:`add_results<doxid-classov_1_1_model_1a838b3ab179ae22f1193e56e2b7ab7094>`(const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& results);
		void :ref:`remove_result<doxid-classov_1_1_model_1a53a74feddee42a8bec333ccd6317b453>`(const std::shared_ptr<:ref:`ov::op::v0::Result<doxid-classov_1_1op_1_1v0_1_1_result>`>& result);
		void :ref:`add_parameters<doxid-classov_1_1_model_1ada0ad94e62a7ef06a8420be30eea928c>`(const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& params);
		void :ref:`remove_parameter<doxid-classov_1_1_model_1a04e3f3b126c2b0890aa2796e147ec11c>`(const std::shared_ptr<:ref:`ov::op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>& param);
		void :ref:`add_variables<doxid-classov_1_1_model_1a5913105036357b5ab67f95a745ed73f4>`(const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& variables);
		void :ref:`remove_variable<doxid-classov_1_1_model_1a965c94b335d3385302b9f57172e371dd>`(const :ref:`ov::op::util::Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable);
		const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& :ref:`get_variables<doxid-classov_1_1_model_1adda96e31df1d0691bb6cf2996c74f361>`() const;
		:ref:`ov::op::util::Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>` :ref:`get_variable_by_id<doxid-classov_1_1_model_1ae16a6fea854fcf916f149fc345070002>`(const std::string& variable_id) const;
		:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1_model_1aba81b2f3c2d661ad76b48da682e3d106>`();
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1_model_1afd1365256209524e1d184679b24e06e5>`() const;
		Model& :target:`operator =<doxid-classov_1_1_model_1aef4cbf76311e8abc93b63be6c50162af>` (const Model&);
		Model& :target:`operator =<doxid-classov_1_1_model_1a5f97c340ea858667a38b7f888d5989c1>` (Model&&);
	};
.. _details-classov_1_1_model:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A user-defined model.

Construction
------------

.. _doxid-classov_1_1_model_1a7a622cfc1950e80081771d54226dbcc9:
.. index:: pair: function; Model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Model(const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results, const std::string& name = "")

Constructs a :ref:`Model <doxid-classov_1_1_model>`. Lists of parameters and variables will be generated automatically based on traversing the graph from the results.

.. _doxid-classov_1_1_model_1a0a13212ea1dfea183e99dece6cea169c:
.. index:: pair: function; Model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Model(
		const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& results,
		const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks,
		const std::string& name = ""
		)

Constructs a :ref:`Model <doxid-classov_1_1_model>`. Lists of parameters and variables will be generated automatically based on traversing the graph from the results and the sinks.

Methods
-------

.. _doxid-classov_1_1_model_1a495378df3029c9b36522bbb16f9287cc:
.. index:: pair: function; get_output_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_output_size() const

Return the number of outputs for this :ref:`Model <doxid-classov_1_1_model>`.

.. _doxid-classov_1_1_model_1a45aab1fcda019daee294caa8b14f3699:
.. index:: pair: function; get_output_op

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> get_output_op(size_t i) const

Return the op that generates output i.

.. _doxid-classov_1_1_model_1a6837448bf09d8658e38e79fd4349037a:
.. index:: pair: function; clone

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<ov::Model> clone() const

Clones the original model.

.. _doxid-classov_1_1_model_1a89c629856666f1064cf0418c432004f0:
.. index:: pair: function; outputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>> outputs()

:ref:`Model <doxid-classov_1_1_model>` outputs.

.. _doxid-classov_1_1_model_1a7121b50a2990b63eb6a73945f0cae089:
.. index:: pair: function; inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>> inputs()

:ref:`Model <doxid-classov_1_1_model>` inputs.

.. _doxid-classov_1_1_model_1ad00c1d863d5d1175f9b53ecd4ee79bef:
.. index:: pair: function; get_output_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& get_output_element_type(size_t i) const

Return the element type of output i.

.. _doxid-classov_1_1_model_1af197bf031e7e69c21d191593bc96027a:
.. index:: pair: function; get_output_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_output_shape(size_t i) const

Return the shape of element i.

.. _doxid-classov_1_1_model_1a12f48699294215965a4bf1ea9c70ea93:
.. index:: pair: function; get_output_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_output_partial_shape(size_t i) const

Return the partial shape of element i.

.. _doxid-classov_1_1_model_1ae67fa23e41fc5117d81c4aea2e3a84a4:
.. index:: pair: function; get_result

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> get_result() const

Check that there is a single result and return it.

.. _doxid-classov_1_1_model_1abeca2ccc5f53e96e1423b5d1dcdcba26:
.. index:: pair: function; get_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& get_name() const

Get the unique name of the model.



.. rubric:: Returns:

A const reference to the model's unique name.

.. _doxid-classov_1_1_model_1ae2b870ed7c5f4c369980b366b7e7b44c:
.. index:: pair: function; set_friendly_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_friendly_name(const std::string& name)

Sets a friendly name for a model. This does not overwrite the unique name of the model and is retrieved via :ref:`get_friendly_name() <doxid-classov_1_1_model_1a7f981f85e9f95dce670b82cfc673368c>`. Used mainly for debugging.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- is the friendly name to set

.. _doxid-classov_1_1_model_1a7f981f85e9f95dce670b82cfc673368c:
.. index:: pair: function; get_friendly_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& get_friendly_name() const

Gets the friendly name for a model. If no friendly name has been set via set_friendly_name then the model's unique name is returned.



.. rubric:: Returns:

A const reference to the model's friendly name.

.. _doxid-classov_1_1_model_1acee6b571b65a11843476616db6ec6a66:
.. index:: pair: function; get_graph_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_graph_size() const

Returns the sum of the size of all nodes in the graph plus the size of all constant data. This has little value beyond comparing the relative size of graphs and should not be considered the actual memory consumption of a graph.

.. _doxid-classov_1_1_model_1ace78bc92f1046ac2ba8207029b1206fc:
.. index:: pair: function; is_dynamic

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_dynamic() const

Returns true if any of the op's defined in the model contains partial shape.

.. _doxid-classov_1_1_model_1a4bcc29f28fc5eaa7caee849491887fb0:
.. index:: pair: function; replace_parameter

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void replace_parameter(
		size_t parameter_index,
		const std::shared_ptr<:ref:`ov::op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>& parameter
		)

Replace the ``parameter_index`` th parameter of the model with ``parameter``.

All users of the ``parameter_index`` th parameter are redirected to ``parameter``, and the ``parameter_index`` th entry in the model parameter list is replaced with ``parameter``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- parameter_index

		- The index of the parameter to replace.

	*
		- parameter

		- The parameter to substitute for the ``parameter_index`` th parameter.

.. _doxid-classov_1_1_model_1a035279c6d62ab4e2d58606f24ad312f4:
.. index:: pair: function; get_parameters

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& get_parameters() const

Return the model parameters.

.. _doxid-classov_1_1_model_1ae062eb2a6b7729b3ab398af05effda8a:
.. index:: pair: function; get_results

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& get_results() const

Return a list of model's outputs.

.. _doxid-classov_1_1_model_1aa34cf485058100fde1329e24a91c7440:
.. index:: pair: function; get_parameter_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t get_parameter_index(const std::shared_ptr<:ref:`ov::op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>& parameter) const

Index for parameter, or -1.

.. _doxid-classov_1_1_model_1abccf7a86adf919a60cc4206684b8236f:
.. index:: pair: function; get_result_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t get_result_index(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>& value) const

Return the index of this model's Result represented by the "value" :ref:`Output <doxid-classov_1_1_output>` object. This method returns -1 if an the passed output is not related to the Results of a model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- :ref:`Output <doxid-classov_1_1_output>` containing :ref:`Node <doxid-classov_1_1_node>`

.. _doxid-classov_1_1_model_1a090cb5854c213eec5bfdfcc57d89fa53:
.. index:: pair: function; get_result_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t get_result_index(const :ref:`ov::Output<doxid-classov_1_1_output>`<const :ref:`ov::Node<doxid-classov_1_1_node>`>& value) const

Return the index of this model's Result represented by the "value" :ref:`Output <doxid-classov_1_1_output>` object. This method returns -1 if an the passed output is not related to the Results of a model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- :ref:`Output <doxid-classov_1_1_output>` containing :ref:`Node <doxid-classov_1_1_node>`

.. _doxid-classov_1_1_model_1ac1e725aeeb2d68dd7f7fd696534e11fa:
.. index:: pair: function; evaluate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool evaluate(
		const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& output_tensors,
		const :ref:`ov::HostTensorVector<doxid-namespaceov_1a2e5bf6dcca008b0147e825595f57c03b>`& input_tensors,
		:ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>` evaluation_context = :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`()
		) const

Evaluate the model on inputs, putting results in outputs.

Deprecated Use evaluate with :ref:`ov::Tensor <doxid-classov_1_1_tensor>` instead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_tensors

		- Tensors for the outputs to compute. One for each result

	*
		- input_tensors

		- Tensors for the inputs. One for each inputs.

	*
		- evaluation_context

		- Storage of additional settings and attributes that can be used when evaluating the model. This additional information can be shared across nodes.

.. _doxid-classov_1_1_model_1abe8c8f16f5bb35f5e935070a194eeed0:
.. index:: pair: function; evaluate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool evaluate(
		:ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& output_tensors,
		const :ref:`ov::TensorVector<doxid-namespaceov_1aa2127061451ba4f5a6e6904b88e72c6e>`& input_tensors,
		:ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>` evaluation_context = :ref:`ov::EvaluationContext<doxid-namespaceov_1a46b08f86068f674a4e0748651b85a4b6>`()
		) const

Evaluate the model on inputs, putting results in outputs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_tensors

		- Tensors for the outputs to compute. One for each result

	*
		- input_tensors

		- Tensors for the inputs. One for each inputs.

	*
		- evaluation_context

		- Storage of additional settings and attributes that can be used when evaluating the model. This additional information can be shared across nodes.

.. _doxid-classov_1_1_model_1a5ed86622a021261b8483ea2635f31034:
.. index:: pair: function; get_sinks

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& get_sinks() const

Return a list of model's sinks.

.. _doxid-classov_1_1_model_1a2050d478ff2fd7e665c64bcde4e842fa:
.. index:: pair: function; add_sinks

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_sinks(const :ref:`ov::SinkVector<doxid-namespaceov_1ac3345f8bb7cf21a546f437de5f1db333>`& sinks)

Add new sink nodes to the list. Method doesn't validate graph, it should be done manually after all changes.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- sinks

		- new sink nodes

.. _doxid-classov_1_1_model_1a19f4bdecb589fc466c746368bd1b5bfd:
.. index:: pair: function; remove_sink

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_sink(const std::shared_ptr<:ref:`ov::op::Sink<doxid-classov_1_1op_1_1_sink>`>& sink)

Delete sink node from the list of sinks. Method doesn't delete node from graph.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- sink

		- Sink to delete

.. _doxid-classov_1_1_model_1a838b3ab179ae22f1193e56e2b7ab7094:
.. index:: pair: function; add_results

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_results(const :ref:`ov::ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& results)

Add new Result nodes to the list. Method doesn't validate graph, it should be done manually after all changes.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- results

		- new Result nodes

.. _doxid-classov_1_1_model_1a53a74feddee42a8bec333ccd6317b453:
.. index:: pair: function; remove_result

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_result(const std::shared_ptr<:ref:`ov::op::v0::Result<doxid-classov_1_1op_1_1v0_1_1_result>`>& result)

Delete Result node from the list of results. Method will not delete node from graph.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- result

		- Result node to delete

.. _doxid-classov_1_1_model_1ada0ad94e62a7ef06a8420be30eea928c:
.. index:: pair: function; add_parameters

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_parameters(const :ref:`ov::ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& params)

Add new Parameter nodes to the list.

Method doesn't change or validate graph, it should be done manually. For example, if you want to replace ``ReadValue`` node by ``Parameter``, you should do the following steps:

* replace node ``ReadValue`` by ``Parameter`` in graph

* call add_parameter() to add new input to the list

* call graph validation to check correctness of changes



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- params

		- new Parameter nodes

.. _doxid-classov_1_1_model_1a04e3f3b126c2b0890aa2796e147ec11c:
.. index:: pair: function; remove_parameter

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_parameter(const std::shared_ptr<:ref:`ov::op::v0::Parameter<doxid-classov_1_1op_1_1v0_1_1_parameter>`>& param)

Delete Parameter node from the list of parameters. Method will not delete node from graph. You need to replace Parameter with other operation manually. Attention: Indexing of parameters can be changed.

Possible use of method is to replace input by variable. For it the following steps should be done:

* ``Parameter`` node should be replaced by ``ReadValue``

* call remove_parameter(param) to remove input from the list

* check if any parameter indexes are saved/used somewhere, update it for all inputs because indexes can be changed

* call graph validation to check all changes



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- param

		- Parameter node to delete

.. _doxid-classov_1_1_model_1a5913105036357b5ab67f95a745ed73f4:
.. index:: pair: function; add_variables

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_variables(const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& variables)

Add new variables to the list. Method doesn't validate graph, it should be done manually after all changes.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variables

		- new variables to add

.. _doxid-classov_1_1_model_1a965c94b335d3385302b9f57172e371dd:
.. index:: pair: function; remove_variable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_variable(const :ref:`ov::op::util::Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable)

Delete variable from the list of variables. Method doesn't delete nodes that used this variable from the graph.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable

		- Variable to delete

.. _doxid-classov_1_1_model_1adda96e31df1d0691bb6cf2996c74f361:
.. index:: pair: function; get_variables

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ov::op::util::VariableVector<doxid-namespaceov_1_1op_1_1util_1af06f1f0c7c82505f2c71066de68e775d>`& get_variables() const

Return a list of model's variables.

.. _doxid-classov_1_1_model_1ae16a6fea854fcf916f149fc345070002:
.. index:: pair: function; get_variable_by_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::op::util::Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>` get_variable_by_id(const std::string& variable_id) const

Return a variable by specified variable_id.


