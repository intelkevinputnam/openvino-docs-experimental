.. index:: pair: class; InferenceEngine::LockedMemory<void>
.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4:

class InferenceEngine::LockedMemory<void>
=========================================



Overview
~~~~~~~~

This class is for <void\*> data and allows casting to any pointers. :ref:`More...<details-class_inference_engine_1_1_locked_memory_3_01void_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_locked_memory.hpp>
	
	template <>
	class LockedMemory<void>: public InferenceEngine::details::LockedMemoryBase< void >
	{
	public:
		// construction
	
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a3c21d89fdc0caa365014e4385df6189c>`(:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>` \* ptr, void \* handle, size_t offsetInBytes);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a4642ed9fc56828cebf97ce861bda4027>`(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void>&&);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1aff0bfa4863523b87d0c189a291d42284>`(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void>&& that, size_t offset);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1aa4e44ae423451a1bd3041dd9c2a5f39c>`(const :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void>&);

		// methods
	
		template <class S>
		:ref:`operator S\*<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a8e6d7238bcdad6b06f6dfa18499568eb>` ();
	
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a258b9009dd6a544c4d44c82edf91562d>` (const void \* pointer) const;
	
		template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
		S :ref:`as<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1ab6c75503c858b076f528a5a0d971227f>`();
	
		template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
		const S :ref:`as<doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a24909bd3a9327646ef194a8584fafcb9>`() const;
	};
.. _details-class_inference_engine_1_1_locked_memory_3_01void_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is for <void\*> data and allows casting to any pointers.

Construction
------------

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a3c21d89fdc0caa365014e4385df6189c:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>` \* ptr, void \* handle, size_t offsetInBytes)

A constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ptr

		- Pointer to :ref:`IAllocator <doxid-class_inference_engine_1_1_i_allocator>` object

	*
		- handle

		- Handle provided by allocator

	*
		- offsetInBytes

		- Offset in originally locked region

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a4642ed9fc56828cebf97ce861bda4027:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void>&&)

A default copy constructor that accepts rvalue.

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1aff0bfa4863523b87d0c189a291d42284:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void>&& that, size_t offset)

A default copy constructor that accepts rvalue.

Also sets the offset value for the new memory object



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- that

		- Rvalue reference for the other LockedMemoryBase instance

	*
		- offset

		- Offset value

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1aa4e44ae423451a1bd3041dd9c2a5f39c:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(const :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<void>&)

A disabled copy constructor for lvalue.

Methods
-------

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a8e6d7238bcdad6b06f6dfa18499568eb:
.. index:: pair: function; operator S\*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class S>
	operator S\* ()

Gets the pointer to the stored object of the given template type.

Dereferences from the base class.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- S

		- Type to be casted to



.. rubric:: Returns:

The pointer to the object of the given template type

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a258b9009dd6a544c4d44c82edf91562d:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const void \* pointer) const

Compares stored object with the given one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pointer

		- A pointer to compare with



.. rubric:: Returns:

``true`` if objects are equal, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1ab6c75503c858b076f528a5a0d971227f:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
	S as()

Casts stored object to any given type.

Uses reinterpret_cast.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- S

		- Type to be casted to



.. rubric:: Returns:

Casted to the given type object

.. _doxid-class_inference_engine_1_1_locked_memory_3_01void_01_4_1a24909bd3a9327646ef194a8584fafcb9:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
	const S as() const

Casts stored object to any given type.

Uses reinterpret_cast.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- S

		- Type to be casted to



.. rubric:: Returns:

Casted to the given type const object


.. index:: pair: class; InferenceEngine::LockedMemory
.. _doxid-class_inference_engine_1_1_locked_memory:

class InferenceEngine::LockedMemory
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

This class represents locked memory for read/write memory. :ref:`More...<details-class_inference_engine_1_1_locked_memory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_locked_memory.hpp>
	
	template <class T>
	class LockedMemory: public InferenceEngine::details::LockedMemoryBase< T >
	{
	public:
		// construction
	
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_1aec432066a40a9ebb9cea82afd7a4aefd>`(:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>` \* ptr, void \* handle, size_t offsetInBytes = 0);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_1ab36ef617634752794937d2fc83a6d112>`(LockedMemory<T>&&);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_1aae50616febcf8cf15b2d85c78730d5da>`(LockedMemory<T>&& that, size_t offset);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_1a33ff298d3d0447f4e9dcea175c150c6d>`(const LockedMemory<T>&);

		// methods
	
		:ref:`operator T\*<doxid-class_inference_engine_1_1_locked_memory_1a7b227fccb2f80d1d18bbc6ba218f2951>` ();
		:ref:`operator const T \*<doxid-class_inference_engine_1_1_locked_memory_1a1fc8ed09e5203c33ddc729ccb0588eca>` () const;
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_locked_memory_1a188defaa0e32097637fbdd48174b2c59>` (const T \* pointer) const;
	
		template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
		S :ref:`as<doxid-class_inference_engine_1_1_locked_memory_1a178d658777b108f168c492392b3d7052>`();
	
		template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
		const S :ref:`as<doxid-class_inference_engine_1_1_locked_memory_1a6fd39cb6524cbab23124f78dad0cbea2>`() const;
	};
.. _details-class_inference_engine_1_1_locked_memory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents locked memory for read/write memory.

Construction
------------

.. _doxid-class_inference_engine_1_1_locked_memory_1aec432066a40a9ebb9cea82afd7a4aefd:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>` \* ptr, void \* handle, size_t offsetInBytes = 0)

A constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ptr

		- Pointer to :ref:`IAllocator <doxid-class_inference_engine_1_1_i_allocator>` object

	*
		- handle

		- Handle provided by allocator

	*
		- offsetInBytes

		- Offset in originally locked region

