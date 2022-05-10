.. index:: pair: class; ngraph::QuantizationGranularityAttribute
.. _doxid-classngraph_1_1_quantization_granularity_attribute:

class ngraph::QuantizationGranularityAttribute
==============================================

.. toctree::
	:hidden:

	Granularity <enumngraph_1_1QuantizationGranularityAttribute_1_1Granularity.rst>

Overview
~~~~~~~~

:ref:`QuantizationGranularityAttribute <doxid-classngraph_1_1_quantization_granularity_attribute>` defines quantization granularity of operation inputs. :ref:`More...<details-classngraph_1_1_quantization_granularity_attribute>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <quantization_granularity_attribute.hpp>
	
	class QuantizationGranularityAttribute: public :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`
	{
	public:
		// enums
	
		enum :ref:`Granularity<doxid-classngraph_1_1_quantization_granularity_attribute_1af0340f573997b98910c1f3c33742f530>`;

		// fields
	
		:ref:`Granularity<doxid-classngraph_1_1_quantization_granularity_attribute_1af0340f573997b98910c1f3c33742f530>` :target:`granularity<doxid-classngraph_1_1_quantization_granularity_attribute_1ab542bfef1d35d1eb154770149acf5baf>`;

		// construction
	
		:target:`QuantizationGranularityAttribute<doxid-classngraph_1_1_quantization_granularity_attribute_1a237bb597820cd9fc537cc918b2d25af0>`();
		:target:`QuantizationGranularityAttribute<doxid-classngraph_1_1_quantization_granularity_attribute_1a3ae36abd7701689f4f5e2410637e225c>`(const :ref:`Granularity<doxid-classngraph_1_1_quantization_granularity_attribute_1af0340f573997b98910c1f3c33742f530>` granularity);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_quantization_granularity_attribute_1a202faf44c0648a3efa48fff7ebc17cd9>`(
			"LowPrecision::QuantizationGranularity",
			"",
			:ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`,
			0
			);
	
		bool :target:`operator ==<doxid-classngraph_1_1_quantization_granularity_attribute_1adc3d973572ba39ddef0c43a3a160b75f>` (const QuantizationGranularityAttribute& attribute) const;
		bool :target:`is_skipped<doxid-classngraph_1_1_quantization_granularity_attribute_1acdaebd3caccc29ee6fbdd09cdfb6de2a>`() const;
		virtual std::string :target:`to_string<doxid-classngraph_1_1_quantization_granularity_attribute_1a4e8072b14952630026e85c651c42871c>`() const;
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

.. _details-classngraph_1_1_quantization_granularity_attribute:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`QuantizationGranularityAttribute <doxid-classngraph_1_1_quantization_granularity_attribute>` defines quantization granularity of operation inputs.

For more details about the attribute, refer to :ref:`QuantizationGranularityAttribute <doxid-openvino_docs__o_v__u_g_lpt__quantization_granularity>` page in the Inference Engine Developer Guide.


