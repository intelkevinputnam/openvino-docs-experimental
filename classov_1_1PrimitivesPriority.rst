.. index:: pair: class; ov::PrimitivesPriority
.. _doxid-classov_1_1_primitives_priority:

class ov::PrimitivesPriority
============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <primitives_priority_attribute.hpp>
	
	class PrimitivesPriority: public :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`
	{
	public:
		// fields
	
		std::string :target:`value<doxid-classov_1_1_primitives_priority_1aa8699faf56f541e0ac58ee9f127358db>`;

		// construction
	
		:target:`PrimitivesPriority<doxid-classov_1_1_primitives_priority_1a913183614c30504bc807c6d19c285408>`();
		:target:`PrimitivesPriority<doxid-classov_1_1_primitives_priority_1a09225c884da472a6cc8025e974f12035>`(const std::string& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_primitives_priority_1a4decae4882980c2b996883209d8b5749>`("primitives_priority", "0");
		:ref:`Any<doxid-classov_1_1_any>` :target:`merge<doxid-classov_1_1_primitives_priority_1a5bb22596c00ee9d5a1ef3b9bbd7df9c7>`(const :ref:`ngraph::NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& nodes) const;
		virtual bool :target:`visit_attributes<doxid-classov_1_1_primitives_priority_1aa7cf338a4abbeba214026abe7c6fe197>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		virtual std::string :target:`to_string<doxid-classov_1_1_primitives_priority_1a43fcdc9b05e41c14bbea8acac6dbde89>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Ptr<doxid-classov_1_1_runtime_attribute_1a0ac56ae81bace38d80c2c57e6695cf8f>`;
		typedef std::tuple<:::ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Base<doxid-classov_1_1_runtime_attribute_1aa8d1a337411d2728e4d8beb58eeb7ccc>`;

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


