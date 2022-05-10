.. index:: pair: namespace; ov::device
.. _doxid-namespaceov_1_1device:

namespace ov::device
====================

.. toctree::
	:hidden:

	capability <namespaceov_1_1device_1_1capability.rst>

Namespace with device properties.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace device {

	// namespaces

	namespace :ref:`ov::device::capability<doxid-namespaceov_1_1device_1_1capability>`;

	// enums

	enum :ref:`Type<doxid-group__ov__runtime__cpp__prop__api_1ga3c08e596389a1a1266dfa52681acd314>`;

	// structs

	struct :ref:`Priorities<doxid-structov_1_1device_1_1_priorities>`;
	struct :ref:`Properties<doxid-structov_1_1device_1_1_properties>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> :ref:`id<doxid-group__ov__runtime__cpp__prop__api_1ga433b8ea52e99c2b1fa8b26453485d75d>` {"DEVICE_ID"};
	static constexpr :ref:`Priorities<doxid-structov_1_1device_1_1_priorities>` :ref:`priorities<doxid-group__ov__runtime__cpp__prop__api_1gae88af90a18871677f39739cb0ef0101e>` {"MULTI_DEVICE_PRIORITIES"};
	static constexpr :ref:`Properties<doxid-structov_1_1device_1_1_properties>` :ref:`properties<doxid-group__ov__runtime__cpp__prop__api_1ga794d09f2bd8aad506508b2c53ef6a6fc>`;
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`full_name<doxid-group__ov__runtime__cpp__prop__api_1gaabacd9ea113b966be7b53b1d70fd6f42>` {"FULL_DEVICE_NAME"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`architecture<doxid-group__ov__runtime__cpp__prop__api_1gae2e72a4510ecf768ca196959b6c92fd4>` {"DEVICE_ARCHITECTURE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Type<doxid-group__ov__runtime__cpp__prop__api_1ga3c08e596389a1a1266dfa52681acd314>`, PropertyMutability::RO> :ref:`type<doxid-group__ov__runtime__cpp__prop__api_1gaf9b20fd37487c1f525e68c6e0567f1f1>` {"DEVICE_TYPE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, float>, PropertyMutability::RO> :ref:`gops<doxid-group__ov__runtime__cpp__prop__api_1gae233c458317f6ae508b887eb09308c4c>` {"DEVICE_GOPS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<float, PropertyMutability::RO> :ref:`thermal<doxid-group__ov__runtime__cpp__prop__api_1ga821543ca749cd78a8ced9930e0fec466>` {"DEVICE_THERMAL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`capabilities<doxid-group__ov__runtime__cpp__prop__api_1gadb13d62787fc4485733329f044987294>` {"OPTIMIZATION_CAPABILITIES"};

	} // namespace device
