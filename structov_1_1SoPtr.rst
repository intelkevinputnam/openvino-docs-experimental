.. index:: pair: struct; ov::SoPtr
.. _doxid-structov_1_1_so_ptr:

struct ov::SoPtr
================



Overview
~~~~~~~~

This class instantiate object using shared library. :ref:`More...<details-structov_1_1_so_ptr>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <so_ptr.hpp>
	
	template <class T>
	struct SoPtr
	{
		// fields
	
		std::shared_ptr<T> :ref:`_ptr<doxid-structov_1_1_so_ptr_1a95c1eb4549cfde69051c51ab7c5bfe5a>`;
		std::shared_ptr<void> :ref:`_so<doxid-structov_1_1_so_ptr_1a497316a14902fcb092d812d2020dd14b>`;

		// construction
	
		:ref:`SoPtr<doxid-structov_1_1_so_ptr_1a4e2951b8363e8f4b0141cb00aa454910>`();
		:ref:`SoPtr<doxid-structov_1_1_so_ptr_1a47bcc70b24421567ba435b78900834c5>`(const std::shared_ptr<T>& ptr, const std::shared_ptr<void>& so);
	
		template <typename U>
		:ref:`SoPtr<doxid-structov_1_1_so_ptr_1a95d26bcf8496ecd836b8219920b3dffc>`(const SoPtr<U>& that);

		// methods
	
		T \* :ref:`operator -><doxid-structov_1_1_so_ptr_1a43c11c3f77f4c98d7798b8fc744ab4bb>` () const;
		:target:`operator bool<doxid-structov_1_1_so_ptr_1a122b3126b04349ac51ed5bbc7508ded9>` () const;
	};
.. _details-structov_1_1_so_ptr:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class instantiate object using shared library.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- An type of object :ref:`SoPtr <doxid-structov_1_1_so_ptr>` can hold

Fields
------

.. _doxid-structov_1_1_so_ptr_1a95c1eb4549cfde69051c51ab7c5bfe5a:
.. index:: pair: variable; _ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<T> _ptr

Gets a smart pointer to the custom object.

.. _doxid-structov_1_1_so_ptr_1a497316a14902fcb092d812d2020dd14b:
.. index:: pair: variable; _so

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<void> _so

The shared object or dinamic loaded library.

Construction
------------

.. _doxid-structov_1_1_so_ptr_1a4e2951b8363e8f4b0141cb00aa454910:
.. index:: pair: function; SoPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SoPtr()

Default constructor.

.. _doxid-structov_1_1_so_ptr_1a47bcc70b24421567ba435b78900834c5:
.. index:: pair: function; SoPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SoPtr(const std::shared_ptr<T>& ptr, const std::shared_ptr<void>& so)

Constructs an object with existing shared object reference and loaded pointer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ptr

		- pointer to the loaded object

	*
		- so

		- Existing reference to library

.. _doxid-structov_1_1_so_ptr_1a95d26bcf8496ecd836b8219920b3dffc:
.. index:: pair: function; SoPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename U>
	SoPtr(const SoPtr<U>& that)

The copy-like constructor, can create So Pointer that dereferenced into child type if T is derived of U.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- that

		- copied :ref:`SoPtr <doxid-structov_1_1_so_ptr>` object

Methods
-------

.. _doxid-structov_1_1_so_ptr_1a43c11c3f77f4c98d7798b8fc744ab4bb:
.. index:: pair: function; operator->

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	T \* operator -> () const

Standard pointer operator.



.. rubric:: Returns:

underlined interface with disabled Release method