.. _doxid-class_inference_engine_1_1_locked_memory_1ab36ef617634752794937d2fc83a6d112:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(LockedMemory<T>&&)

A default copy constructor, accepting rvalue.

.. _doxid-class_inference_engine_1_1_locked_memory_1aae50616febcf8cf15b2d85c78730d5da:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(LockedMemory<T>&& that, size_t offset)

A default copy constructor that accepts rvalue.

Also sets the offset value for the new memory object



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- that

		- Rvalue reference for the other LockedMemoryBase instance

	*
		- offset

		- Offset value

.. _doxid-class_inference_engine_1_1_locked_memory_1a33ff298d3d0447f4e9dcea175c150c6d:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(const LockedMemory<T>&)

A disabled copy constructor for lvalue.

Methods
-------

.. _doxid-class_inference_engine_1_1_locked_memory_1a7b227fccb2f80d1d18bbc6ba218f2951:
.. index:: pair: function; operator T\*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator T\* ()

Gets a pointer to the stored object.

Dereferences from the base class.



.. rubric:: Returns:

The pointer to the object of the given template type

.. _doxid-class_inference_engine_1_1_locked_memory_1a1fc8ed09e5203c33ddc729ccb0588eca:
.. index:: pair: function; operator const T \*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator const T \* () const

Gets the const pointer to the stored object.

Dereferences from the base class.



.. rubric:: Returns:

The const pointer object of the given template type.

.. _doxid-class_inference_engine_1_1_locked_memory_1a188defaa0e32097637fbdd48174b2c59:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const T \* pointer) const

Compares stored object with the given one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pointer

		- An pointer to compare with.



.. rubric:: Returns:

``true`` if objects are equal, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_locked_memory_1a178d658777b108f168c492392b3d7052:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
	S as()

Casts stored object to any provided type.

Uses reinterpret_cast.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- S

		- Type to be casted to



.. rubric:: Returns:

Casted to the given type object

.. _doxid-class_inference_engine_1_1_locked_memory_1a6fd39cb6524cbab23124f78dad0cbea2:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class S, typename = std::enable_if<std::is_pointer<S>::value>>
	const S as() const

Casts stored object to any provided type.

Uses reinterpret_cast.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- S

		- Type to be casted to



.. rubric:: Returns:

Casted to the given type const object


.. index:: pair: class; InferenceEngine::LockedMemory<const T>
.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4:

class InferenceEngine::LockedMemory<const T>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

This class is for read-only segments. :ref:`More...<details-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_locked_memory.hpp>
	
	template <class T>
	class LockedMemory<const T>: public InferenceEngine::details::LockedMemoryBase< T >
	{
	public:
		// construction
	
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a775b3a8fb7b1a5cdce9b812b43ec6cfb>`(:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>` \* ptr, void \* handle, size_t offset);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1af210d65c23691d5f376411f2136c9a54>`(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T>&&);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a9201057396506b4c58e314ee5f41f1c9>`(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T>&& that, size_t offset);
		:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a802d95c3de176606a302c5cbc67a087e>`(const :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T>&);

		// methods
	
		:ref:`operator const T \*<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a473a05b5a08de5a0402fdf82d9331692>` () const;
		bool :ref:`operator ==<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a4f711f039ebe7d90bf1d9e94a8370f0c>` (const T \* pointer) const;
	
		template <
			class S,
			typename = std::enable_if<std::is_pointer<S>::value&& std::is_const<S>::value>
			>
		S :ref:`as<doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1abf56b3d713f5810aea5230c747721f03>`() const;
	};
.. _details-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is for read-only segments.

Construction
------------

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a775b3a8fb7b1a5cdce9b812b43ec6cfb:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`IAllocator<doxid-class_inference_engine_1_1_i_allocator>` \* ptr, void \* handle, size_t offset)

A constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ptr

		- Pointer to :ref:`IAllocator <doxid-class_inference_engine_1_1_i_allocator>` object

	*
		- handle

		- Handle provided by allocator

	*
		- offset

		- Offset in bytes in originally locked region

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1af210d65c23691d5f376411f2136c9a54:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T>&&)

A default copy constructor that accepts rvalue.

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a9201057396506b4c58e314ee5f41f1c9:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(:ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T>&& that, size_t offset)

A default copy constructor that accepts rvalue.

Also sets the offset value for the new memory object



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- that

		- Rvalue reference for the other LockedMemoryBase instance

	*
		- offset

		- Offset value

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a802d95c3de176606a302c5cbc67a087e:
.. index:: pair: function; LockedMemory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LockedMemory(const :ref:`LockedMemory<doxid-class_inference_engine_1_1_locked_memory>`<const T>&)

A disabled copy constructor for lvalue.

Methods
-------

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a473a05b5a08de5a0402fdf82d9331692:
.. index:: pair: function; operator const T \*

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator const T \* () const

Gets the const pointer to the stored object.

Dereferences from the base class.



.. rubric:: Returns:

The pointer to the object.

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1a4f711f039ebe7d90bf1d9e94a8370f0c:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const T \* pointer) const

Compares stored object with the given one.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pointer

		- A pointer to compare with



.. rubric:: Returns:

``true`` if objects are equal, ``false`` otherwise

.. _doxid-class_inference_engine_1_1_locked_memory_3_01const_01_t_01_4_1abf56b3d713f5810aea5230c747721f03:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class S,
		typename = std::enable_if<std::is_pointer<S>::value&& std::is_const<S>::value>
		>
	S as() const

Casts stored object to any given type.

Uses reinterpret_cast.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- S

		- Type to be casted to



.. rubric:: Returns:

Casted to the given type object


