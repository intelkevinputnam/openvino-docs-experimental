.. index:: pair: class; ngraph::QuantizationModeAttribute
.. _doxid-classngraph_1_1_quantization_mode_attribute:

class ngraph::QuantizationModeAttribute
=======================================

.. toctree::
	:hidden:

	Mode <enumngraph_1_1QuantizationModeAttribute_1_1Mode.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <quantization_mode_attribute.hpp>
	
	class QuantizationModeAttribute: public :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`
	{
	public:
		// enums
	
		enum :ref:`Mode<doxid-classngraph_1_1_quantization_mode_attribute_1ae0aeb93d6c933f39c14ac2b72244e578>`;

		// fields
	
		:ref:`Mode<doxid-classngraph_1_1_quantization_mode_attribute_1ae0aeb93d6c933f39c14ac2b72244e578>` :target:`mode<doxid-classngraph_1_1_quantization_mode_attribute_1a8cef6c55c39ce63f9691cb6cec9191aa>`;

		// construction
	
		:target:`QuantizationModeAttribute<doxid-classngraph_1_1_quantization_mode_attribute_1a0c9b41c811c47c5be62ac262119dce4b>`();
		:target:`QuantizationModeAttribute<doxid-classngraph_1_1_quantization_mode_attribute_1a05b10c8ca61a681f685b2a186ea1171d>`(const :ref:`Mode<doxid-classngraph_1_1_quantization_mode_attribute_1ae0aeb93d6c933f39c14ac2b72244e578>` mode);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_quantization_mode_attribute_1a2dc06e9ac29d298a18a6fa25abff0ef7>`(
			"LowPrecision::QuantizationModeAttribute",
			"",
			:ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`,
			0
			);
	
		bool :target:`operator ==<doxid-classngraph_1_1_quantization_mode_attribute_1a194cb484a3b5853dda2777721b328133>` (const QuantizationModeAttribute& attribute) const;
		virtual std::string :target:`to_string<doxid-classngraph_1_1_quantization_mode_attribute_1a0ca83ee88ce71c931f26145da243d47a>`() const;
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


