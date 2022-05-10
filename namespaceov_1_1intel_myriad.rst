.. index:: pair: namespace; ov::intel_myriad
.. _doxid-namespaceov_1_1intel__myriad:

namespace ov::intel_myriad
==========================

.. toctree::
	:hidden:

	hddl <namespaceov_1_1intel_myriad_1_1hddl.rst>

Namespace with Intel MYRIAD specific properties.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace intel_myriad {

	// namespaces

	namespace :ref:`ov::intel_myriad::hddl<doxid-namespaceov_1_1intel__myriad_1_1hddl>`;

	// enums

	enum :ref:`DDRType<doxid-group__ov__runtime__myriad__prop__cpp__api_1gaf3f7a1cafdc1acaec64ec9dfbaf42787>`;
	enum :ref:`Protocol<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga2c3d4f3906b3ea3dbcb6d6856a5ee8ff>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`enable_hw_acceleration<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga6d41482880d8da150897dedce899daa0>` {"MYRIAD_ENABLE_HW_ACCELERATION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`enable_receiving_tensor_time<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga7787dfa516d32419556b2434d1eb3a2b>` {     "MYRIAD_ENABLE_RECEIVING_TENSOR_TIME"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`custom_layers<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga166948dec9902d5bf331f8e1ff4d145d>` {"MYRIAD_CUSTOM_LAYERS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Protocol<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga2c3d4f3906b3ea3dbcb6d6856a5ee8ff>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`protocol<doxid-group__ov__runtime__myriad__prop__cpp__api_1ga5d9fb02cb36acca0777b6a2571599cd3>` {"MYRIAD_PROTOCOL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`enable_force_reset<doxid-group__ov__runtime__myriad__prop__cpp__api_1ga1fcc2ed7f52f92abd3318734121c3a97>` {"MYRIAD_ENABLE_FORCE_RESET"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`DDRType<doxid-group__ov__runtime__myriad__prop__cpp__api_1gaf3f7a1cafdc1acaec64ec9dfbaf42787>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ddr_type<doxid-group__ov__runtime__myriad__prop__cpp__api_1ga0587abb1479085412e6d0decfbd298d9>` {"MYRIAD_DDR_TYPE"};

	} // namespace intel_myriad
