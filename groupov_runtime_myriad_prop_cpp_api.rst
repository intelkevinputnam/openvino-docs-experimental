.. index:: pair: group; Intel MYRIAD specific properties
.. _doxid-group__ov__runtime__myriad__prop__cpp__api:

Intel MYRIAD specific properties
================================

.. toctree::
	:hidden:

	DDRType <enumov_1_1intel_myriad_1_1DDRType.rst>

Overview
~~~~~~~~

Set of Intel MYRIAD specific properties. :ref:`More...<details-group__ov__runtime__myriad__prop__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// enums

	enum :ref:`ov::intel_myriad::DDRType<doxid-group__ov__runtime__myriad__prop__cpp__api_1gaf3f7a1cafdc1acaec64ec9dfbaf42787>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Protocol<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga2c3d4f3906b3ea3dbcb6d6856a5ee8ff>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::protocol<doxid-group__ov__runtime__myriad__prop__cpp__api_1ga5d9fb02cb36acca0777b6a2571599cd3>` {"MYRIAD_PROTOCOL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::enable_force_reset<doxid-group__ov__runtime__myriad__prop__cpp__api_1ga1fcc2ed7f52f92abd3318734121c3a97>` {"MYRIAD_ENABLE_FORCE_RESET"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`DDRType<doxid-group__ov__runtime__myriad__prop__cpp__api_1gaf3f7a1cafdc1acaec64ec9dfbaf42787>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::ddr_type<doxid-group__ov__runtime__myriad__prop__cpp__api_1ga0587abb1479085412e6d0decfbd298d9>` {"MYRIAD_DDR_TYPE"};

.. _details-group__ov__runtime__myriad__prop__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of Intel MYRIAD specific properties.

Global Variables
----------------

.. _doxid-group__ov__runtime__myriad__prop__cpp__api_1ga5d9fb02cb36acca0777b6a2571599cd3:
.. index:: pair: variable; protocol

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Protocol<doxid-group__ov__runtime__myriad__hddl__prop__cpp__api_1ga2c3d4f3906b3ea3dbcb6d6856a5ee8ff>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::protocol {"MYRIAD_PROTOCOL"}

This option allows to specify protocol.

.. _doxid-group__ov__runtime__myriad__prop__cpp__api_1ga1fcc2ed7f52f92abd3318734121c3a97:
.. index:: pair: variable; enable_force_reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::enable_force_reset {"MYRIAD_ENABLE_FORCE_RESET"}

The flag to reset stalled devices.

.. _doxid-group__ov__runtime__myriad__prop__cpp__api_1ga0587abb1479085412e6d0decfbd298d9:
.. index:: pair: variable; ddr_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`DDRType<doxid-group__ov__runtime__myriad__prop__cpp__api_1gaf3f7a1cafdc1acaec64ec9dfbaf42787>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::ddr_type {"MYRIAD_DDR_TYPE"}

This option allows to specify device memory type.

