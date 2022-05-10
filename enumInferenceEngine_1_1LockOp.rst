.. index:: pair: enum; LockOp
.. _doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748:

enum InferenceEngine::LockOp
============================

Overview
~~~~~~~~

Allocator handle mapping type. :ref:`More...<details-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_allocator.hpp>

	enum LockOp
	{
	    :ref:`LOCK_FOR_READ<doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748a455fd37b41073383decc4f578297152f>`  = 0,
	    :ref:`LOCK_FOR_WRITE<doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748a9ae5a20894f9cef968af6db3cdcdbe62>`,
	};

.. _details-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Allocator handle mapping type.

Enum Values
-----------

.. _doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748a455fd37b41073383decc4f578297152f:
.. index:: pair: enumvalue; LOCK_FOR_READ

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LOCK_FOR_READ

A flag to lock data for read.

.. _doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748a9ae5a20894f9cef968af6db3cdcdbe62:
.. index:: pair: enumvalue; LOCK_FOR_WRITE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LOCK_FOR_WRITE

A flag to lock data for write.

