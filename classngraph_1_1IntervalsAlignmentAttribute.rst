.. index:: pair: class; ngraph::IntervalsAlignmentAttribute
.. _doxid-classngraph_1_1_intervals_alignment_attribute:

class ngraph::IntervalsAlignmentAttribute
=========================================



Overview
~~~~~~~~

:ref:`IntervalsAlignmentAttribute <doxid-classngraph_1_1_intervals_alignment_attribute>` defines subgraph with the same quantization intervals alignment. FakeQuantize operations are included. The attribute is used by quantization operations. :ref:`More...<details-classngraph_1_1_intervals_alignment_attribute>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <intervals_alignment_attribute.hpp>
	
	class IntervalsAlignmentAttribute: public :ref:`SharedAttribute<doxid-class_shared_attribute>`
	{
	public:
		// fields
	
		size_t :target:`levels<doxid-classngraph_1_1_intervals_alignment_attribute_1a2624599e1009d7359852b44a2ed9f449>`;

		// construction
	
		:target:`IntervalsAlignmentAttribute<doxid-classngraph_1_1_intervals_alignment_attribute_1a01cd10a5f3a3571cc9a580acd7fc162b>`();
	
		:target:`IntervalsAlignmentAttribute<doxid-classngraph_1_1_intervals_alignment_attribute_1accb450686514b1abab2608ca9c25ce7b>`(
			:ref:`IntervalsAlignmentSharedValue::Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>` combinedInterval,
			size_t levels
			);
	
		:target:`IntervalsAlignmentAttribute<doxid-classngraph_1_1_intervals_alignment_attribute_1a09bba73bcc4b88ed85a97db0f7f1c810>`(
			const :ref:`IntervalsAlignmentSharedValue::Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>` combinedInterval,
			const size_t levels,
			const :ref:`IntervalsAlignmentSharedValue::Interval<doxid-classngraph_1_1_intervals_alignment_shared_value_1_1_interval>` minInterval,
			const size_t minLevels
			);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_intervals_alignment_attribute_1a67ac01b1a53e9023db36bce16f6beb05>`("LowPrecision::IntervalsAlignment", "", :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`, 0);
		void :target:`merge<doxid-classngraph_1_1_intervals_alignment_attribute_1a473f941fca86241aaf8090386bf5df67>`(std::vector<:ref:`ov::Any<doxid-classov_1_1_any>`>& attributes);
		virtual std::string :target:`to_string<doxid-classngraph_1_1_intervals_alignment_attribute_1a996cff4b302efb3a4ca16f4cbb74d94f>`() const;
	
		static :ref:`ov::Any<doxid-classov_1_1_any>` :target:`create<doxid-classngraph_1_1_intervals_alignment_attribute_1a720aeef6345d13187a4fed107bf68e69>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
			const :ref:`AttributeParameters<doxid-class_attribute_parameters>`& params = :ref:`AttributeParameters<doxid-class_attribute_parameters>`()
			);
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

.. _details-classngraph_1_1_intervals_alignment_attribute:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`IntervalsAlignmentAttribute <doxid-classngraph_1_1_intervals_alignment_attribute>` defines subgraph with the same quantization intervals alignment. FakeQuantize operations are included. The attribute is used by quantization operations.

For more details about the attribute, refer to :ref:`IntervalsAlignmentAttribute <doxid-openvino_docs__o_v__u_g_lpt__intervals_alignment>` page in the Inference Engine Developer Guide.


