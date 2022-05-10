.. index:: pair: enum; PerformanceMode
.. _doxid-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73:

enum ov::hint::PerformanceMode
==============================

Overview
~~~~~~~~

Enum to define possible performance mode hints. :ref:`More...<details-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>

	enum PerformanceMode
	{
	    :ref:`UNDEFINED<doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a0db45d2a4141101bdfe48e3314cfbca3>`             = -1,
	    :ref:`LATENCY<doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a501069dd75f76384ba18f133fdce99c2>`               = 1,
	    :ref:`THROUGHPUT<doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a50f9b1f40c078d242af7ec323ace44b3>`            = 2,
	    :ref:`CUMULATIVE_THROUGHPUT<doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a02633a467c46bbc726b6dd719d224fc9>` = 3,
	};

.. _details-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define possible performance mode hints.

Enum Values
-----------

.. _doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a0db45d2a4141101bdfe48e3314cfbca3:
.. index:: pair: enumvalue; UNDEFINED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	UNDEFINED

Undefined value, performance setting may vary from device to device.

.. _doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a501069dd75f76384ba18f133fdce99c2:
.. index:: pair: enumvalue; LATENCY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LATENCY

Optimize for latency.

.. _doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a50f9b1f40c078d242af7ec323ace44b3:
.. index:: pair: enumvalue; THROUGHPUT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	THROUGHPUT

Optimize for throughput.

.. _doxid-group__ov__runtime__cpp__prop__api_1gga032aa530efa40760b79af14913d48d73a02633a467c46bbc726b6dd719d224fc9:
.. index:: pair: enumvalue; CUMULATIVE_THROUGHPUT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CUMULATIVE_THROUGHPUT

Optimize for cumulative throughput.

