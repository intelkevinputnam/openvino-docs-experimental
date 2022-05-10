.. index:: pair: class; ov::IndirectScalarValueAccessor
.. _doxid-classov_1_1_indirect_scalar_value_accessor:

class ov::IndirectScalarValueAccessor
=====================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attribute_adapter.hpp>
	
	template <typename AT, typename VAT>
	class IndirectScalarValueAccessor: public :ref:`ov::ValueAccessor<doxid-classov_1_1_value_accessor>`
	{
	public:
		// construction
	
		:target:`IndirectScalarValueAccessor<doxid-classov_1_1_indirect_scalar_value_accessor_1a7a0baad78d4320e486a1b3d3276e6b18>`(AT& ref);

		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131>`();
		virtual void :ref:`set<doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6>`(const VAT& value);
		void :target:`set_as_any<doxid-classov_1_1_indirect_scalar_value_accessor_1acc149417f79351ea9db3375f05626836>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);
	};

	// direct descendants

	template <>
	class :ref:`AttributeAdapter<float><doxid-classov_1_1_attribute_adapter_3_01float_01_4>`;

	template <>
	class :ref:`AttributeAdapter<int16_t><doxid-classov_1_1_attribute_adapter_3_01int16__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<int32_t><doxid-classov_1_1_attribute_adapter_3_01int32__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<int8_t><doxid-classov_1_1_attribute_adapter_3_01int8__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<uint16_t><doxid-classov_1_1_attribute_adapter_3_01uint16__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<uint32_t><doxid-classov_1_1_attribute_adapter_3_01uint32__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<uint64_t><doxid-classov_1_1_attribute_adapter_3_01uint64__t_01_4>`;

	template <>
	class :ref:`AttributeAdapter<uint8_t><doxid-classov_1_1_attribute_adapter_3_01uint8__t_01_4>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const VAT& :ref:`get<doxid-classov_1_1_value_accessor_1a8b9168b1c1839190cb7b9ac6442e56a0>`() = 0;
		virtual void :ref:`set<doxid-classov_1_1_value_accessor_1ac7807627850f319e95b8963f07e0f9e9>`(const VAT& value) = 0;
		void :ref:`set_as_any<doxid-classov_1_1_value_accessor_1a75e7e9a7c0acb0233d311619a65aa96c>`(const :ref:`ov::Any<doxid-classov_1_1_any>`& x);

.. _details-classov_1_1_indirect_scalar_value_accessor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1_indirect_scalar_value_accessor_1a043b6bbf2b4490ddfea5e3a9b8c40131:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const VAT& get()

Returns the value.

.. _doxid-classov_1_1_indirect_scalar_value_accessor_1ae3d4e2aa73aa6183afcca2be2a1413c6:
.. index:: pair: function; set

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set(const VAT& value)

Sets the value.


