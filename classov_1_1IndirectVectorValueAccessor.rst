.. index:: pair: class; ov::IndirectVectorValueAccessor
.. _doxid-classov_1_1_indirect_vector_value_accessor:

class ov::IndirectVectorValueAccessor
=====================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <typename AT, typename VAT>
	class IndirectVectorValueAccessor: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// construction
	
		:target:`IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor_1ab5a42eab18f20dff888f284fc1a507ee>`(AT& ref);

		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4>`(const VAT& value);
		void :target:`set_as_any<doxid-classov_1_1_indirect_vector_value_accessor_1a92bfd6646dbb5351205f6ad3d9e11b3a>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
		:target:`operator AT &<doxid-classov_1_1_indirect_vector_value_accessor_1ad197d00c5756ba246f2a391d8d22aa02>` ();
	};

	// direct descendants

	template <>
	class :ref:`AttributeAdapter<AxisVector><doxid-classov_1_1_attribute_adapter_3_01_axis_vector_01_4>`;

	template <>
	class :ref:`AttributeAdapter<Coordinate><doxid-classov_1_1_attribute_adapter_3_01_coordinate_01_4>`;

	template <>
	class :ref:`AttributeAdapter<CoordinateDiff><doxid-classov_1_1_attribute_adapter_3_01_coordinate_diff_01_4>`;

	template <>
	class :ref:`AttributeAdapter<ov::Shape><doxid-classov_1_1_attribute_adapter_3_01ov_1_1_shape_01_4>`;

	template <>
	class :ref:`AttributeAdapter<Strides><doxid-classov_1_1_attribute_adapter_3_01_strides_01_4>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_indirect_vector_value_accessor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1_indirect_vector_value_accessor_1aca78a12c9c6ef053a873b3067576d3cd:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const VAT& get()

Returns the value.

.. _doxid-classov_1_1_indirect_vector_value_accessor_1adafe956d7745655dfc8423320cfa93c4:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const VAT& value)

Sets the value.


