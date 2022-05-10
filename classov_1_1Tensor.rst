.. index:: pair: class; ov::Tensor
.. _doxid-classov_1_1_tensor:

class ov::Tensor
================



Overview
~~~~~~~~

:ref:`Tensor <doxid-classov_1_1_tensor>` API holding host memory It can throw exceptions safely for the application, where it is properly handled. :ref:`More...<details-classov_1_1_tensor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <tensor.hpp>
	
	class Tensor
	{
	public:
		// construction
	
		:ref:`Tensor<doxid-classov_1_1_tensor_1a50b5d3c5e71f4d30da8c71a8f4397af3>`();
		:ref:`Tensor<doxid-classov_1_1_tensor_1a486603ee276e99f6e537640fcee39b0f>`(const Tensor& other);
		:ref:`Tensor<doxid-classov_1_1_tensor_1a5154e2ae344d1c0f8ab747c4f6fa784a>`(Tensor&& other);
	
		:ref:`Tensor<doxid-classov_1_1_tensor_1a464c71b240bebcadf89442432df26efb>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const :ref:`Allocator<doxid-classov_1_1_allocator>`& allocator = {}
			);
	
		:ref:`Tensor<doxid-classov_1_1_tensor_1a900804c0948fca52f8d848e93bd393d8>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			void \* host_ptr,
			const :ref:`Strides<doxid-classov_1_1_strides>`& strides = {}
			);
	
		:ref:`Tensor<doxid-classov_1_1_tensor_1ad2d8cdb3c97ff1a6f212a59f1a4e07ef>`(const Tensor& other, const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& begin, const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& end);

		// methods
	
		Tensor& :ref:`operator =<doxid-classov_1_1_tensor_1a83b0b800c932eca2a5e9d42dfdae655c>` (const Tensor& other);
		Tensor& :ref:`operator =<doxid-classov_1_1_tensor_1a3cf1d342fa056b59fd5bc38964d54575>` (Tensor&& other);
		void :ref:`set_shape<doxid-classov_1_1_tensor_1a7a513a53ac7221d1a52006c34bce6c18>`(const :ref:`ov::Shape<doxid-classov_1_1_shape>`& shape);
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :ref:`get_element_type<doxid-classov_1_1_tensor_1a7b00f757407bfee07d831647f15b1686>`() const;
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`get_shape<doxid-classov_1_1_tensor_1a706163e01fb555eb9ccdfb5204cf7834>`() const;
		size_t :ref:`get_size<doxid-classov_1_1_tensor_1a26dfed6a65b46d9a25562e811912f09d>`() const;
		size_t :ref:`get_byte_size<doxid-classov_1_1_tensor_1ae540fcafc1e9dc9181e86a1ec2682935>`() const;
		:ref:`Strides<doxid-classov_1_1_strides>` :ref:`get_strides<doxid-classov_1_1_tensor_1a610491239de68e700c7c3579479b6692>`() const;
		void \* :ref:`data<doxid-classov_1_1_tensor_1ac1b8835f54d67d92969d7979e666e2a8>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type = {}) const;
	
		template <typename T, typename datatype = typename std::decay<T>::type>
		T \* :ref:`data<doxid-classov_1_1_tensor_1ae73e29ecaf40339a7b4f6b65cdde0736>`() const;
	
		bool :ref:`operator !<doxid-classov_1_1_tensor_1aa65688ce884468fdd9bd9cc24dda907a>` () const;
		:ref:`operator bool<doxid-classov_1_1_tensor_1a7ac03a96d3eeca3f057307bccb095df5>` () const;
	
		template <typename T>
		std::enable_if<std::is_base_of<Tensor, T>::value, bool>::type :ref:`is<doxid-classov_1_1_tensor_1a287c90f6c44793fd411e26490786c83d>`() const;
	
		template <typename T>
		const std::enable_if<std::is_base_of<Tensor, T>::value, T>::type :ref:`as<doxid-classov_1_1_tensor_1a345f8ade85da6fe30bcf8a3ae15a4bca>`() const;
	
		static void :ref:`type_check<doxid-classov_1_1_tensor_1a8beef8846cacaa542e3b51c061d50e42>`(const Tensor& tensor);
	};

	// direct descendants

	class :ref:`RemoteTensor<doxid-classov_1_1_remote_tensor>`;
