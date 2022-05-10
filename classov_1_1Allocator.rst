.. index:: pair: class; ov::Allocator
.. _doxid-classov_1_1_allocator:

class ov::Allocator
===================



Overview
~~~~~~~~

Wraps allocator implementation to provide safe way to store allocater loaded from shared library And constructs default based on ``new`` ``delete`` c++ calls allocator if created without parameters. :ref:`More...<details-classov_1_1_allocator>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <allocator.hpp>
	
	class Allocator
	{
	public:
		// construction
	
		:ref:`Allocator<doxid-classov_1_1_allocator_1a907ad438bfb888b1193716874d7f7aeb>`();
		:ref:`Allocator<doxid-classov_1_1_allocator_1a094022c8d330c0079b64983862ec831f>`(const Allocator& other);
		:ref:`Allocator<doxid-classov_1_1_allocator_1a1da7720c8ee082335e1ccea1a4af8cee>`(Allocator&& other);
		:ref:`Allocator<doxid-classov_1_1_allocator_1aaba5c8627d378728cd7135e3d88a51c7>`(const :ref:`AllocatorImpl::Ptr<doxid-structov_1_1_allocator_impl_1a4aeac3df3fb19ddc7198da386ba7a97c>`& impl);

		// methods
	
		Allocator& :ref:`operator =<doxid-classov_1_1_allocator_1a7a57e650ccb672b1a0c6e796b7c7614e>` (const Allocator& other);
		Allocator& :ref:`operator =<doxid-classov_1_1_allocator_1ae4baff3f3e85bcf7b887272b745fdada>` (Allocator&& other);
	
		void \* :ref:`allocate<doxid-classov_1_1_allocator_1ab56f7d0a903b71ca7aa96b66cabd0627>`(
			const size_t bytes,
			const size_t alignment = alignof(max_align_t)
			);
	
		void :ref:`deallocate<doxid-classov_1_1_allocator_1af15fd104d9196aa150255737c08da612>`(
			void \* ptr,
			const size_t bytes = 0,
			const size_t alignment = alignof(max_align_t)
			);
	
		bool :ref:`operator ==<doxid-classov_1_1_allocator_1ab2ad5cd1e1beaf825f48c17bff8e6c57>` (const Allocator& other) const;
		bool :ref:`operator !<doxid-classov_1_1_allocator_1a3a80d7decd3ee7de595adf293f306284>` () const;
		:ref:`operator bool<doxid-classov_1_1_allocator_1a791cb1e71eb8017a250c8849b4f0fd84>` () const;
	};
.. _details-classov_1_1_allocator:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Wraps allocator implementation to provide safe way to store allocater loaded from shared library And constructs default based on ``new`` ``delete`` c++ calls allocator if created without parameters.

Construction
------------

.. _doxid-classov_1_1_allocator_1a907ad438bfb888b1193716874d7f7aeb:
.. index:: pair: function; Allocator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Allocator()

Default constructor.

.. _doxid-classov_1_1_allocator_1a094022c8d330c0079b64983862ec831f:
.. index:: pair: function; Allocator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Allocator(const Allocator& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Allocator <doxid-classov_1_1_allocator>` object

.. _doxid-classov_1_1_allocator_1a1da7720c8ee082335e1ccea1a4af8cee:
.. index:: pair: function; Allocator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Allocator(Allocator&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Allocator <doxid-classov_1_1_allocator>` object

.. _doxid-classov_1_1_allocator_1aaba5c8627d378728cd7135e3d88a51c7:
.. index:: pair: function; Allocator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Allocator(const :ref:`AllocatorImpl::Ptr<doxid-structov_1_1_allocator_impl_1a4aeac3df3fb19ddc7198da386ba7a97c>`& impl)

Constructs :ref:`Allocator <doxid-classov_1_1_allocator>` from the initialized std::shared_ptr.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- impl

		- Initialized shared pointer

Methods
-------

.. _doxid-classov_1_1_allocator_1a7a57e650ccb672b1a0c6e796b7c7614e:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Allocator& operator = (const Allocator& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Allocator <doxid-classov_1_1_allocator>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-classov_1_1_allocator_1ae4baff3f3e85bcf7b887272b745fdada:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Allocator& operator = (Allocator&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Allocator <doxid-classov_1_1_allocator>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-classov_1_1_allocator_1ab56f7d0a903b71ca7aa96b66cabd0627:
.. index:: pair: function; allocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void \* allocate(
		const size_t bytes,
		const size_t alignment = alignof(max_align_t)
		)

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

.. _doxid-classov_1_1_allocator_1af15fd104d9196aa150255737c08da612:
.. index:: pair: function; deallocate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void deallocate(
		void \* ptr,
		const size_t bytes = 0,
		const size_t alignment = alignof(max_align_t)
		)

Releases the handle and all associated memory resources which invalidates the handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ptr

		- The handle to free

	*
		- bytes

		- The size in bytes that was passed into :ref:`allocate() <doxid-classov_1_1_allocator_1ab56f7d0a903b71ca7aa96b66cabd0627>` method

	*
		- alignment

		- The alignment of storage that was passed into :ref:`allocate() <doxid-classov_1_1_allocator_1ab56f7d0a903b71ca7aa96b66cabd0627>` method

.. _doxid-classov_1_1_allocator_1ab2ad5cd1e1beaf825f48c17bff8e6c57:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const Allocator& other) const

Compares with other :ref:`AllocatorImpl <doxid-structov_1_1_allocator_impl>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Other instance of allocator



.. rubric:: Returns:

``true`` if and only if memory allocated from one :ref:`AllocatorImpl <doxid-structov_1_1_allocator_impl>` can be deallocated from the other and vice versa

.. _doxid-classov_1_1_allocator_1a3a80d7decd3ee7de595adf293f306284:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Checks if current :ref:`Allocator <doxid-classov_1_1_allocator>` object is not initialized.



.. rubric:: Returns:

``true`` if current :ref:`Allocator <doxid-classov_1_1_allocator>` object is not initialized, ``false`` - otherwise

.. _doxid-classov_1_1_allocator_1a791cb1e71eb8017a250c8849b4f0fd84:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Checks if current :ref:`Allocator <doxid-classov_1_1_allocator>` object is initialized.



.. rubric:: Returns:

``true`` if current :ref:`Allocator <doxid-classov_1_1_allocator>` object is initialized, ``false`` - otherwise


