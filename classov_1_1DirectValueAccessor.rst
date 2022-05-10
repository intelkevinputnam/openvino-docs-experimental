.. index:: pair: class; ov::DirectValueAccessor
.. _doxid-classov_1_1_direct_value_accessor:

class ov::DirectValueAccessor
=============================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <typename AT>
	class DirectValueAccessor: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// construction
	
		:target:`DirectValueAccessor<doxid-classov_1_1_direct_value_accessor_1adba763b7b792a53f75b86128cdc9d019>`(AT& ref);

		// methods
	
		virtual const AT& :ref:`get<doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa>`();
		virtual void :ref:`set<doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6>`(const AT& value);
	};

	// direct descendants

	template <>
	class :ref:`AttributeAdapter<bool><doxid-classov_1_1_attribute_adapter_3_01bool_01_4>`;

	template <>
	class :ref:`AttributeAdapter<double><doxid-classov_1_1_attribute_adapter_3_01double_01_4>`;

	template <>
	class :ref:`AttributeAdapter<int64_t><doxid-classov_1_1_attribute_adapter_3_01int64__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<op::v5::Loop::SpecialBodyPorts><doxid-classov_1_1_attribute_adapter_3_01op_1_1v5_1_1_loop_1_1_special_body_ports_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::Dimension><doxid-classov_1_1_attribute_adapter_3_01ov_1_1_dimension_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::element::TypeVector><doxid-classov_1_1_attribute_adapter_3_01ov_1_1element_1_1_type_vector_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::op::util::FrameworkNodeAttrs><doxid-classov_1_1_attribute_adapter_3_01ov_1_1op_1_1util_1_1_framework_node_attrs_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::PartialShape><doxid-classov_1_1_attribute_adapter_3_01ov_1_1_partial_shape_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::set<std::string>><doxid-classov_1_1_attribute_adapter_3_01std_1_1set_3_01std_1_1string_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::shared_ptr<ngraph::runtime::AlignedBuffer>><doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ngraph_1_1runtime_1_1_aligned_buffer_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::shared_ptr<op::util::Variable>><doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_variable_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::shared_ptr<ov::Model>><doxid-classov_1_1_attribute_adapter_3_01std_1_1shared__ptr_3_01ov_1_1_model_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::string><doxid-classov_1_1_attribute_adapter_3_01std_1_1string_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<double>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01double_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<float>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01float_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<int16_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int16__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<int32_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int32__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<int64_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int64__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<int8_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01int8__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::InputDescription>>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_166f0f1a593b5eb051c4008d21b4c2bf>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<std::shared_ptr<op::util::MultiSubGraphOp::OutputDescription>>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1shared__ptr_3_01op_1_1util_1_1_multi_6f33950209287517a71efbff21746b54>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<std::string>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01std_1_1string_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<uint16_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint16__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<uint32_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint32__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<uint64_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint64__t_01_4_01_4>`;

	template <>
	class :ref:`AttributeAdapter<std::vector<uint8_t>><doxid-classov_1_1_attribute_adapter_3_01std_1_1vector_3_01uint8__t_01_4_01_4>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_direct_value_accessor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1_direct_value_accessor_1aac4d30112eced447c497372895cf84fa:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const AT& get()

Returns the value.

.. _doxid-classov_1_1_direct_value_accessor_1abdf5a6e902f40491bbe199fc1fd3cda6:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const AT& value)

Sets the value.


