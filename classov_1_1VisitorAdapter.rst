.. index:: pair: class; ov::VisitorAdapter
.. _doxid-classov_1_1_visitor_adapter:

class ov::VisitorAdapter
========================



Adapters will see visitor.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	class VisitorAdapter: public :ref:`ov::ValueAccessor<void><doxid-classov_1_1_value_accessor_3_01void_01_4>`
	{
	public:
		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;
	};

	// direct descendants

	template <>
	class :ref:`AttributeAdapter<op::AutoBroadcastSpec><doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_spec_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::BroadcastModeSpec><doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_mode_spec_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::NodeVector><doxid-classov_1_1_attribute_adapter_3_01ov_1_1_node_vector_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ParameterVector><doxid-classov_1_1_attribute_adapter_3_01_parameter_vector_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ResultVector><doxid-classov_1_1_attribute_adapter_3_01_result_vector_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::shared_ptr<ov::Node>><doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_node_01_4_01_4>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


