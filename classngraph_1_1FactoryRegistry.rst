.. index:: pair: class; ngraph::FactoryRegistry
.. _doxid-classngraph_1_1_factory_registry:

class ngraph::FactoryRegistry
=============================



Overview
~~~~~~~~

Registry of factories that can construct objects derived from BASE_TYPE. :ref:`More...<details-classngraph_1_1_factory_registry>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <factory.hpp>
	
	template <typename BASE_TYPE>
	class FactoryRegistry
	{
	public:
		// typedefs
	
		typedef std::function<BASE_TYPE \*()> :target:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>`;
		typedef std::unordered_map<typename BASE_TYPE::type_info_t, :ref:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>`> :target:`FactoryMap<doxid-classngraph_1_1_factory_registry_1a84507d8150fffe42cb1fcf27ae22f512>`;

		// methods
	
		template <typename DERIVED_TYPE>
		static :ref:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>` :target:`get_default_factory<doxid-classngraph_1_1_factory_registry_1a1ea824d7c7929d0afd024adf8f0ec0ca>`();
	
		void :ref:`register_factory<doxid-classngraph_1_1_factory_registry_1a891b3eea7cbf54356ed2923b26891d19>`(
			const typename BASE_TYPE::type_info_t& type_info,
			:ref:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>` factory
			);
	
		template <
			typename DERIVED_TYPE,
			typename std::enable_if<!HasTypeInfoMember<DERIVED_TYPE>::value, bool>::type = true
			>
		void :ref:`register_factory<doxid-classngraph_1_1_factory_registry_1a316960105dc47cec2d82e40951598fb7>`(:ref:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>` factory);
	
		template <typename DERIVED_TYPE>
		void :ref:`register_factory<doxid-classngraph_1_1_factory_registry_1a1f9e500f05ccee783652fa0d42470e38>`();
	
		bool :ref:`has_factory<doxid-classngraph_1_1_factory_registry_1a33065f1b3e89b44fe4d1e762d2a8a592>`(const typename BASE_TYPE::type_info_t& info);
	
		template <
			typename DERIVED_TYPE,
			typename std::enable_if<!HasTypeInfoMember<DERIVED_TYPE>::value, bool>::type = true
			>
		bool :ref:`has_factory<doxid-classngraph_1_1_factory_registry_1ac0c9ed7c8216f05f172f990681490c7a>`();
	
		BASE_TYPE \* :ref:`create<doxid-classngraph_1_1_factory_registry_1a560573585274e78a212c8d2891ad047e>`(const typename BASE_TYPE::type_info_t& type_info) const;
	
		template <
			typename DERIVED_TYPE,
			typename std::enable_if<!HasTypeInfoMember<DERIVED_TYPE>::value, bool>::type = true
			>
		BASE_TYPE \* :ref:`create<doxid-classngraph_1_1_factory_registry_1a002f58982dfe380848e699d27c70584a>`() const;
	};
.. _details-classngraph_1_1_factory_registry:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Registry of factories that can construct objects derived from BASE_TYPE.

Methods
-------

.. _doxid-classngraph_1_1_factory_registry_1a891b3eea7cbf54356ed2923b26891d19:
.. index:: pair: function; register_factory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void register_factory(
		const typename BASE_TYPE::type_info_t& type_info,
		:ref:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>` factory
		)

Register a custom factory for type_info.

.. _doxid-classngraph_1_1_factory_registry_1a316960105dc47cec2d82e40951598fb7:
.. index:: pair: function; register_factory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename DERIVED_TYPE,
		typename std::enable_if<!HasTypeInfoMember<DERIVED_TYPE>::value, bool>::type = true
		>
	void register_factory(:ref:`Factory<doxid-classngraph_1_1_factory_registry_1ab2cc7f9235b3461e9ddc8b143d0146ba>` factory)

Register a custom factory for DERIVED_TYPE.

.. _doxid-classngraph_1_1_factory_registry_1a1f9e500f05ccee783652fa0d42470e38:
.. index:: pair: function; register_factory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename DERIVED_TYPE>
	void register_factory()

Register the defualt constructor factory for DERIVED_TYPE.

.. _doxid-classngraph_1_1_factory_registry_1a33065f1b3e89b44fe4d1e762d2a8a592:
.. index:: pair: function; has_factory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has_factory(const typename BASE_TYPE::type_info_t& info)

Check to see if a factory is registered.

.. _doxid-classngraph_1_1_factory_registry_1ac0c9ed7c8216f05f172f990681490c7a:
.. index:: pair: function; has_factory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename DERIVED_TYPE,
		typename std::enable_if<!HasTypeInfoMember<DERIVED_TYPE>::value, bool>::type = true
		>
	bool has_factory()

Check to see if DERIVED_TYPE has a registered factory.

.. _doxid-classngraph_1_1_factory_registry_1a560573585274e78a212c8d2891ad047e:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BASE_TYPE \* create(const typename BASE_TYPE::type_info_t& type_info) const

Create an instance for type_info.

.. _doxid-classngraph_1_1_factory_registry_1a002f58982dfe380848e699d27c70584a:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename DERIVED_TYPE,
		typename std::enable_if<!HasTypeInfoMember<DERIVED_TYPE>::value, bool>::type = true
		>
	BASE_TYPE \* create() const

Create an instance using factory for DERIVED_TYPE.


