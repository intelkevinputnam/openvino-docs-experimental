.. index:: pair: enum; PropertyMutability
.. _doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47:

enum ov::PropertyMutability
===========================

Overview
~~~~~~~~

Enum to define property value mutability. :ref:`More...<details-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>

	enum PropertyMutability
	{
	    :ref:`RO<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`,
	    :ref:`RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47a5c6dc3d436504b7a65191cafe28212ee>`,
	};

.. _details-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define property value mutability.

Enum Values
-----------

.. _doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c:
.. index:: pair: enumvalue; RO

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RO

Read-only property values can not be passed as input parameter.

.. _doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47a5c6dc3d436504b7a65191cafe28212ee:
.. index:: pair: enumvalue; RW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RW

Read/Write property key may change readability in runtime.

