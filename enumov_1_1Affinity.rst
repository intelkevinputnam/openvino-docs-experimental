.. index:: pair: enum; Affinity
.. _doxid-group__ov__runtime__cpp__prop__api_1ga72b7c6cde7f94f07bc1519464c55e9c5:

enum ov::Affinity
=================

Overview
~~~~~~~~

Enum to define possible affinity patterns. :ref:`More...<details-group__ov__runtime__cpp__prop__api_1ga72b7c6cde7f94f07bc1519464c55e9c5>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>

	enum Affinity
	{
	    :ref:`NONE<doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ab50339a10e1de285ac99d4c3990b8693>`         = -1,
	    :ref:`CORE<doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ac5d5df976f196200d1900b2b51827dbb>`         = 0,
	    :ref:`NUMA<doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ab50c8803b99f15e242d2f68eac46d4fe>`         = 1,
	    :ref:`HYBRID_AWARE<doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ab251efd889b530f06f4abe4c690a39d0>` = 2,
	};

.. _details-group__ov__runtime__cpp__prop__api_1ga72b7c6cde7f94f07bc1519464c55e9c5:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define possible affinity patterns.

Enum Values
-----------

.. _doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ab50339a10e1de285ac99d4c3990b8693:
.. index:: pair: enumvalue; NONE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NONE

Disable threads affinity pinning.

.. _doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ac5d5df976f196200d1900b2b51827dbb:
.. index:: pair: enumvalue; CORE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CORE

Pin threads to cores, best for static benchmarks.

.. _doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ab50c8803b99f15e242d2f68eac46d4fe:
.. index:: pair: enumvalue; NUMA

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NUMA

Pin threads to NUMA nodes, best for real-life, contented cases. On the Windows and MacOS\* this option behaves as CORE

.. _doxid-group__ov__runtime__cpp__prop__api_1gga72b7c6cde7f94f07bc1519464c55e9c5ab251efd889b530f06f4abe4c690a39d0:
.. index:: pair: enumvalue; HYBRID_AWARE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HYBRID_AWARE

Let the runtime to do pinning to the cores types, e.g. prefer the "big" cores for latency tasks. On the hybrid CPUs this option is default

