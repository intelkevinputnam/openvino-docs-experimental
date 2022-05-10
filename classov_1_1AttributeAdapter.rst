.. index:: pair: class; ov::AttributeAdapter<ov::PartialShape>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_partial_shape_01_4:

class ov::AttributeAdapter<ov::PartialShape>
============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <partial_shape.hpp>
	
	template <>
	class AttributeAdapter<ov::PartialShape>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_partial_shape_01_4_1aade0789afc540c3fe00a881b5da66991>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_partial_shape_01_4_1aab52ce50d68668d00708a871841f4007>`(:ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_partial_shape_01_4_1a640afb10ea071846645d9af528bc8670>`("AttributeAdapter<:ref:`PartialShape<doxid-classov_1_1_partial_shape>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<ov::op::util::FrameworkNodeAttrs>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1op_1_1util_1_1_framework_node_attrs_01_4:

class ov::AttributeAdapter<ov::op::util::FrameworkNodeAttrs>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <framework_node.hpp>
	
	template <>
	class AttributeAdapter<ov::op::util::FrameworkNodeAttrs>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1op_1_1util_1_1_framework_node_attrs_01_4_1ae15ef5c5d941050e9cafdf8b45446dd7>`(:ref:`ov::op::util::FrameworkNodeAttrs<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1op_1_1util_1_1_framework_node_attrs_01_4_1ad7bde4d743e5733a7f0d149253819e33>`("AttributeAdapter<FrameworkNodeAttr>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<ov::Shape>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_shape_01_4:

class ov::AttributeAdapter<ov::Shape>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <shape.hpp>
	
	template <>
	class AttributeAdapter<ov::Shape>: public :ref:`ov::IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_shape_01_4_1ad0cd793c93f1f02a0f4a4cb1086315ac>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_shape_01_4_1ad6ece946bd639a2780b103d4954ea626>`(:ref:`ov::Shape<doxid-classov_1_1_shape>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_shape_01_4_1a75729b3611993ed62845e1f4f91acb11>`("AttributeAdapter<:ref:`Shape<doxid-classov_1_1_shape>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_vector_value_accessor_1a92bfd6646dbb5351205f6ad3d9e11b3a>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		:ref:`operator AT &<doxid-classov_1_1_indirect_vector_value_accessor_1ad197d00c5756ba246f2a391d8d22aa02>` ();


.. index:: pair: class; ov::AttributeAdapter<ParameterVector>
.. _doxid-classov_1_1_attribute_adapter_3_01_parameter_vector_01_4:

class ov::AttributeAdapter<ParameterVector>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <parameter.hpp>
	
	template <>
	class AttributeAdapter<ParameterVector>: public :ref:`ov::VisitorAdapter<doxid-classov_1_1_visitor_adapter>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01_parameter_vector_01_4_1ac1cdc45b633cbe148ad71c973997ef9a>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_parameter_vector_01_4_1a8bd8c2f27ba878a72b23d20742c6507b>`(:ref:`ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`& ref);

		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_attribute_adapter_3_01_parameter_vector_01_4_1a2d04bcac199deec45aad9e0eb7175a51>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_parameter_vector_01_4_1afc32c90d74467d960602f1d3a02e4423>`("AttributeAdapter<:ref:`ParameterVector<doxid-namespaceov_1a2fd9bce881f1d37b496cf2e098274098>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;


.. index:: pair: class; ov::AttributeAdapter<ResultVector>
.. _doxid-classov_1_1_attribute_adapter_3_01_result_vector_01_4:

class ov::AttributeAdapter<ResultVector>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <result.hpp>
	
	template <>
	class AttributeAdapter<ResultVector>: public :ref:`ov::VisitorAdapter<doxid-classov_1_1_visitor_adapter>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01_result_vector_01_4_1aa6d215cbcba3a8f7acabdbdecc20349f>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_result_vector_01_4_1a5e6ba988550dc860b3b090d55f441a22>`(:ref:`ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`& ref);

		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_attribute_adapter_3_01_result_vector_01_4_1aa2698d7aae84babd65f3709c9734e8b4>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_result_vector_01_4_1a7dcd1e50b2febd24ffe1d063f388106d>`("AttributeAdapter<:ref:`ResultVector<doxid-namespaceov_1adf9015702d0f2f7e69c705651f19b72a>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;


.. index:: pair: class; ov::AttributeAdapter<std::set<std::string>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1set_3_01std_1_1string_01_4_01_4:

class ov::AttributeAdapter<std::set<std::string>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::set<std::string>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1set_3_01std_1_1string_01_4_01_4_1a5cdedaf60200ea8b21a09317aa828507>`(std::set<std::string>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1set_3_01std_1_1string_01_4_01_4_1a7c4be59867ae7818ed5b3383eac482a1>`("AttributeAdapter<:ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`<string>>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<ov::NodeVector>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_node_vector_01_4:

class ov::AttributeAdapter<ov::NodeVector>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node.hpp>
	
	template <>
	class AttributeAdapter<ov::NodeVector>: public :ref:`ov::VisitorAdapter<doxid-classov_1_1_visitor_adapter>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_node_vector_01_4_1a9ca7f361af021aa04f37c155087e00fd>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_node_vector_01_4_1acb4bf142e68fbe03d12733ee5bd2e42b>`(:ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& ref);

		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_node_vector_01_4_1a77226a6df959975037992014301bbaef>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_node_vector_01_4_1a54bbcdd2ef6552ff758c7760c57d2185>`("AttributeAdapter<:ref:`NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;


.. index:: pair: class; ov::AttributeAdapter<std::shared_ptr<ngraph::runtime::AlignedBuffer>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ngraph_1_1runtime_1_1_aligned_buffer_01_4_01_4:

class ov::AttributeAdapter<std::shared_ptr<ngraph::runtime::AlignedBuffer>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <aligned_buffer.hpp>
	
	template <>
	class AttributeAdapter<std::shared_ptr<ngraph::runtime::AlignedBuffer>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ngraph_1_1runtime_1_1_aligned_buffer_01_4_01_4_1aea6436ef94d028610dd5895d5f8b58e8>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ngraph_1_1runtime_1_1_aligned_buffer_01_4_01_4_1ade666dff3f4fcaf14eb84e1744c90a29>`(std::shared_ptr<:ref:`ngraph::runtime::AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer>`>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ngraph_1_1runtime_1_1_aligned_buffer_01_4_01_4_1ad726c5cca42ccce67115503a9e1b00cd>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<ov::element::TypeVector>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_vector_01_4:

class ov::AttributeAdapter<ov::element::TypeVector>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <element_type.hpp>
	
	template <>
	class AttributeAdapter<ov::element::TypeVector>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_vector_01_4_1aa34441c0d2db80d8f67a08cf623a84df>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_vector_01_4_1a0b762ec743831243eef39e86962867d4>`(:ref:`ov::element::TypeVector<doxid-namespaceov_1_1element_1a7f46cb660ffbefcd50cfa90d8bfe0824>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_vector_01_4_1a15e176a71893949c9c6ad3f6604e930d>`("AttributeAdapter<:ref:`ov::element::TypeVector<doxid-namespaceov_1_1element_1a7f46cb660ffbefcd50cfa90d8bfe0824>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<ov::element::Type_t>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type__t_01_4:

class ov::AttributeAdapter<ov::element::Type_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <element_type.hpp>
	
	template <>
	class AttributeAdapter<ov::element::Type_t>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type__t_01_4_1ab37ce8376b113b39bd50fb0596c0d8c8>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type__t_01_4_1ac21ef1caf73c09e847730decc2d2a020>`(:ref:`ov::element::Type_t<doxid-group__ov__element__cpp__api_1gac13a83fdcf171bd2c98577bfcd37f2f1>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type__t_01_4_1a62c2479cc4be07a43d83ed1f9f3550bd>`("AttributeAdapter<:ref:`ov::element::Type_t<doxid-group__ov__element__cpp__api_1gac13a83fdcf171bd2c98577bfcd37f2f1>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<ov::element::Type>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4:

class ov::AttributeAdapter<ov::element::Type>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <element_type.hpp>
	
	template <>
	class AttributeAdapter<ov::element::Type>: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1ab8f3a7c601f124ebf96f7a2408335d9b>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a40fc93fb31a44d9d603f13d543d10c23>`(:ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a079fa98f944740c2bc0d147b80c31945>`("AttributeAdapter<:ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`>");
		virtual const std::string& :ref:`get<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a607731d2a7b8030613bc3d07ad9088ba>`();
		virtual void :ref:`set<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a4640ca78e7b8eeefa98e9d2a98c46873>`(const std::string& value);
		:target:`operator ov::element::Type &<doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a02cfd18963c5858d096de7d316bfdfba>` ();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a607731d2a7b8030613bc3d07ad9088ba:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& get()

Returns the value.

.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_01_4_1a4640ca78e7b8eeefa98e9d2a98c46873:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const std::string& value)

Sets the value.


.. index:: pair: class; ov::AttributeAdapter<op::v8::MatrixNms::DecayFunction>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v8_1_1_matrix_nms_1_1_decay_function_01_4:

class ov::AttributeAdapter<op::v8::MatrixNms::DecayFunction>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <matrix_nms.hpp>
	
	template <>
	class AttributeAdapter<op::v8::MatrixNms::DecayFunction>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v8_1_1_matrix_nms_1_1_decay_function_01_4_1af8d08887987759f8628aa51a7f0f027b>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v8_1_1_matrix_nms_1_1_decay_function_01_4_1a1213189da2367bad85771f295fa06c87>`(:ref:`op::v8::MatrixNms::DecayFunction<doxid-classov_1_1op_1_1v8_1_1_matrix_nms_1a152a686a5c925bf06d99743101a1a01b>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v8_1_1_matrix_nms_1_1_decay_function_01_4_1ab86d4161f3deffb52cab38a018f07c67>`("AttributeAdapter<:ref:`ov::op::v8::MatrixNms::DecayFunction<doxid-classov_1_1op_1_1v8_1_1_matrix_nms_1a152a686a5c925bf06d99743101a1a01b>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v5::Round::RoundMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_round_1_1_round_mode_01_4:

class ov::AttributeAdapter<op::v5::Round::RoundMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <round.hpp>
	
	template <>
	class AttributeAdapter<op::v5::Round::RoundMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_round_1_1_round_mode_01_4_1a212fb58f64279032c8de80cf199728f0>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_round_1_1_round_mode_01_4_1ab0033eaaf5b179655e3557ed4761a0c6>`(:ref:`op::v5::Round::RoundMode<doxid-classov_1_1op_1_1v5_1_1_round_1a25a2039a1e12e5aa8e612cb5bb82af7e>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_round_1_1_round_mode_01_4_1a09f6899ef02f76da8e490e31e77241d8>`("AttributeAdapter<:ref:`ov::op::v5::Round::RoundMode<doxid-classov_1_1op_1_1v5_1_1_round_1a25a2039a1e12e5aa8e612cb5bb82af7e>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v5::NonMaxSuppression::BoxEncodingType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_non_max_suppression_1_1_box_encoding_type_01_4:

class ov::AttributeAdapter<op::v5::NonMaxSuppression::BoxEncodingType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <non_max_suppression.hpp>
	
	template <>
	class AttributeAdapter<op::v5::NonMaxSuppression::BoxEncodingType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1a1a9173e0370a95451d450bfdee4a1a35>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1a347312e746f806f248f814f42ce6feeb>`(:ref:`op::v5::NonMaxSuppression::BoxEncodingType<doxid-classov_1_1op_1_1v5_1_1_non_max_suppression_1afad3db6910a6abd2b19d1db0fd8cb693>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1adacbd99dbd7b0d750b0e2de0d21cd63b>`("AttributeAdapter<ov::v5::NonMaxSuppression::BoxEncodingType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<std::shared_ptr<op::util::Variable>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_variable_01_4_01_4:

class ov::AttributeAdapter<std::shared_ptr<op::util::Variable>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable.hpp>
	
	template <>
	class AttributeAdapter<std::shared_ptr<op::util::Variable>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_variable_01_4_01_4_1af1dfba91bd468d52c59a3055e44318fb>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_variable_01_4_01_4_1a890c640009b5fe95ea48a122d361c819>`(std::shared_ptr<:ref:`op::util::Variable<doxid-classov_1_1op_1_1util_1_1_variable>`>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_variable_01_4_01_4_1a90c169bf49df5c2d8a7f8d7aa2df5ff3>`("AttributeAdapter<std::shared_ptr<:ref:`ov::op::util::Variable<doxid-classov_1_1op_1_1util_1_1_variable>`>>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<op::v9::ROIAlign::AlignedMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_aligned_mode_01_4:

class ov::AttributeAdapter<op::v9::ROIAlign::AlignedMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <roi_align.hpp>
	
	template <>
	class AttributeAdapter<op::v9::ROIAlign::AlignedMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_aligned_mode_01_4_1a74592b3662aa5cdfe96c80f66e719163>`(:ref:`op::v9::ROIAlign::AlignedMode<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1a647f0c34a0cbfe186bb2570dcbdb7d29>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_aligned_mode_01_4_1a94957117219cf0b8f12dfbcb3f62b478>`("AttributeAdapter<:ref:`ov::op::v9::ROIAlign::AlignedMode<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1a647f0c34a0cbfe186bb2570dcbdb7d29>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<ov::AxisSet>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4:

class ov::AttributeAdapter<ov::AxisSet>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <axis_set.hpp>
	
	template <>
	class AttributeAdapter<ov::AxisSet>: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1aa6dbf399f6526b6cee86355793ed928f>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a2d0fb862c79cb2e5f4d984fdc5d61338>`(:ref:`ov::AxisSet<doxid-classov_1_1_axis_set>`& value);

		// methods
	
		virtual const std::vector<int64_t>& :ref:`get<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a704ce082a0b423f418963d4694111466>`();
		virtual void :ref:`set<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a34f8432a5ae9a37fe87b6de46e22baf0>`(const std::vector<int64_t>& value);
		:target:`operator ov::AxisSet &<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a30ff724a50db0f63c3c873b13472c5e3>` ();
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a686e5530d8ea38b1a383a98d2272a1f5>`("AttributeAdapter<:ref:`AxisSet<doxid-classov_1_1_axis_set>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a704ce082a0b423f418963d4694111466:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::vector<int64_t>& get()

Returns the value.

.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_axis_set_01_4_1a34f8432a5ae9a37fe87b6de46e22baf0:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const std::vector<int64_t>& value)

Sets the value.


.. index:: pair: class; ov::AttributeAdapter<op::v9::ROIAlign::PoolingMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_pooling_mode_01_4:

class ov::AttributeAdapter<op::v9::ROIAlign::PoolingMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <roi_align.hpp>
	
	template <>
	class AttributeAdapter<op::v9::ROIAlign::PoolingMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_pooling_mode_01_4_1a9891ded0851e965b51e4ad01801efecc>`(:ref:`op::v9::ROIAlign::PoolingMode<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1aa6d46dab33d253ef2943e7cc6c68031a>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v9_1_1_r_o_i_align_1_1_pooling_mode_01_4_1a4faf2ba508a4b13cf4a89dd54417a411>`("AttributeAdapter<:ref:`ov::op::v9::ROIAlign::PoolingMode<doxid-classov_1_1op_1_1v9_1_1_r_o_i_align_1aa6d46dab33d253ef2943e7cc6c68031a>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<ov::Dimension>
.. _doxid-classov_1_1_attribute_adapter_3_01ov_1_1_dimension_01_4:

class ov::AttributeAdapter<ov::Dimension>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <dimension.hpp>
	
	template <>
	class AttributeAdapter<ov::Dimension>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_dimension_01_4_1a22faa875542da7d00451831a010fc74a>`(:ref:`ov::Dimension<doxid-classov_1_1_dimension>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ov_1_1_dimension_01_4_1aa1244511b14efe4bbe3c8b142bbe4aec>`("AttributeAdapter<:ref:`ov::Dimension<doxid-classov_1_1_dimension>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::shared_ptr<ov::Model>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_model_01_4_01_4:

class ov::AttributeAdapter<std::shared_ptr<ov::Model>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <model.hpp>
	
	template <>
	class AttributeAdapter<std::shared_ptr<ov::Model>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_model_01_4_01_4_1a3607b06322435d60e3739b8fdf0c6929>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_model_01_4_01_4_1aeaeb695f247f839ca12dbaf247c7dd0c>`(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_model_01_4_01_4_1a4b666a7b3a90b7f7221a5085ee3ec897>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::shared_ptr<ov::Node>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_node_01_4_01_4:

class ov::AttributeAdapter<std::shared_ptr<ov::Node>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Visits a reference to a node that has been registered with the visitor.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node.hpp>
	
	template <>
	class AttributeAdapter<std::shared_ptr<ov::Node>>: public :ref:`ov::VisitorAdapter<doxid-classov_1_1_visitor_adapter>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_node_01_4_01_4_1af06f60e29be38d3dd87e1e227fc9908c>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_node_01_4_01_4_1af044f01625498e43249216d188d12b1a>`(std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`>& value);

		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_node_01_4_01_4_1a99cecd31e4d5f8567263b7d682632339>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_node_01_4_01_4_1abb1b636727ce3108b6f72bd280ee14b5>`("AttributeAdapter<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;


.. index:: pair: class; ov::AttributeAdapter<std::string>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1string_01_4:

class ov::AttributeAdapter<std::string>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a string as a string.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::string>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1string_01_4_1a6bc58c3d52b06897caa8734e0b48aff7>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1string_01_4_1aeefbf74a165d109fbce28950ced1ad21>`(std::string& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1string_01_4_1aa143e892da0f2a81999c75ded123b52e>`("AttributeAdapter<std::string>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<Strides>
.. _doxid-classov_1_1_attribute_adapter_3_01_strides_01_4:

class ov::AttributeAdapter<Strides>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <strides.hpp>
	
	template <>
	class AttributeAdapter<Strides>: public :ref:`ov::IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01_strides_01_4_1abfd40fab1a186f8fdb2ae08f448e4895>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_strides_01_4_1ad921668258c3a6de6675427ada862277>`(:ref:`Strides<doxid-classov_1_1_strides>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_strides_01_4_1a56a7d83a8b53dcf25222409a8decf9aa>`("AttributeAdapter<:ref:`Strides<doxid-classov_1_1_strides>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_vector_value_accessor_1a92bfd6646dbb5351205f6ad3d9e11b3a>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		:ref:`operator AT &<doxid-classov_1_1_indirect_vector_value_accessor_1ad197d00c5756ba246f2a391d8d22aa02>` ();


.. index:: pair: class; ov::AttributeAdapter<std::vector<uint8_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint8__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<uint8_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<uint8_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<uint8_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint8__t_01_4_01_4_1aa2424381f94613f2d4ac5e0dc8038273>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint8__t_01_4_01_4_1aeafc5f15e7b643876fb53a880b8fb467>`(std::vector<uint8_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint8__t_01_4_01_4_1a1550657857a88765d56a91943ca142bc>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<uint64_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint64__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<uint64_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<uint64_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<uint64_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint64__t_01_4_01_4_1aa98a9850ff52421546b27d7606ea8db3>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint64__t_01_4_01_4_1a9435d56ed423a465f9fdca2019fc0988>`(std::vector<uint64_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint64__t_01_4_01_4_1a47bca221eb0b8ce04afd06a242522944>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<uint32_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint32__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<uint32_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<uint32_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<uint32_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint32__t_01_4_01_4_1a3edc5ccd6c42a30354387449406a9efa>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint32__t_01_4_01_4_1a8c373b13a721ef9a74ab72b5df06b039>`(std::vector<uint32_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint32__t_01_4_01_4_1ae9a47f24d73c6184f3f0d36ef0a35395>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<uint16_t>
.. _doxid-classov_1_1_attribute_adapter_3_01uint16__t_01_4:

class ov::AttributeAdapter<uint16_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a uint16_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<uint16_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01uint16__t_01_4_1a87ab70c125eb1c3f12785fe7f658b564>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01uint16__t_01_4_1a8733142a98e394862c826ee106180efe>`(uint16_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01uint16__t_01_4_1ab62646e008298cbe66d1327ead779011>`("AttributeAdapter<uint16_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<uint64_t>
.. _doxid-classov_1_1_attribute_adapter_3_01uint64__t_01_4:

class ov::AttributeAdapter<uint64_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a uint64_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<uint64_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01uint64__t_01_4_1a6d04c92fd067406885a3ea191f573fab>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01uint64__t_01_4_1a01cb26d90646e77950c664fd1c7553b5>`(uint64_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01uint64__t_01_4_1acae18d88bbb3268b94f1a7243f538bdf>`("AttributeAdapter<uint64_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<uint32_t>
.. _doxid-classov_1_1_attribute_adapter_3_01uint32__t_01_4:

class ov::AttributeAdapter<uint32_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a uint32_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<uint32_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01uint32__t_01_4_1ac2b9ef34c22b72100c7c2f9e622bea85>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01uint32__t_01_4_1afca717756621ee8468cf4c39d859cfd2>`(uint32_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01uint32__t_01_4_1a211cd81efc55f26d9a5e058b8ef94e83>`("AttributeAdapter<uint32_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<uint8_t>
.. _doxid-classov_1_1_attribute_adapter_3_01uint8__t_01_4:

class ov::AttributeAdapter<uint8_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a uint8_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<uint8_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01uint8__t_01_4_1a30edcee1b591043a7788211e4060a7bc>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01uint8__t_01_4_1aaa2e161492d3d1f4e20db0966dcd9ddb>`(uint8_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01uint8__t_01_4_1a4c834c737f63e0221df1541acc81e55f>`("AttributeAdapter<uint8_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v5::Loop::SpecialBodyPorts>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_loop_1_1_special_body_ports_01_4:

class ov::AttributeAdapter<op::v5::Loop::SpecialBodyPorts>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <loop.hpp>
	
	template <>
	class AttributeAdapter<op::v5::Loop::SpecialBodyPorts>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_loop_1_1_special_body_ports_01_4_1a512a97f9c164794ca0511a8babe57843>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_loop_1_1_special_body_ports_01_4_1a5fba65136ea036dd83d4966969a52772>`(:ref:`op::v5::Loop::SpecialBodyPorts<doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_loop_1_1_special_body_ports_01_4_1a21781d4bd03638cd7a54b5c50889e6e3>`("AttributeAdapter<:ref:`ov::op::v5::Loop::SpecialBodyPorts<doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<uint16_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint16__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<uint16_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<uint16_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<uint16_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint16__t_01_4_01_4_1adbd33e78cdde2c6c236550e10362518b>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint16__t_01_4_01_4_1a401ee164803b9c6a432c7efa7a59d1c6>`(std::vector<uint16_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint16__t_01_4_01_4_1a2d470ebd0cfda2c590c8bd39e6b63c54>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::OutputDescription>>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_6f33950209287517a71efbff21746b54:

class ov::AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::OutputDescription>>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	template <>
	class AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::OutputDescription>>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_6f33950209287517a71efbff21746b54_1a0ee3c3dcb9b640fe11dc7f9aba8da0df>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_6f33950209287517a71efbff21746b54_1a25770b4cd254cbd7d163f985762e694c>`(std::vector<std::shared_ptr<:ref:`op::util::MultiSubGraphOp::OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`>>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_6f33950209287517a71efbff21746b54_1add0a8be5b0df41744d6c567fd4c437c8>`("AttributeAdapter<std::vector<std::shared_ptr<:ref:`ov::op::util::MultiSubGraphOp::OutputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_output_description>`>>>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<float>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01float_01_4_01_4:

class ov::AttributeAdapter<std::vector<float>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<float>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<float>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01float_01_4_01_4_1aebc4b6e18daba55625a6b4ef46c0cca4>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01float_01_4_01_4_1aa7a6bf7e710baebbe38b5506c786c87c>`(std::vector<float>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01float_01_4_01_4_1ac9c17cc214cb4e03eb823a2f53975257>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<double>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01double_01_4_01_4:

class ov::AttributeAdapter<std::vector<double>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<double>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<double>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01double_01_4_01_4_1a3e6e16d71e1a0ef0d0dd1c329509298f>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01double_01_4_01_4_1af9ab865d989e6478646f8d0f290e305f>`(std::vector<double>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01double_01_4_01_4_1a7d2c4065ed5489bdfea23ee8b9a3a9e5>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<std::string>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1string_01_4_01_4:

class ov::AttributeAdapter<std::vector<std::string>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<string>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<std::string>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1string_01_4_01_4_1ae29857a6bbcbdde18216d3f0e4db7df0>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1string_01_4_01_4_1ac8e6400aeebc2be0a65739d4bec6ec93>`(std::vector<std::string>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1string_01_4_01_4_1a10f869f4fbacbb780b83a73079c4c273>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<int16_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int16__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<int16_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<int16_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<int16_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int16__t_01_4_01_4_1ab68592cd6b4db1b2229a1cbceab32455>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int16__t_01_4_01_4_1a64fa1e799914879a26438c496710109c>`(std::vector<int16_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int16__t_01_4_01_4_1ac11b8e346e970ca1fcc9a5b1559060f8>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<int64_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int64__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<int64_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<int64_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<int64_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int64__t_01_4_01_4_1a8fcf48ce83257d3948ab489852fee1af>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int64__t_01_4_01_4_1a92284d801d47d10b1baf25ce1513e3dd>`(std::vector<int64_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int64__t_01_4_01_4_1aa5b4ae7550269f7738f44a33076d384e>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<int32_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int32__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<int32_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a vector<int32_t>


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<int32_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int32__t_01_4_01_4_1afa37fd068285f9c0ca82395371a77024>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int32__t_01_4_01_4_1a25c0de569e8848c1399650e64c560e57>`(std::vector<int32_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int32__t_01_4_01_4_1a23b31baea699471086cc3f677edb1e6a>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::InputDescription>>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_166f0f1a593b5eb051c4008d21b4c2bf:

class ov::AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::InputDescription>>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <multi_subgraph_base.hpp>
	
	template <>
	class AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::InputDescription>>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_166f0f1a593b5eb051c4008d21b4c2bf_1afb9913eb8918bdeb4bf852fcf01cf36e>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_166f0f1a593b5eb051c4008d21b4c2bf_1a11b0b8fa92465f77ea48b787da374676>`(std::vector<std::shared_ptr<:ref:`op::util::MultiSubGraphOp::InputDescription<doxid-classov_1_1op_1_1util_1_1_multi_sub_graph_op_1_1_input_description>`>>& value);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<op::v4::Interpolate::ShapeCalcMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_shape_calc_mode_01_4:

class ov::AttributeAdapter<op::v4::Interpolate::ShapeCalcMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	template <>
	class AttributeAdapter<op::v4::Interpolate::ShapeCalcMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_shape_calc_mode_01_4_1ab53a90f7fc796bdb972874914681e9b3>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_shape_calc_mode_01_4_1a5700df8d5e2bce2ada18b9fe69fd7e37>`(:ref:`op::v4::Interpolate::ShapeCalcMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_shape_calc_mode_01_4_1a914628e82dc29043d29de42f732a4d78>`("AttributeAdapter<:ref:`ov::op::v4::Interpolate::ShapeCalcMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aeea9e299094216009ca1d3e18c029faa>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<std::vector<int8_t>>
.. _doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4:

class ov::AttributeAdapter<std::vector<int8_t>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

Access a vector<int8_t> :ref:`More...<details-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<std::vector<int8_t>>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4_1a670298bfbb42aef877032a540065b973>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4_1a28931b25335e023a31b24bca3cc1c0ea>`(std::vector<int8_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4_1a6e22192621a010967cfce2ad3bdbe1ab>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);

.. _details-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Access a vector<int8_t>

Note: These class bodies cannot be defined with templates because of interactions between dllexport and templates on Windows.


.. index:: pair: class; ov::AttributeAdapter<op::v4::Interpolate::InterpolateMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_interpolate_mode_01_4:

class ov::AttributeAdapter<op::v4::Interpolate::InterpolateMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	template <>
	class AttributeAdapter<op::v4::Interpolate::InterpolateMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_interpolate_mode_01_4_1a7fb9efd496459c75c29f29855a714f19>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_interpolate_mode_01_4_1a2bc7f0319558d89006d67077a3d319b9>`(:ref:`op::v4::Interpolate::InterpolateMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1a567d8870044804dc59d6d6e3df290da7>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_interpolate_mode_01_4_1af2d60c27bbd9160b12dc1b37d8b73fb9>`("AttributeAdapter<:ref:`ov::op::v4::Interpolate::InterpolateMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1a567d8870044804dc59d6d6e3df290da7>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v4::Interpolate::NearestMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_nearest_mode_01_4:

class ov::AttributeAdapter<op::v4::Interpolate::NearestMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	template <>
	class AttributeAdapter<op::v4::Interpolate::NearestMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_nearest_mode_01_4_1a35fb69f2dd45d5062412a782260b8f66>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_nearest_mode_01_4_1a552e1bdc127670a9a4f954453a83ffb3>`(:ref:`op::v4::Interpolate::NearestMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_nearest_mode_01_4_1a303845fc8a41808cbd315798ddfb7bfe>`("AttributeAdapter<:ref:`ov::op::v4::Interpolate::NearestMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1ad79e2d96abdf4d07b5d9f322372149c2>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<int8_t>
.. _doxid-classov_1_1_attribute_adapter_3_01int8__t_01_4:

class ov::AttributeAdapter<int8_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access an int8_t and an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<int8_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01int8__t_01_4_1a1ee891f0fce5c5ec0d83f8172c096cc8>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01int8__t_01_4_1aed280ba9febb2bc780bb7e6995424622>`(int8_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01int8__t_01_4_1acbd223be66a7fda1e235e4c23772769c>`("AttributeAdapter<int8_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<int64_t>
.. _doxid-classov_1_1_attribute_adapter_3_01int64__t_01_4:

class ov::AttributeAdapter<int64_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access an int64_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<int64_t>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01int64__t_01_4_1a2edc5f4e7a8074cb979c94a8e3600802>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01int64__t_01_4_1ae831b070599bee3d78ff2a505425343c>`(int64_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01int64__t_01_4_1ab03cc75dbbd0d4f7c028aed0d761fc00>`("AttributeAdapter<int64_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<int32_t>
.. _doxid-classov_1_1_attribute_adapter_3_01int32__t_01_4:

class ov::AttributeAdapter<int32_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access an int32_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<int32_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01int32__t_01_4_1a9d52e6d2402795646f9e06ead047f289>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01int32__t_01_4_1ab2da3c5ecd05193c1b1ef7190db8a14b>`(int32_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01int32__t_01_4_1a3e97c464c94d5b2a89389f62f09ece95>`("AttributeAdapter<int32_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<Layout>
.. _doxid-classov_1_1_attribute_adapter_3_01_layout_01_4:

class ov::AttributeAdapter<Layout>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layout.hpp>
	
	template <>
	class AttributeAdapter<Layout>: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1a4593a53029d295e19c118cb4c3cb86fe>`(:ref:`Layout<doxid-classov_1_1_layout>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1a2000ff0fa9e32b1f9e798ab356d44f18>`("AttributeAdapter<:ref:`Layout<doxid-classov_1_1_layout>`>");
		virtual const std::string& :ref:`get<doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1a997aa10e7ee88dccfcbfb44f8ecbffa6>`();
		virtual void :ref:`set<doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1a8c40667eddeb4500bcd7e94fd176dec0>`(const std::string& value);
		:target:`operator Layout &<doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1af4116be634d23b31be8613d127b1b777>` ();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_attribute_adapter_3_01_layout_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1a997aa10e7ee88dccfcbfb44f8ecbffa6:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& get()

Returns the value.

.. _doxid-classov_1_1_attribute_adapter_3_01_layout_01_4_1a8c40667eddeb4500bcd7e94fd176dec0:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const std::string& value)

Sets the value.


.. index:: pair: class; ov::AttributeAdapter<op::AutoBroadcastSpec>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_spec_01_4:

class ov::AttributeAdapter<op::AutoBroadcastSpec>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::AutoBroadcastSpec>: public :ref:`ov::VisitorAdapter<doxid-classov_1_1_visitor_adapter>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_spec_01_4_1aa0bac5deab43c705e708db8b221d6953>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_spec_01_4_1ad2cc2d690f38a63ee26112a58b9d2e89>`(:ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& value);

		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_spec_01_4_1af3d93e19f0fb08500fd607408776e106>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_spec_01_4_1ae49772c4d484a971a51c4c9e4f2a7692>`("AttributeAdapter<AutoBroadcastSpec>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;


.. index:: pair: class; ov::AttributeAdapter<ngraph::reduction::Type>
.. _doxid-classov_1_1_attribute_adapter_3_01ngraph_1_1reduction_1_1_type_01_4:

class ov::AttributeAdapter<ngraph::reduction::Type>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <distributed.hpp>
	
	template <>
	class AttributeAdapter<ngraph::reduction::Type>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01ngraph_1_1reduction_1_1_type_01_4_1a3149bf001f63256789dd5781397b5434>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01ngraph_1_1reduction_1_1_type_01_4_1acec23515f3ef11a31582fc6065d7780c>`(:ref:`ngraph::reduction::Type<doxid-namespacengraph_1_1reduction_1a3816ea23de325e23ec7cb516b25f1e70>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01ngraph_1_1reduction_1_1_type_01_4_1a79875c826f97621e61ae54340bfe6f88>`("AttributeAdapter<reduction::Type>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::BroadcastModeSpec>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_mode_spec_01_4:

class ov::AttributeAdapter<op::BroadcastModeSpec>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::BroadcastModeSpec>: public :ref:`ov::VisitorAdapter<doxid-classov_1_1_visitor_adapter>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_mode_spec_01_4_1a529edad3689087c6652c4f7219846f5e>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_mode_spec_01_4_1af42c9251161a485666f2ed3aa4d3e312>`(:ref:`op::BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec>`& value);

		// methods
	
		virtual bool :target:`visit_attributes<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_mode_spec_01_4_1a702212e3014fe79243688e6fffded712>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_mode_spec_01_4_1a49c0c0fb1e2113c34f9b9279ab967e5f>`("AttributeAdapter<BroadcastModeSpec>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_visitor_adapter_1afdc2175bfdefa22f6aff9ba4b05657b9>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) = 0;


.. index:: pair: class; ov::AttributeAdapter<op::BroadcastType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_type_01_4:

class ov::AttributeAdapter<op::BroadcastType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::BroadcastType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_type_01_4_1a541789b71e6ca24cff60f24abcad4a48>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_type_01_4_1acd3c6d707fe65b91c7053057796bca6c>`(:ref:`op::BroadcastType<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_broadcast_type_01_4_1a0ff2395152acd9d2c063bf48ed878472>`("AttributeAdapter<BroadcastType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<int16_t>
.. _doxid-classov_1_1_attribute_adapter_3_01int16__t_01_4:

class ov::AttributeAdapter<int16_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access an int16_t as an int64_t.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<int16_t>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01int16__t_01_4_1ae781de35e3bf6418056c5f3cc544cf01>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01int16__t_01_4_1a9378e9ce2b3b606c4c0cfa319b495d8c>`(int16_t& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01int16__t_01_4_1a60a7960cf5159f177c794dcf518cdc76>`("AttributeAdapter<int16_t>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<ELTWISE_TYPE>
.. _doxid-classov_1_1_attribute_adapter_3_01_e_l_t_w_i_s_e___t_y_p_e_01_4:

class ov::AttributeAdapter<ELTWISE_TYPE>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <eltwise.hpp>
	
	template <>
	class AttributeAdapter<ELTWISE_TYPE>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		static constexpr :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :target:`type_info<doxid-classov_1_1_attribute_adapter_3_01_e_l_t_w_i_s_e___t_y_p_e_01_4_1ab12af3f910af3852541d0c6fa97a771b>` {"AttributeAdapter<:ref:`ELTWISE_TYPE<doxid-eltwise_8hpp_1aca2b664f1fd62f182b07693d53c56611>`>",                                               1};

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_e_l_t_w_i_s_e___t_y_p_e_01_4_1aca3db58153afe0de624d10bd067fc75e>`(:ref:`ELTWISE_TYPE<doxid-eltwise_8hpp_1aca2b664f1fd62f182b07693d53c56611>`& value);

		// methods
	
		const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info<doxid-classov_1_1_attribute_adapter_3_01_e_l_t_w_i_s_e___t_y_p_e_01_4_1ad9d94e7895df9e2352a5315fe33c332b>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<AxisVector>
.. _doxid-classov_1_1_attribute_adapter_3_01_axis_vector_01_4:

class ov::AttributeAdapter<AxisVector>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <axis_vector.hpp>
	
	template <>
	class AttributeAdapter<AxisVector>: public :ref:`ov::IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01_axis_vector_01_4_1a6d33efa7b66664cdd0a3c6185586875c>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_axis_vector_01_4_1a20d02ee212b6408c52c9d2bfd2ad0a6a>`(:ref:`AxisVector<doxid-classov_1_1_axis_vector>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_axis_vector_01_4_1acc3fd7e4df4d4fcd4596041fd2638aee>`("AttributeAdapter<:ref:`AxisVector<doxid-classov_1_1_axis_vector>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_vector_value_accessor_1a92bfd6646dbb5351205f6ad3d9e11b3a>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		:ref:`operator AT &<doxid-classov_1_1_indirect_vector_value_accessor_1ad197d00c5756ba246f2a391d8d22aa02>` ();


.. index:: pair: class; ov::AttributeAdapter
.. _doxid-classov_1_1_attribute_adapter:

class ov::AttributeAdapter
^^^^^^^^^^^^^^^^^^^^^^^^^^



An :ref:`AttributeAdapter <doxid-classov_1_1_attribute_adapter>` "captures" an attribute as an AT& and makes it available as a ValueAccessor<VAT>.


.. index:: pair: class; ov::AttributeAdapter<float>
.. _doxid-classov_1_1_attribute_adapter_3_01float_01_4:

class ov::AttributeAdapter<float>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<float>: public :ref:`ov::IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01float_01_4_1ad8b7db8c60c2de043b5f844126904f88>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01float_01_4_1a4ad7926e475cce87c7f7419b40445c97>`(float& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01float_01_4_1a8fc339e672573fde70a36b6d4ed0bf70>`("AttributeAdapter<float>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<bool>
.. _doxid-classov_1_1_attribute_adapter_3_01bool_01_4:

class ov::AttributeAdapter<bool>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a bool as a bool.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<bool>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01bool_01_4_1a17d1330e16038a3bcaf831d146dfe87e>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01bool_01_4_1a218928604352602578c8ef7da87c4d1e>`(bool& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01bool_01_4_1afc6f585af75c04da23940d80dd26bc5d>`("AttributeAdapter<bool>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<CoordinateDiff>
.. _doxid-classov_1_1_attribute_adapter_3_01_coordinate_diff_01_4:

class ov::AttributeAdapter<CoordinateDiff>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <coordinate_diff.hpp>
	
	template <>
	class AttributeAdapter<CoordinateDiff>: public :ref:`ov::IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01_coordinate_diff_01_4_1a06c67fe46a8d3bd1b8333fb75b59daed>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_coordinate_diff_01_4_1a188a9514c691957920477194f89d93d9>`(:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_coordinate_diff_01_4_1a0c5b18fa03dfc7951102c9932dff5a74>`("AttributeAdapter<:ref:`CoordinateDiff<doxid-classov_1_1_coordinate_diff>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_vector_value_accessor_1a92bfd6646dbb5351205f6ad3d9e11b3a>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		:ref:`operator AT &<doxid-classov_1_1_indirect_vector_value_accessor_1ad197d00c5756ba246f2a391d8d22aa02>` ();


.. index:: pair: class; ov::AttributeAdapter<Coordinate>
.. _doxid-classov_1_1_attribute_adapter_3_01_coordinate_01_4:

class ov::AttributeAdapter<Coordinate>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <coordinate.hpp>
	
	template <>
	class AttributeAdapter<Coordinate>: public :ref:`ov::IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01_coordinate_01_4_1a9916cc75bdaa151db2b570da4d1f8a5f>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01_coordinate_01_4_1a2d1dd044625bb5df03c5c7694640e2d1>`(:ref:`Coordinate<doxid-classov_1_1_coordinate>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01_coordinate_01_4_1a19f15b5a5cdff7348151b5a46943d7e8>`("AttributeAdapter<:ref:`Coordinate<doxid-classov_1_1_coordinate>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4>`(const VAT& value);
		void :ref:`set_as_any<doxid-classov_1_1_indirect_vector_value_accessor_1a92bfd6646dbb5351205f6ad3d9e11b3a>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		:ref:`operator AT &<doxid-classov_1_1_indirect_vector_value_accessor_1ad197d00c5756ba246f2a391d8d22aa02>` ();


.. index:: pair: class; ov::AttributeAdapter<double>
.. _doxid-classov_1_1_attribute_adapter_3_01double_01_4:

class ov::AttributeAdapter<double>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Access a double as a double.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class AttributeAdapter<double>: public :ref:`ov::DirectValueAccessor<doxid-classov_1_1_direct_value_accessor>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01double_01_4_1a8130ec92534e06fe7741af8a375c2431>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01double_01_4_1adfdcd2802e796e549e57bafb357c4d5e>`(double& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01double_01_4_1a2c64cad1e01a9d8df53ecca7b7014598>`("AttributeAdapter<double>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);


.. index:: pair: class; ov::AttributeAdapter<op::EpsMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_eps_mode_01_4:

class ov::AttributeAdapter<op::EpsMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::EpsMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_eps_mode_01_4_1ac4d40ab58cf55ff26be8357d1cbb2032>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_eps_mode_01_4_1ac107378e74ed7e4bf36d4ee6c3f73d20>`(:ref:`op::EpsMode<doxid-namespaceov_1_1op_1abde68b9f95937807257f2be0a05165b3>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_eps_mode_01_4_1a9820ab91b0b08416367f273e8f3dddc3>`("AttributeAdapter<EpsMode>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::AutoBroadcastType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_type_01_4:

class ov::AttributeAdapter<op::AutoBroadcastType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::AutoBroadcastType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_type_01_4_1a5b95f313cd95f9c701a1a8cdf07e36e4>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_type_01_4_1a05667974e204585c51478fc7de75dca1>`(:ref:`op::AutoBroadcastType<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_auto_broadcast_type_01_4_1ad4b9c923df6e419ef473a991207ae23b>`("AttributeAdapter<AutoBroadcastType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::LSTMWeightsFormat>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_l_s_t_m_weights_format_01_4:

class ov::AttributeAdapter<op::LSTMWeightsFormat>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <lstm_cell.hpp>
	
	template <>
	class AttributeAdapter<op::LSTMWeightsFormat>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_l_s_t_m_weights_format_01_4_1a70c88ff04793e4cec4db356ecd488f22>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_l_s_t_m_weights_format_01_4_1a2260d5ef89a278748162c8b84968832d>`(:ref:`op::LSTMWeightsFormat<doxid-namespaceov_1_1op_1a6efe5db5f325a937a6662cd2b66e1437>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_l_s_t_m_weights_format_01_4_1a710c94aa8c4d173a3633305a32375601>`("AttributeAdapter<:ref:`ov::op::LSTMWeightsFormat<doxid-namespaceov_1_1op_1a6efe5db5f325a937a6662cd2b66e1437>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v1::NonMaxSuppression::BoxEncodingType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_non_max_suppression_1_1_box_encoding_type_01_4:

class ov::AttributeAdapter<op::v1::NonMaxSuppression::BoxEncodingType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <non_max_suppression.hpp>
	
	template <>
	class AttributeAdapter<op::v1::NonMaxSuppression::BoxEncodingType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1a73588c1595f99eb6d1d65765ba1dfb73>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1ac37f4faddcafc9e82500deba071ab719>`(:ref:`op::v1::NonMaxSuppression::BoxEncodingType<doxid-classov_1_1op_1_1v1_1_1_non_max_suppression_1a9a64fb28f8bc647fbd016619a5fbdda0>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1a332aae4248bb2fac15a32a6792964e06>`("AttributeAdapter<ov::v1::NonMaxSuppression::BoxEncodingType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::GeluApproximationMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_gelu_approximation_mode_01_4:

class ov::AttributeAdapter<op::GeluApproximationMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <gelu.hpp>
	
	template <>
	class AttributeAdapter<op::GeluApproximationMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_gelu_approximation_mode_01_4_1a8f360c07978ac5d6d594435e8909581b>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_gelu_approximation_mode_01_4_1aae1d0526fd1190aa044736b5533018f4>`(:ref:`op::GeluApproximationMode<doxid-namespaceov_1_1op_1a1ab40a6efb6720925e3d75890dd87d63>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_gelu_approximation_mode_01_4_1a86ad823631800ce9b0d68a325b031b13>`("AttributeAdapter<:ref:`ov::op::GeluApproximationMode<doxid-namespaceov_1_1op_1a1ab40a6efb6720925e3d75890dd87d63>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v0::SpaceToDepth::SpaceToDepthMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_space_to_depth_1_1_space_to_depth_mode_01_4:

class ov::AttributeAdapter<op::v0::SpaceToDepth::SpaceToDepthMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <space_to_depth.hpp>
	
	template <>
	class AttributeAdapter<op::v0::SpaceToDepth::SpaceToDepthMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_space_to_depth_1_1_space_to_depth_mode_01_4_1aa2ecfd9b053cc3c1b4f6f69048f5c5bd>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_space_to_depth_1_1_space_to_depth_mode_01_4_1ae18dc348899b571ef2e02189b5f5d3de>`(:ref:`op::v0::SpaceToDepth::SpaceToDepthMode<doxid-classov_1_1op_1_1v0_1_1_space_to_depth_1ad6b782e0cfede20e971e2ff658d80957>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_space_to_depth_1_1_space_to_depth_mode_01_4_1a800a24d37ff6dcb9a1b1d92a5bf6af08>`("AttributeAdapter<:ref:`ov::op::v0::SpaceToDepth::SpaceToDepthMode<doxid-classov_1_1op_1_1v0_1_1_space_to_depth_1ad6b782e0cfede20e971e2ff658d80957>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v0::Interpolate::InterpolateMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_interpolate_1_1_interpolate_mode_01_4:

class ov::AttributeAdapter<op::v0::Interpolate::InterpolateMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	template <>
	class AttributeAdapter<op::v0::Interpolate::InterpolateMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_interpolate_1_1_interpolate_mode_01_4_1ab36d28598e4be21ed6692865c5a495cf>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_interpolate_1_1_interpolate_mode_01_4_1a99d666a0b37de706797fbd610488bf6c>`(:ref:`op::v0::Interpolate::InterpolateMode<doxid-classov_1_1op_1_1v0_1_1_interpolate_1ae6b119b345a7d6cf0e249c5390535581>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_interpolate_1_1_interpolate_mode_01_4_1a6a7f3f17b84541030e6590a297c53fd8>`("AttributeAdapter<:ref:`ov::op::v0::Interpolate::InterpolateMode<doxid-classov_1_1op_1_1v0_1_1_interpolate_1ae6b119b345a7d6cf0e249c5390535581>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v1::Reverse::Mode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_reverse_1_1_mode_01_4:

class ov::AttributeAdapter<op::v1::Reverse::Mode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <reverse.hpp>
	
	template <>
	class AttributeAdapter<op::v1::Reverse::Mode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_reverse_1_1_mode_01_4_1a2425d706a53942a06405c958189289b6>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_reverse_1_1_mode_01_4_1a258737fcd9d92267b51bcd34f7aa0e37>`(:ref:`op::v1::Reverse::Mode<doxid-classov_1_1op_1_1v1_1_1_reverse_1ad4489cd12a59c950fe16f88ccd88a4f6>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_reverse_1_1_mode_01_4_1ae57628f581f4e4765f5fd171c1fc50ae>`("AttributeAdapter<:ref:`ov::op::v1::Reverse::Mode<doxid-classov_1_1op_1_1v1_1_1_reverse_1ad4489cd12a59c950fe16f88ccd88a4f6>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v3::ROIAlign::PoolingMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_r_o_i_align_1_1_pooling_mode_01_4:

class ov::AttributeAdapter<op::v3::ROIAlign::PoolingMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <roi_align.hpp>
	
	template <>
	class AttributeAdapter<op::v3::ROIAlign::PoolingMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_r_o_i_align_1_1_pooling_mode_01_4_1ac516818f963ba4bbb38e09b749a88d30>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_r_o_i_align_1_1_pooling_mode_01_4_1af3cec2b7558db87df10eb152d2d86060>`(:ref:`op::v3::ROIAlign::PoolingMode<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align_1a7ef654649e9fe953a81a3cf7a30c85d7>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_r_o_i_align_1_1_pooling_mode_01_4_1a794b2f888fd31a5767f47d9c47a3ac16>`("AttributeAdapter<:ref:`ov::op::v3::ROIAlign::PoolingMode<doxid-classov_1_1op_1_1v3_1_1_r_o_i_align_1a7ef654649e9fe953a81a3cf7a30c85d7>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v3::NonMaxSuppression::BoxEncodingType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_non_max_suppression_1_1_box_encoding_type_01_4:

class ov::AttributeAdapter<op::v3::NonMaxSuppression::BoxEncodingType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <non_max_suppression.hpp>
	
	template <>
	class AttributeAdapter<op::v3::NonMaxSuppression::BoxEncodingType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1a27c55dfd9aa1c3d76b60cd0e6ee462b7>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1a86ed63ca656f7245a8421212f79dd918>`(:ref:`op::v3::NonMaxSuppression::BoxEncodingType<doxid-classov_1_1op_1_1v3_1_1_non_max_suppression_1afbb5f2cab744c997b97ca0e9968f002c>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v3_1_1_non_max_suppression_1_1_box_encoding_type_01_4_1ac798c5a6c891801cbabe45fe021e14dc>`("AttributeAdapter<ov::v3::NonMaxSuppression::BoxEncodingType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v4::Interpolate::CoordinateTransformMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_coordinate_transform_mode_01_4:

class ov::AttributeAdapter<op::v4::Interpolate::CoordinateTransformMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	template <>
	class AttributeAdapter<op::v4::Interpolate::CoordinateTransformMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_coordinate_transform_mode_01_4_1a6ed940e13631a50236e859649fbdc7cd>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_coordinate_transform_mode_01_4_1aa20660c0520307450307d186ca9153d1>`(:ref:`op::v4::Interpolate::CoordinateTransformMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v4_1_1_interpolate_1_1_coordinate_transform_mode_01_4_1a1ac3f9ade6525e3560309be5ceacccbc>`("AttributeAdapter<:ref:`ov::op::v4::Interpolate::CoordinateTransformMode<doxid-classov_1_1op_1_1v4_1_1_interpolate_1aa769e0059d897c8dc7187f8df8a753e5>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v0::DepthToSpace::DepthToSpaceMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_depth_to_space_1_1_depth_to_space_mode_01_4:

class ov::AttributeAdapter<op::v0::DepthToSpace::DepthToSpaceMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <depth_to_space.hpp>
	
	template <>
	class AttributeAdapter<op::v0::DepthToSpace::DepthToSpaceMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_depth_to_space_1_1_depth_to_space_mode_01_4_1aa8708f46b2a497c0c11fd4847c7b80db>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_depth_to_space_1_1_depth_to_space_mode_01_4_1ac790bdd63b735ca59a6deaec9f29a8f7>`(:ref:`op::v0::DepthToSpace::DepthToSpaceMode<doxid-classov_1_1op_1_1v0_1_1_depth_to_space_1adf46d7cb205c4a8b94bafa9d4c34c303>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v0_1_1_depth_to_space_1_1_depth_to_space_mode_01_4_1a0efcada29a20aae50a75892ce87d81f7>`("AttributeAdapter<:ref:`ov::op::v0::DepthToSpace::DepthToSpaceMode<doxid-classov_1_1op_1_1v0_1_1_depth_to_space_1adf46d7cb205c4a8b94bafa9d4c34c303>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::v1::BinaryConvolution::BinaryConvolutionMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_binary_convolution_1_1_binary_convolution_mode_01_4:

class ov::AttributeAdapter<op::v1::BinaryConvolution::BinaryConvolutionMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <binary_convolution.hpp>
	
	template <>
	class AttributeAdapter<op::v1::BinaryConvolution::BinaryConvolutionMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_binary_convolution_1_1_binary_convolution_mode_01_4_1ae7cfe7f739e9625fa897544a69a8f82e>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_binary_convolution_1_1_binary_convolution_mode_01_4_1a01d0b9f0755f23428007a40faccee4f8>`(:ref:`op::v1::BinaryConvolution::BinaryConvolutionMode<doxid-classov_1_1op_1_1v1_1_1_binary_convolution_1aff500c1508ca17c80cc8c7c503aa040f>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1v1_1_1_binary_convolution_1_1_binary_convolution_mode_01_4_1abd4a10da1716d9be83235ef1c5aa9b3c>`("AttributeAdapter<:ref:`ov::op::v1::BinaryConvolution::BinaryConvolutionMode<doxid-classov_1_1op_1_1v1_1_1_binary_convolution_1aff500c1508ca17c80cc8c7c503aa040f>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::TopKSortType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_sort_type_01_4:

class ov::AttributeAdapter<op::TopKSortType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::TopKSortType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_sort_type_01_4_1a711c7ca878dfad34683854bc235ca869>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_sort_type_01_4_1a8c55e695c9fde01c77043fec921c39eb>`(:ref:`op::TopKSortType<doxid-namespaceov_1_1op_1adb25710a58c013466ba8b371156e09cb>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_sort_type_01_4_1a75fc9feb130a7214bc312c471b312479>`("AttributeAdapter<TopKSortType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::PadMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_mode_01_4:

class ov::AttributeAdapter<op::PadMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::PadMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_mode_01_4_1af8649bf515ae318a0aec8ea6f26a3aa2>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_mode_01_4_1a3820e50479fad5e606212f001b027a7b>`(:ref:`op::PadMode<doxid-namespaceov_1_1op_1aff39ecf8a8a3110216bfe131cc8b9ae0>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_mode_01_4_1a806c33820eccce83f58161050b5c1703>`("AttributeAdapter<PadMode>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::util::NmsBase::SortResultType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1util_1_1_nms_base_1_1_sort_result_type_01_4:

class ov::AttributeAdapter<op::util::NmsBase::SortResultType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <nms_base.hpp>
	
	template <>
	class AttributeAdapter<op::util::NmsBase::SortResultType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1util_1_1_nms_base_1_1_sort_result_type_01_4_1a39f5c31cf342e90a42ecadebaaff3e9e>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1util_1_1_nms_base_1_1_sort_result_type_01_4_1a0cba9b8ce663a1906c153b47ae62b2e7>`(:ref:`op::util::NmsBase::SortResultType<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1util_1_1_nms_base_1_1_sort_result_type_01_4_1a1e638c1ac9f3ef75b89a5baa3bf7c7c0>`("AttributeAdapter<:ref:`ov::op::util::NmsBase::SortResultType<doxid-classov_1_1op_1_1util_1_1_nms_base_1a2bd5a4283198ccea241f81235c1b7bc2>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::PadType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_type_01_4:

class ov::AttributeAdapter<op::PadType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::PadType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_type_01_4_1a842c113f096fac69995faadca72e4dd1>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_type_01_4_1a2a16ac40ae9147389ac35b650eacd0e4>`(:ref:`op::PadType<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_pad_type_01_4_1a2267ced0da3bb4778b9f7903058da918>`("AttributeAdapter<PadType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::MVNEpsMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_m_v_n_eps_mode_01_4:

class ov::AttributeAdapter<op::MVNEpsMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <mvn.hpp>
	
	template <>
	class AttributeAdapter<op::MVNEpsMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_m_v_n_eps_mode_01_4_1ad6115359f00dd8f8f2a29d931bd06ba3>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_m_v_n_eps_mode_01_4_1aec4a36a5aa27b9accb13ba22675ae782>`(:ref:`op::MVNEpsMode<doxid-namespaceov_1_1op_1a2fa6abf51a614b1b7f65f6bcafa88d99>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_m_v_n_eps_mode_01_4_1aade662f833e2122b73f9682f47f3d6c0>`("AttributeAdapter<:ref:`ov::op::MVNEpsMode<doxid-namespaceov_1_1op_1a2fa6abf51a614b1b7f65f6bcafa88d99>`>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::RoundingType>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_rounding_type_01_4:

class ov::AttributeAdapter<op::RoundingType>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::RoundingType>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_rounding_type_01_4_1a87ce029d5947fd642377d7339f9c40f0>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_rounding_type_01_4_1aaba7835e453bf0dae36dadf8affd0498>`(:ref:`op::RoundingType<doxid-namespaceov_1_1op_1a3f5ee36f633920020e774d506a8ffba6>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_rounding_type_01_4_1a8cbb7411858ad264a88b223fab87dea9>`("AttributeAdapter<RoundingType>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::RecurrentSequenceDirection>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_recurrent_sequence_direction_01_4:

class ov::AttributeAdapter<op::RecurrentSequenceDirection>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::RecurrentSequenceDirection>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_recurrent_sequence_direction_01_4_1a5508f1e60883c8c744caeb351bbd635a>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_recurrent_sequence_direction_01_4_1a0c5e7abf09ad1280a6e510170955f7ed>`(:ref:`op::RecurrentSequenceDirection<doxid-namespaceov_1_1op_1a9ea79d465e912e768d0ac8fe24d6f0cc>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_recurrent_sequence_direction_01_4_1abdf341478736053c070915fd5f4bbd55>`("AttributeAdapter<RecurrentSequenceDirection>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::AttributeAdapter<op::TopKMode>
.. _doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_mode_01_4:

class ov::AttributeAdapter<op::TopKMode>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	template <>
	class AttributeAdapter<op::TopKMode>: public :ref:`ov::EnumAttributeAdapterBase<doxid-classov_1_1_enum_attribute_adapter_base>`
	{
	public:
		// fields
	
		 :target:`BWDCMP_RTTI_DECLARATION<doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_mode_01_4_1a4efb08d2e4e7255419b6c6cfd92ed57a>`;

		// construction
	
		:target:`AttributeAdapter<doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_mode_01_4_1ab247127dd134753229cde143fe3a421f>`(:ref:`op::TopKMode<doxid-namespaceov_1_1op_1a1b4a5e596b7b28cc8a8746fda9ee1a97>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_attribute_adapter_3_01op_1_1_top_k_mode_01_4_1a6ffcdc1608436efdf7bfeb278af836c7>`("AttributeAdapter<TopKMode>");
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		virtual const std::string& :ref:`get<doxid-classov_1_1_enum_attribute_adapter_base_1ad156e70966e405251a9326421ad05454>`();
		virtual void :ref:`set<doxid-classov_1_1_enum_attribute_adapter_base_1ad66afbf25647a99e45c17ede06b5344b>`(const std::string& value);
		:ref:`operator AT &<doxid-classov_1_1_enum_attribute_adapter_base_1a4ebdea06afe3fa3f7896b85e73df6414>` ();
		void :ref:`set_as_any<doxid-classov_1_1_enum_attribute_adapter_base_1ac9744b565e64f6849235d95798efa15c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


