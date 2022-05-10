.. index:: pair: class; ov::ValueAccessor<void>
.. _doxid-classov_1_1_value_accessor_3_01void_01_4:

class ov::ValueAccessor<void>
=============================



Overview
~~~~~~~~

:ref:`ValueAccessor\<void> <doxid-classov_1_1_value_accessor_3_01void_01_4>` provides an accessor for values that do not have get/set methods via :ref:`AttributeVisitor.on_adapter <doxid-classov_1_1_attribute_visitor_1aa2db9dc01b6d21ec1644b40396e99e1b>`. :ref:`More...<details-classov_1_1_value_accessor_3_01void_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class ValueAccessor<void>
	{
	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :target:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
	};

	// direct descendants

	template <>
	class :ref:`ValueAccessor<void \*><doxid-classov_1_1_value_accessor_3_01void_01_5_01_4>`;

	class :ref:`VisitorAdapter<doxid-classov_1_1_visitor_adapter>`;
.. _details-classov_1_1_value_accessor_3_01void_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`ValueAccessor\<void> <doxid-classov_1_1_value_accessor_3_01void_01_4>` provides an accessor for values that do not have get/set methods via :ref:`AttributeVisitor.on_adapter <doxid-classov_1_1_attribute_visitor_1aa2db9dc01b6d21ec1644b40396e99e1b>`.

All ValueAccessors must be derived from :ref:`ValueAccessor\<void> <doxid-classov_1_1_value_accessor_3_01void_01_4>` so that an :ref:`AttributeVisitor <doxid-classov_1_1_attribute_visitor>` only needs to implement a subset of the on_adapter methods.

Methods
-------

.. _doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819:
.. index:: pair: function; get_type_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& get_type_info() const = 0

type info enables identification of the value accessor, as well as is_type and as_type.


.. index:: pair: class; ov::ValueAccessor<void \*>
.. _doxid-classov_1_1_value_accessor_3_01void_01_5_01_4:

class ov::ValueAccessor<void \*>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <>
	class ValueAccessor<void \*>: public :ref:`ov::ValueAccessor<void><doxid-classov_1_1_value_accessor_3_01void_01_4>`
	{
	public:
		// methods
	
		virtual void \* :target:`get_ptr<doxid-classov_1_1_value_accessor_3_01void_01_5_01_4_1a54fe16d869a124f33c0382ccb7f01580>`() = 0;
		virtual size_t :target:`size<doxid-classov_1_1_value_accessor_3_01void_01_5_01_4_1af4e0399efee0e34625f07a2de9ff7209>`() = 0;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_value_accessor_3_01void_01_4_1a4b0ebdf722f5f94e7a7347297c03e819>`() const = 0;
		virtual void :ref:`set_as_any<doxid-classov_1_1_value_accessor_3_01void_01_4_1a0c1742a307e955a2dd854fd350464644>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);


.. index:: pair: class; ov::ValueAccessor
.. _doxid-classov_1_1_value_accessor:

class ov::ValueAccessor
^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

Provides access to an attribute of type AT as a value accessor type VAT. :ref:`More...<details-classov_1_1_value_accessor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <typename VAT>
	class ValueAccessor
	{
	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :target:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
	};

	// direct descendants

	template <typename AT, typename VAT>
	class :ref:`IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor>`;

	template <typename AT, typename VAT>
	class :ref:`IndirectVectorValueAccessor<doxid-classov_1_1_indirect_vector_value_accessor>`;
.. _details-classov_1_1_value_accessor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Provides access to an attribute of type AT as a value accessor type VAT.

Provides access to values via get/set methods from an m_value, typically from ValueReference.

The m_buffer holds a VAT, which may be wider than the attribute AT. For example, serializers that only support int64_t integers would use a :ref:`ValueAccessor <doxid-classov_1_1_value_accessor>` <vector<int64_t>> to reference a vector<int8_t> attribute. Destruction moves the value back to the attribute if it was changed.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- VAT

		- The adapter value type; may be wider than the value being accessed.

Methods
-------

.. _doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const VAT& get() = 0

Returns the value.

.. _doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const VAT& value) = 0

Sets the value.


