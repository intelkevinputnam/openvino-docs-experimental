.. index:: pair: class; ngraph::VariantWrapper
.. _doxid-classngraph_1_1_variant_wrapper:

class ngraph::VariantWrapper
============================






.. index:: pair: class; ngraph::VariantWrapper<int64_t>
.. _doxid-classngraph_1_1_variant_wrapper_3_01int64__t_01_4:

class ngraph::VariantWrapper<int64_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variant.hpp>
	
	template <>
	class VariantWrapper<int64_t>: public :ref:`ngraph::VariantImpl<doxid-classngraph_1_1_variant_impl>`
	{
	public:
		// construction
	
		:target:`VariantWrapper<doxid-classngraph_1_1_variant_wrapper_3_01int64__t_01_4_1a083bca5fc6a8d889892597e4109b9ff8>`(const :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_variant_wrapper_3_01int64__t_01_4_1a5d1603bd66e22125f97d787b6eb30287>`("VariantWrapper<int64_t>");
		virtual std::string :target:`to_string<doxid-classngraph_1_1_variant_wrapper_3_01int64__t_01_4_1a6593227d0f3decc594962d07a19adfc3>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Ptr<doxid-classov_1_1_runtime_attribute_1a0ac56ae81bace38d80c2c57e6695cf8f>`;
		typedef std::tuple<:::ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Base<doxid-classov_1_1_runtime_attribute_1aa8d1a337411d2728e4d8beb58eeb7ccc>`;
		typedef VT :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`;

		// methods
	
		static :ref:`_OPENVINO_HIDDEN_METHOD<doxid-core_2include_2openvino_2core_2visibility_8hpp_1a751977ff5ff49e1bfd5b4efc0b994f27>` const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info_static<doxid-classov_1_1_runtime_attribute_1a57fac9ef5e4f13144d53102212bed8c6>`();
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_runtime_attribute_1a1c452854e1d01d1852cca180327c6882>`() const;
		virtual bool :ref:`is_copyable<doxid-classov_1_1_runtime_attribute_1a0813e513d24e9fc5c7a010732c179eb5>`() const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`init<doxid-classov_1_1_runtime_attribute_1a85cfa598b9589c581cb1cdababf36cd6>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`merge<doxid-classov_1_1_runtime_attribute_1abbc804f43f52cd6ed54fab2b6c7b573b>`(const :ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& nodes) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`merge<doxid-classov_1_1_runtime_attribute_1a034010091b62f617c14e4576fcf56cb2>`(const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& outputs) const;
		virtual std::string :ref:`to_string<doxid-classov_1_1_runtime_attribute_1aaf017b973a9eb4ef7e5d8466cf385ee4>`() const;
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_runtime_attribute_1abacd4929156e317cdb0c74d9cc714025>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		bool :ref:`visit_attributes<doxid-classov_1_1_runtime_attribute_1ad41560d786103ecad79977ce84e68912>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) const;
		:ref:`OPENVINO_RTTI<doxid-classngraph_1_1_variant_impl_1a1004b3991aba86836610f4c2312fe769>`(typeid(VT).name());
		const :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& :ref:`get<doxid-classngraph_1_1_variant_impl_1af9e0c31123848c871d61dce4fdc889c3>`() const;
		:ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& :ref:`get<doxid-classngraph_1_1_variant_impl_1a818ce83f210e764aef7de94466ebd904>`();
		void :ref:`set<doxid-classngraph_1_1_variant_impl_1a993dc3bb2100c379dbbcebdfb3f06859>`(const :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& value);


.. index:: pair: class; ngraph::VariantWrapper<std::string>
.. _doxid-classngraph_1_1_variant_wrapper_3_01std_1_1string_01_4:

class ngraph::VariantWrapper<std::string>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variant.hpp>
	
	template <>
	class VariantWrapper<std::string>: public :ref:`ngraph::VariantImpl<doxid-classngraph_1_1_variant_impl>`
	{
	public:
		// construction
	
		:target:`VariantWrapper<doxid-classngraph_1_1_variant_wrapper_3_01std_1_1string_01_4_1afd1288287d1ab84f40721392ff65c467>`(const :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_variant_wrapper_3_01std_1_1string_01_4_1aa853d02e6e2aaee3b34f2ecdd00de5c1>`("VariantWrapper<std::string>");
		virtual std::string :target:`to_string<doxid-classngraph_1_1_variant_wrapper_3_01std_1_1string_01_4_1a9606448ff8d8214efafe740424289378>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Ptr<doxid-classov_1_1_runtime_attribute_1a0ac56ae81bace38d80c2c57e6695cf8f>`;
		typedef std::tuple<:::ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Base<doxid-classov_1_1_runtime_attribute_1aa8d1a337411d2728e4d8beb58eeb7ccc>`;
		typedef VT :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`;

		// methods
	
		static :ref:`_OPENVINO_HIDDEN_METHOD<doxid-core_2include_2openvino_2core_2visibility_8hpp_1a751977ff5ff49e1bfd5b4efc0b994f27>` const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info_static<doxid-classov_1_1_runtime_attribute_1a57fac9ef5e4f13144d53102212bed8c6>`();
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_runtime_attribute_1a1c452854e1d01d1852cca180327c6882>`() const;
		virtual bool :ref:`is_copyable<doxid-classov_1_1_runtime_attribute_1a0813e513d24e9fc5c7a010732c179eb5>`() const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`init<doxid-classov_1_1_runtime_attribute_1a85cfa598b9589c581cb1cdababf36cd6>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`merge<doxid-classov_1_1_runtime_attribute_1abbc804f43f52cd6ed54fab2b6c7b573b>`(const :ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& nodes) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`merge<doxid-classov_1_1_runtime_attribute_1a034010091b62f617c14e4576fcf56cb2>`(const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& outputs) const;
		virtual std::string :ref:`to_string<doxid-classov_1_1_runtime_attribute_1aaf017b973a9eb4ef7e5d8466cf385ee4>`() const;
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_runtime_attribute_1abacd4929156e317cdb0c74d9cc714025>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		bool :ref:`visit_attributes<doxid-classov_1_1_runtime_attribute_1ad41560d786103ecad79977ce84e68912>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) const;
		:ref:`OPENVINO_RTTI<doxid-classngraph_1_1_variant_impl_1a1004b3991aba86836610f4c2312fe769>`(typeid(VT).name());
		const :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& :ref:`get<doxid-classngraph_1_1_variant_impl_1af9e0c31123848c871d61dce4fdc889c3>`() const;
		:ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& :ref:`get<doxid-classngraph_1_1_variant_impl_1a818ce83f210e764aef7de94466ebd904>`();
		void :ref:`set<doxid-classngraph_1_1_variant_impl_1a993dc3bb2100c379dbbcebdfb3f06859>`(const :ref:`value_type<doxid-classngraph_1_1_variant_impl_1a353c18b7615aee86dcbde7665ea2c004>`& value);