.. _details-classov_1_1_tensor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Tensor <doxid-classov_1_1_tensor>` API holding host memory It can throw exceptions safely for the application, where it is properly handled.

Construction
------------

.. _doxid-classov_1_1_tensor_1a50b5d3c5e71f4d30da8c71a8f4397af3:
.. index:: pair: function; Tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor()

Default constructor.

.. _doxid-classov_1_1_tensor_1a486603ee276e99f6e537640fcee39b0f:
.. index:: pair: function; Tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor(const Tensor& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Tensor <doxid-classov_1_1_tensor>` object

.. _doxid-classov_1_1_tensor_1a5154e2ae344d1c0f8ab747c4f6fa784a:
.. index:: pair: function; Tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor(Tensor&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Tensor <doxid-classov_1_1_tensor>` object

.. _doxid-classov_1_1_tensor_1a464c71b240bebcadf89442432df26efb:
.. index:: pair: function; Tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const :ref:`Allocator<doxid-classov_1_1_allocator>`& allocator = {}
		)

Constructs :ref:`Tensor <doxid-classov_1_1_tensor>` using element type and shape. Allocate internal host storage using default allocator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- allocator

		- allocates memory for internal tensor storage

.. _doxid-classov_1_1_tensor_1a900804c0948fca52f8d848e93bd393d8:
.. index:: pair: function; Tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		void \* host_ptr,
		const :ref:`Strides<doxid-classov_1_1_strides>`& strides = {}
		)

Constructs :ref:`Tensor <doxid-classov_1_1_tensor>` using element type and shape. Wraps allocated host memory.

Does not perform memory allocation internally



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape

	*
		- host_ptr

		- Pointer to pre-allocated host memory

	*
		- strides

		- Optional strides parameters in bytes. :ref:`Strides <doxid-classov_1_1_strides>` are supposed to be computed automatically based on shape and element size

.. _doxid-classov_1_1_tensor_1ad2d8cdb3c97ff1a6f212a59f1a4e07ef:
.. index:: pair: function; Tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor(const Tensor& other, const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& begin, const :ref:`Coordinate<doxid-classov_1_1_coordinate>`& end)

Constructs region of interest (ROI) tensor form another tensor.

Does not perform memory allocation internally

A Number of dimensions in ``begin`` and ``end`` must match number of dimensions in ``other.get_shape()``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- original tensor

	*
		- begin

		- start coordinate of ROI object inside of the original object.

	*
		- end

		- end coordinate of ROI object inside of the original object.

Methods
-------

.. _doxid-classov_1_1_tensor_1a83b0b800c932eca2a5e9d42dfdae655c:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor& operator = (const Tensor& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Tensor <doxid-classov_1_1_tensor>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-classov_1_1_tensor_1a3cf1d342fa056b59fd5bc38964d54575:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Tensor& operator = (Tensor&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Tensor <doxid-classov_1_1_tensor>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-classov_1_1_tensor_1a7a513a53ac7221d1a52006c34bce6c18:
.. index:: pair: function; set_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_shape(const :ref:`ov::Shape<doxid-classov_1_1_shape>`& shape)

Set new shape for tensor, deallocate/allocate if new total size is bigger than previous one.

Memory allocation may happen



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- shape

		- A new shape

.. _doxid-classov_1_1_tensor_1a7b00f757407bfee07d831647f15b1686:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`element::Type<doxid-classov_1_1element_1_1_type>` get_element_type() const



.. rubric:: Returns:

A tensor element type

.. _doxid-classov_1_1_tensor_1a706163e01fb555eb9ccdfb5204cf7834:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Shape<doxid-classov_1_1_shape>` get_shape() const



.. rubric:: Returns:

A tensor shape

.. _doxid-classov_1_1_tensor_1a26dfed6a65b46d9a25562e811912f09d:
.. index:: pair: function; get_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_size() const

Returns the total number of elements (a product of all the dims or 1 for scalar)



.. rubric:: Returns:

The total number of elements

.. _doxid-classov_1_1_tensor_1ae540fcafc1e9dc9181e86a1ec2682935:
.. index:: pair: function; get_byte_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_byte_size() const

Returns the size of the current :ref:`Tensor <doxid-classov_1_1_tensor>` in bytes.



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` 's size in bytes

.. _doxid-classov_1_1_tensor_1a610491239de68e700c7c3579479b6692:
.. index:: pair: function; get_strides

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Strides<doxid-classov_1_1_strides>` get_strides() const



.. rubric:: Returns:

:ref:`Tensor <doxid-classov_1_1_tensor>` 's strides in bytes

.. _doxid-classov_1_1_tensor_1ac1b8835f54d67d92969d7979e666e2a8:
.. index:: pair: function; data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void \* data(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type = {}) const

Provides an access to the underlaying host memory.

If type parameter is specified, the method throws an exception if specified type's fundamental type does not match with tensor element type's fundamental type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Optional type parameter.



.. rubric:: Returns:

A host pointer to tensor memory

.. _doxid-classov_1_1_tensor_1ae73e29ecaf40339a7b4f6b65cdde0736:
.. index:: pair: function; data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename datatype = typename std::decay<T>::type>
	T \* data() const

Provides an access to the underlaying host memory casted to type ``T``

Throws exception if specified type does not match with tensor element type



.. rubric:: Returns:

A host pointer to tensor memory casted to specified type ``T``.

.. _doxid-classov_1_1_tensor_1aa65688ce884468fdd9bd9cc24dda907a:
.. index:: pair: function; operator!

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator ! () const

Checks if current :ref:`Tensor <doxid-classov_1_1_tensor>` object is not initialized.



.. rubric:: Returns:

``true`` if current :ref:`Tensor <doxid-classov_1_1_tensor>` object is not initialized, ``false`` - otherwise

.. _doxid-classov_1_1_tensor_1a7ac03a96d3eeca3f057307bccb095df5:
.. index:: pair: function; operator bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator bool () const

Checks if current :ref:`Tensor <doxid-classov_1_1_tensor>` object is initialized.



.. rubric:: Returns:

``true`` if current :ref:`Tensor <doxid-classov_1_1_tensor>` object is initialized, ``false`` - otherwise

.. _doxid-classov_1_1_tensor_1a287c90f6c44793fd411e26490786c83d:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	std::enable_if<std::is_base_of<Tensor, T>::value, bool>::type is() const

Checks if the :ref:`Tensor <doxid-classov_1_1_tensor>` object can be cast to the type T.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to be checked. Must represent a class derived from the :ref:`Tensor <doxid-classov_1_1_tensor>`



.. rubric:: Returns:

true if this object can be dynamically cast to the type const T\*. Otherwise, false

.. _doxid-classov_1_1_tensor_1a345f8ade85da6fe30bcf8a3ae15a4bca:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	const std::enable_if<std::is_base_of<Tensor, T>::value, T>::type as() const

Casts this :ref:`Tensor <doxid-classov_1_1_tensor>` object to the type T.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to cast to. Must represent a class derived from the :ref:`Tensor <doxid-classov_1_1_tensor>`



.. rubric:: Returns:

T object

.. _doxid-classov_1_1_tensor_1a8beef8846cacaa542e3b51c061d50e42:
.. index:: pair: function; type_check

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void type_check(const Tensor& tensor)

Checks openvino tensor type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- a tensor which type will be checked

	*
		- :ref:`Exception <doxid-classov_1_1_exception>`

		- if type check with specified tensor is not pass


