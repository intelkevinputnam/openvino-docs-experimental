.. index:: pair: interface; InferenceEngine::IAllocator
.. _doxid-class_inference_engine_1_1_i_allocator:

interface InferenceEngine::IAllocator
=====================================



Overview
~~~~~~~~

Allocator concept to be used for memory management and is used as part of the :ref:`Blob <doxid-class_inference_engine_1_1_blob>`. :ref:`More...<details-class_inference_engine_1_1_i_allocator>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_allocator.hpp>
	
	template IAllocator: public std::enable_shared_from_this< IAllocator >
	{
		// methods
	
		virtual void \* :ref:`lock<doxid-class_inference_engine_1_1_i_allocator_1a56ad770ff0bd80c65c0d22a3ce0e3182>`(void \* handle, :ref:`LockOp<doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748>` op = :ref:`LOCK_FOR_WRITE<doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748a9ae5a20894f9cef968af6db3cdcdbe62>`) = 0;
		virtual void :ref:`unlock<doxid-class_inference_engine_1_1_i_allocator_1ad8670e6ae1cf6d217662fbeb88195da1>`(void \* handle) = 0;
		virtual void \* :ref:`alloc<doxid-class_inference_engine_1_1_i_allocator_1aadb8575b27a1015866d45feb53004367>`(size_t size) = 0;
		virtual bool :ref:`free<doxid-class_inference_engine_1_1_i_allocator_1a6b657b8f4edb595f2d37e03e8ed18815>`(void \* handle) = 0;

	protected:
	};
.. _details-class_inference_engine_1_1_i_allocator:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Allocator concept to be used for memory management and is used as part of the :ref:`Blob <doxid-class_inference_engine_1_1_blob>`.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_allocator_1a56ad770ff0bd80c65c0d22a3ce0e3182:
.. index:: pair: function; lock

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void \* lock(void \* handle, :ref:`LockOp<doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748>` op = :ref:`LOCK_FOR_WRITE<doxid-namespace_inference_engine_1aa4442e6dd90530b2501235e9f5252748a9ae5a20894f9cef968af6db3cdcdbe62>`) = 0

Maps handle to heap memory accessible by any memory manipulation routines.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- handle

		- Handle to the allocated memory to be locked

	*
		- op

		- Operation to lock memory for



.. rubric:: Returns:

Generic pointer to memory

.. _doxid-class_inference_engine_1_1_i_allocator_1ad8670e6ae1cf6d217662fbeb88195da1:
.. index:: pair: function; unlock

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void unlock(void \* handle) = 0

Unmaps memory by handle with multiple sequential mappings of the same handle.

The multiple sequential mappings of the same handle are suppose to get the same result while there isn't a ref counter supported.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- handle

		- Handle to the locked memory to unlock

.. _doxid-class_inference_engine_1_1_i_allocator_1aadb8575b27a1015866d45feb53004367:
.. index:: pair: function; alloc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void \* alloc(size_t size) = 0

Allocates memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size

		- The size in bytes to allocate



.. rubric:: Returns:

Handle to the allocated resource

.. _doxid-class_inference_engine_1_1_i_allocator_1a6b657b8f4edb595f2d37e03e8ed18815:
.. index:: pair: function; free

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool free(void \* handle) = 0

Releases the handle and all associated memory resources which invalidates the handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- handle

		- The handle to free



.. rubric:: Returns:

``false`` if handle cannot be released, otherwise - ``true``.


