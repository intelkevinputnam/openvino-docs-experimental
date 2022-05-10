.. index:: pair: class; ngraph::AvgPoolPrecisionPreservedAttribute
.. _doxid-classngraph_1_1_avg_pool_precision_preserved_attribute:

class ngraph::AvgPoolPrecisionPreservedAttribute
================================================



Overview
~~~~~~~~

:ref:`AvgPoolPrecisionPreservedAttribute <doxid-classngraph_1_1_avg_pool_precision_preserved_attribute>` is utility attribute which is used only during ``AvgPool`` operation precision preserved property definition. :ref:`More...<details-classngraph_1_1_avg_pool_precision_preserved_attribute>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <avg_pool_precision_preserved_attribute.hpp>
	
	class AvgPoolPrecisionPreservedAttribute: public :ref:`ngraph::PrecisionPreservedAttribute<doxid-classngraph_1_1_precision_preserved_attribute>`
	{
	public:
		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute_1a40b8ee28530638db911b20587c0eab05>`(
			"LowPrecision::AvgPoolPrecisionPreserved",
			"",
			:ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`,
			0
			);
	
		void :target:`merge<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute_1a1dfdf4ff41ebc7bf3c465eb54aa18319>`(std::vector<:ref:`ov::Any<doxid-classov_1_1_any>`>& attributes);
		bool :target:`is_skipped<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute_1a87b609a3c9ddb7d1d8907e528594dcdf>`() const;
		virtual std::string :target:`to_string<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute_1a07af8061bacf33b870d565d8a2313341>`() const;
		:target:`PrecisionPreservedAttribute<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute_1a8ea9cea6b0a6c01c544c786d3f5e6fba>`();
		:target:`PrecisionPreservedAttribute<doxid-classngraph_1_1_avg_pool_precision_preserved_attribute_1a9fc556f2f3980a5b8560f834bcc4d321>`(const bool value);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Ptr<doxid-classov_1_1_runtime_attribute_1a0ac56ae81bace38d80c2c57e6695cf8f>`;
		typedef std::tuple<:::ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Base<doxid-classov_1_1_runtime_attribute_1aa8d1a337411d2728e4d8beb58eeb7ccc>`;

		// classes
	
		class :ref:`SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute>`;

		// fields
	
		std::shared_ptr<:ref:`SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute>`> :ref:`attribute<doxid-class_shared_attribute_1a2c796ec7de4975ab5607fffc7c8911ae>`;

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
		const T& :ref:`value<doxid-class_shared_attribute_1a3f546aa49d29bf04b8d65b652f27f542>`() const;
		T& :ref:`value<doxid-class_shared_attribute_1ac87e7f7ec60ab080ba8f4c7bd0489f08>`();
		:ref:`OPENVINO_RTTI<doxid-classngraph_1_1_precision_preserved_attribute_1a43ef33cfa8a9dd6e9bc73b7be93e7533>`("LowPrecision::PrecisionPreserved", "", :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`, 0);
		virtual std::string :ref:`to_string<doxid-classngraph_1_1_precision_preserved_attribute_1ad4fc19f4288331ec4a14b7f2d9ebf6b8>`() const;

.. _details-classngraph_1_1_avg_pool_precision_preserved_attribute:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`AvgPoolPrecisionPreservedAttribute <doxid-classngraph_1_1_avg_pool_precision_preserved_attribute>` is utility attribute which is used only during ``AvgPool`` operation precision preserved property definition.

For more details about the attribute, refer to :ref:`AvgPoolPrecisionPreservedAttribute <doxid-openvino_docs__o_v__u_g_lpt__avg_pool_precision_preserved>` page in the Inference Engine Developer Guide.


