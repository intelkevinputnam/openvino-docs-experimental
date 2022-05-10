.. index:: pair: class; ov::RuntimeAttribute
.. _doxid-classov_1_1_runtime_attribute:

class ov::RuntimeAttribute
==========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <runtime_attribute.hpp>
	
	class RuntimeAttribute
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<RuntimeAttribute> :target:`Ptr<doxid-classov_1_1_runtime_attribute_1a0ac56ae81bace38d80c2c57e6695cf8f>`;
		typedef std::tuple<::ov::RuntimeAttribute> :target:`Base<doxid-classov_1_1_runtime_attribute_1aa8d1a337411d2728e4d8beb58eeb7ccc>`;

		// methods
	
		static :ref:`_OPENVINO_HIDDEN_METHOD<doxid-core_2include_2openvino_2core_2visibility_8hpp_1a751977ff5ff49e1bfd5b4efc0b994f27>` const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info_static<doxid-classov_1_1_runtime_attribute_1a57fac9ef5e4f13144d53102212bed8c6>`();
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info<doxid-classov_1_1_runtime_attribute_1a1c452854e1d01d1852cca180327c6882>`() const;
		virtual bool :target:`is_copyable<doxid-classov_1_1_runtime_attribute_1a0813e513d24e9fc5c7a010732c179eb5>`() const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :target:`init<doxid-classov_1_1_runtime_attribute_1a85cfa598b9589c581cb1cdababf36cd6>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :target:`merge<doxid-classov_1_1_runtime_attribute_1abbc804f43f52cd6ed54fab2b6c7b573b>`(const :ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& nodes) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :target:`merge<doxid-classov_1_1_runtime_attribute_1a034010091b62f617c14e4576fcf56cb2>`(const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& outputs) const;
		virtual std::string :target:`to_string<doxid-classov_1_1_runtime_attribute_1aaf017b973a9eb4ef7e5d8466cf385ee4>`() const;
		virtual bool :target:`visit_attributes<doxid-classov_1_1_runtime_attribute_1abacd4929156e317cdb0c74d9cc714025>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		bool :target:`visit_attributes<doxid-classov_1_1_runtime_attribute_1ad41560d786103ecad79977ce84e68912>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) const;
	};

	// direct descendants

	class :ref:`FusedNames<doxid-classngraph_1_1_fused_names>`;
	class :ref:`QuantizationGranularityAttribute<doxid-classngraph_1_1_quantization_granularity_attribute>`;
	class :ref:`QuantizationModeAttribute<doxid-classngraph_1_1_quantization_mode_attribute>`;

	template <typename VT>
	class :ref:`VariantImpl<doxid-classngraph_1_1_variant_impl>`;

	class :ref:`Decompression<doxid-classov_1_1_decompression>`;
	class :ref:`DisableFP16Compression<doxid-classov_1_1_disable_f_p16_compression>`;
	class :ref:`LayoutAttribute<doxid-classov_1_1_layout_attribute>`;
	class :ref:`NmsSelectedIndices<doxid-classov_1_1_nms_selected_indices>`;
	class :ref:`NonconvertibleDivide<doxid-classov_1_1_nonconvertible_divide>`;
	class :ref:`OldApiMapElementType<doxid-classov_1_1_old_api_map_element_type>`;
	class :ref:`OldApiMapOrder<doxid-classov_1_1_old_api_map_order>`;
	class :ref:`DisableConstantFolding<doxid-classov_1_1pass_1_1_disable_constant_folding>`;
	class :ref:`PrecisionSensitive<doxid-classov_1_1_precision_sensitive>`;
	class :ref:`TensorInfoMemoryType<doxid-classov_1_1preprocess_1_1_tensor_info_memory_type>`;
	class :ref:`PreprocessingAttribute<doxid-classov_1_1_preprocessing_attribute>`;
	class :ref:`PrimitivesPriority<doxid-classov_1_1_primitives_priority>`;
	class :ref:`StridesPropagation<doxid-classov_1_1_strides_propagation>`;

	template <class T>
	class :ref:`SharedAttribute<doxid-class_shared_attribute>`;

