.. index:: pair: interface; ov::AllocatorImpl
.. _doxid-structov_1_1_allocator_impl:

interface ov::AllocatorImpl
===========================



Overview
~~~~~~~~

Tries to act like `std::pmr::memory_resource <https://en.cppreference.com/w/cpp/memory/memory_resource>`__ :ref:`More...<details-structov_1_1_allocator_impl>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <allocator.hpp>
	
	template AllocatorImpl: public std::enable_shared_from_this< AllocatorImpl >
	{
		// typedefs
	
		typedef std::shared_ptr<AllocatorImpl> :ref:`Ptr<doxid-structov_1_1_allocator_impl_1a4aeac3df3fb19ddc7198da386ba7a97c>`;

		// methods
	
		virtual void \* :ref:`allocate<doxid-structov_1_1_allocator_impl_1aeb2053769adda171e7fe8601f99f329b>`(
			const size_t bytes,
			const size_t alignment = alignof(max_align_t)
			) = 0;
	
		virtual void :ref:`deallocate<doxid-structov_1_1_allocator_impl_1a73347925d4951fc2fb4a73402c912b11>`(
			void \* handle,
			const size_t bytes,
			size_t alignment = alignof(max_align_t)
			) = 0;
	
		virtual bool :ref:`is_equal<doxid-structov_1_1_allocator_impl_1a4dd4acab02a2a508f3ee1bb3c28c95f4>`(const AllocatorImpl& other) const = 0;

	protected:
	};
.. _details-structov_1_1_allocator_impl:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Tries to act like `std::pmr::memory_resource <https://en.cppreference.com/w/cpp/memory/memory_resource>`__

Typedefs
--------

.. _doxid-structov_1_1_allocator_impl_1a4aeac3df3fb19ddc7198da386ba7a97c:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<AllocatorImpl> Ptr

A smart pointer containing :ref:`AllocatorImpl <doxid-structov_1_1_allocator_impl>` object.

Methods
-------

.. _doxid-structov_1_1_allocator_impl_1aeb2053769adda171e7fe8601f99f329b:
.. index:: pair: function; allocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void \* allocate(
		const size_t bytes,
		const size_t alignment = alignof(max_align_t)
		) = 0

Allocates memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bytes

		- The size in bytes at least to allocate

	*
		- alignment

		- The alignment of storage

	*
		- :ref:`Exception <doxid-classov_1_1_exception>`

		- if specified size and alignment is not supported



.. rubric:: Returns:

Handle to the allocated resource

.. _doxid-structov_1_1_allocator_impl_1a73347925d4951fc2fb4a73402c912b11:
.. index:: pair: function; deallocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void deallocate(
		void \* handle,
		const size_t bytes,
		size_t alignment = alignof(max_align_t)
		) = 0

Releases the handle and all associated memory resources which invalidates the handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- handle

		- The handle to free

	*
		- bytes

		- The size in bytes that was passed into :ref:`allocate() <doxid-structov_1_1_allocator_impl_1aeb2053769adda171e7fe8601f99f329b>` method

	*
		- alignment

		- The alignment of storage that was passed into :ref:`allocate() <doxid-structov_1_1_allocator_impl_1aeb2053769adda171e7fe8601f99f329b>` method

.. _doxid-structov_1_1_allocator_impl_1a4dd4acab02a2a508f3ee1bb3c28c95f4:
.. index:: pair: function; is_equal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_equal(const AllocatorImpl& other) const = 0

Compares with other :ref:`AllocatorImpl <doxid-structov_1_1_allocator_impl>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Other instance of allocator



.. rubric:: Returns:

``true`` if and only if memory allocated from one :ref:`AllocatorImpl <doxid-structov_1_1_allocator_impl>` can be deallocated from the other and vice versa


