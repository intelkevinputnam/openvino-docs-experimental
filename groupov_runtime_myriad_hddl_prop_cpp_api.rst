.. index:: pair: group; Intel MYRIAD & HDDL specific properties
.. _doxid-group__ov__runtime__myriad__hddl__prop__cpp__api:

Intel MYRIAD & HDDL specific properties
=======================================

.. toctree::
	:hidden:

	Protocol <enumov_1_1intel_myriad_1_1Protocol.rst>

Overview
~~~~~~~~

Set of Intel MYRIAD & HDDL specific properties. :ref:`More...<details-group__ov__runtime__myriad__hddl__prop__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// enums

	enum :ref:`ov::intel_myriad::Protocol<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga2c3d4f3906b3ea3dbcb6d6856a5ee8ff>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::enable_hw_acceleration<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga6d41482880d8da150897dedce899daa0>` {"MYRIAD_ENABLE_HW_ACCELERATION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::enable_receiving_tensor_time<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga7787dfa516d32419556b2434d1eb3a2b>` {     "MYRIAD_ENABLE_RECEIVING_TENSOR_TIME"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::custom_layers<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga166948dec9902d5bf331f8e1ff4d145d>` {"MYRIAD_CUSTOM_LAYERS"};

.. _details-group__ov__runtime__myriad__hddl__prop__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of Intel MYRIAD & HDDL specific properties.

Global Variables
----------------

.. _doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga6d41482880d8da150897dedce899daa0:
.. index:: pair: variable; enable_hw_acceleration

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::enable_hw_acceleration {"MYRIAD_ENABLE_HW_ACCELERATION"}

Turn on HW stages usage (applicable for MyriadX devices only).

.. _doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga7787dfa516d32419556b2434d1eb3a2b:
.. index:: pair: variable; enable_receiving_tensor_time

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::enable_receiving_tensor_time {     "MYRIAD_ENABLE_RECEIVING_TENSOR_TIME"}

The flag for adding to the profiling information the time of obtaining a tensor.

.. _doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga166948dec9902d5bf331f8e1ff4d145d:
.. index:: pair: variable; custom_layers

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::custom_layers {"MYRIAD_CUSTOM_LAYERS"}

This option allows to pass custom layers binding xml. If layer is present in such an xml, it would be used during inference even if the layer is natively supported.

