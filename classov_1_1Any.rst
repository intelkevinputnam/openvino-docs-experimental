.. index:: pair: class; ov::Any
.. _doxid-classov_1_1_any:

class ov::Any
=============

.. toctree::
	:hidden:

	EqualityComparable <structov_1_1Any_1_1EqualityComparable.rst>
	HasBaseMemberType <structov_1_1Any_1_1HasBaseMemberType.rst>
	Impl <structov_1_1Any_1_1Impl.rst>
	TupleToTypeIndex <structov_1_1Any_1_1TupleToTypeIndex.rst>
	Base <classov_1_1Any_1_1Base.rst>

Overview
~~~~~~~~

This class represents an object to work with different types. :ref:`More...<details-classov_1_1_any>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <any.hpp>
	
	class Any
	{
	public:
		// structs
	
		template <typename T>
		struct :ref:`EqualityComparable<doxid-structov_1_1_any_1_1_equality_comparable>`;
		template <typename... T>
		struct :ref:`EqualityComparable<std::map<T...>><doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1map_3_01_t_8_8_8_01_4_01_4>`;
		template <typename... T>
		struct :ref:`EqualityComparable<std::vector<T...>><doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1vector_3_01_t_8_8_8_01_4_01_4>`;
		template <typename T>
		struct :ref:`HasBaseMemberType<doxid-structov_1_1_any_1_1_has_base_member_type>`;
		template <class T>
		struct :ref:`Impl<T, typename std::enable_if<!std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type><doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734>`;
		template <class T>
		struct :ref:`Impl<T, typename std::enable_if<std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type><doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1>`;
		template <class T, typename = void>
		struct :ref:`Impl<doxid-structov_1_1_any_1_1_impl>`;
		template <typename>
		struct :ref:`TupleToTypeIndex<doxid-structov_1_1_any_1_1_tuple_to_type_index>`;
		template <typename... Args>
		struct :ref:`TupleToTypeIndex<std::tuple<Args...>><doxid-structov_1_1_any_1_1_tuple_to_type_index_3_01std_1_1tuple_3_01_args_8_8_8_01_4_01_4>`;

		// classes
	
		class :ref:`Base<doxid-classov_1_1_any_1_1_base>`;

		// construction
	
		:ref:`Any<doxid-classov_1_1_any_1af46a3c7301722699280ce36c105ad44c>`();
		:ref:`Any<doxid-classov_1_1_any_1aa89a38526c238c62f29a4bf06e1c5ec8>`(const Any& other);
		:ref:`Any<doxid-classov_1_1_any_1a557fcd30ec56bc3de914573b35d15b84>`(Any&& other);
	
		template <
			typename T,
			typename std::enable_if<!std::is_same<decay_t<T>, Any>::value&&!std::is_abstract<decay_t<T>>::value&&!std::is_convertible<decay_t<T>, Base::Ptr>::value, bool>::type = true
			>
		:ref:`Any<doxid-classov_1_1_any_1ab07ee67eba0df8a784039f7f7e8c7215>`(T&& value);
	
		:ref:`Any<doxid-classov_1_1_any_1ae49826c8cec0a93bd3a0a218c1073079>`(const char \* str);
		:ref:`Any<doxid-classov_1_1_any_1a371f13d1bdae1f7a59ecbc454de20828>`(const std::nullptr_t);

		// methods
	
		Any& :ref:`operator =<doxid-classov_1_1_any_1a5aafe87b995305bd85cf09a6fd0abc23>` (const Any& other);
		Any& :ref:`operator =<doxid-classov_1_1_any_1a21c69ac02dd6c3d84d35c2a9f59621ef>` (Any&& other);
		const std::type_info& :ref:`type_info<doxid-classov_1_1_any_1af20e9533580ddff213aee7a2c2f15a24>`() const;
		bool :ref:`empty<doxid-classov_1_1_any_1a1ad8e0eb4f857a99e2ba57dfcaf08673>`() const;
	
		template <class T>
		bool :ref:`is<doxid-classov_1_1_any_1a004db3f93298b5735afe156b9a6490ce>`() const;
	
		template <class T>
		std::enable_if<std::is_convertible<T, std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`>>::value, T>::type& :ref:`as<doxid-classov_1_1_any_1a072cf1e9202ba31bd91ebd479488703c>`();
	
		template <class T>
		std::enable_if<!std::is_convertible<T, std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`>>::value&&!std::is_same<T, std::string>::value&&std::is_default_constructible<T>::value&&(util::Istreamable<T>::value||util::Readable<T>::value), T>::type& :ref:`as<doxid-classov_1_1_any_1a47fb76a9a6b2ebb3a337bd28fd58233b>`();
	
		template <class T>
		std::enable_if<!std::is_convertible<T, std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`>>::value&&!std::is_same<T, std::string>::value&&(!std::is_default_constructible<T>::value||(!util::Istreamable<T>::value&&!util::Readable<T>::value)), T>::type& :ref:`as<doxid-classov_1_1_any_1abca7ca9cc2a65334542ae499c10eba22>`();
	
		template <class T>
		std::enable_if<std::is_same<T, std::string>::value, T>::type& :ref:`as<doxid-classov_1_1_any_1a97ce1d254630e010d868320a26e8a915>`();
	
		template <class T>
		const T& :ref:`as<doxid-classov_1_1_any_1a64a2c4cd070f1034001f354e584c2280>`() const;
	
		template <typename T>
		:ref:`operator T&<doxid-classov_1_1_any_1aa56a0d0f39af9bb0d303117579918c0c>` ();
	
		template <typename T>
		:ref:`operator const T &<doxid-classov_1_1_any_1aa1896d2ab2f6cc6ed556b694aaafceaa>` () const;
	
		template <typename T>
		:ref:`operator T&<doxid-classov_1_1_any_1a20a4ea150e8096046df754a9a0afbd17>` () const;
	
		bool :ref:`operator ==<doxid-classov_1_1_any_1aac7fa257c998408f1a2018f34dfd93ee>` (const Any& other) const;
		bool :ref:`operator ==<doxid-classov_1_1_any_1a3ee2e37ac97549999e9312e7d18b4254>` (const std::nullptr_t&) const;
		bool :ref:`operator !=<doxid-classov_1_1_any_1af9cf12ee882baa3933293905f6e12928>` (const Any& other) const;
		Base \* :ref:`operator -><doxid-classov_1_1_any_1a932810966339875065190a0765c9a298>` ();
		const Base \* :ref:`operator -><doxid-classov_1_1_any_1a9c8303c41c1edfeeb64606672abf8bd4>` () const;
		void :ref:`print<doxid-classov_1_1_any_1a8a6ea9926553ce4022146ebe644e9024>`(std::ostream& stream) const;
		void :ref:`read<doxid-classov_1_1_any_1aafe927701e6e3ac927d2eedb90ef235b>`(std::istream& stream);
		Base \* :ref:`get<doxid-classov_1_1_any_1ab13ba33d92154fdbdc049c9c65eca20b>`();
		const Base \* :ref:`get<doxid-classov_1_1_any_1a6245b5256802d838ca8393e7b9268b34>`() const;
		void \* :ref:`addressof<doxid-classov_1_1_any_1ad56d3b8df151800b57cc4bd8c63527d4>`();
		const void \* :ref:`addressof<doxid-classov_1_1_any_1a4a7a330d4958ad7f6dd208bbeddd295b>`() const;
	
		template <typename T, typename... Args>
		static Any :ref:`make<doxid-classov_1_1_any_1aa3eb822d813dd392cda96829c0468872>`(Args&&... args);
	};
.. _details-classov_1_1_any:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an object to work with different types.

Construction
------------

.. _doxid-classov_1_1_any_1af46a3c7301722699280ce36c105ad44c:
.. index:: pair: function; Any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any()

Default constructor.

.. _doxid-classov_1_1_any_1aa89a38526c238c62f29a4bf06e1c5ec8:
.. index:: pair: function; Any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any(const Any& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Any <doxid-classov_1_1_any>` object

.. _doxid-classov_1_1_any_1a557fcd30ec56bc3de914573b35d15b84:
.. index:: pair: function; Any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any(Any&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Any <doxid-classov_1_1_any>` object

.. _doxid-classov_1_1_any_1ab07ee67eba0df8a784039f7f7e8c7215:
.. index:: pair: function; Any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_same<decay_t<T>, Any>::value&&!std::is_abstract<decay_t<T>>::value&&!std::is_convertible<decay_t<T>, Base::Ptr>::value, bool>::type = true
		>
	Any(T&& value)

Constructor creates any with object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- :ref:`Any <doxid-classov_1_1_any>` type

	*
		- value

		- object

.. _doxid-classov_1_1_any_1ae49826c8cec0a93bd3a0a218c1073079:
.. index:: pair: function; Any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any(const char \* str)

Constructor creates string any from char \*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- str

		- char array

.. _doxid-classov_1_1_any_1a371f13d1bdae1f7a59ecbc454de20828:
.. index:: pair: function; Any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any(const std::nullptr_t)

Empty constructor.

Methods
-------

.. _doxid-classov_1_1_any_1a5aafe87b995305bd85cf09a6fd0abc23:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any& operator = (const Any& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Any <doxid-classov_1_1_any>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-classov_1_1_any_1a21c69ac02dd6c3d84d35c2a9f59621ef:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Any& operator = (Any&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- other :ref:`Any <doxid-classov_1_1_any>` object



.. rubric:: Returns:

reference to the current object

.. _doxid-classov_1_1_any_1af20e9533580ddff213aee7a2c2f15a24:
.. index:: pair: function; type_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::type_info& type_info() const

Returns type info



.. rubric:: Returns:

type info

.. _doxid-classov_1_1_any_1a1ad8e0eb4f857a99e2ba57dfcaf08673:
.. index:: pair: function; empty

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool empty() const

Checks that any contains a value



.. rubric:: Returns:

false if any contains a value else false

.. _doxid-classov_1_1_any_1a004db3f93298b5735afe156b9a6490ce:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	bool is() const

Check that stored type can be casted to specified type. If internal type supports Base.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type of value



.. rubric:: Returns:

true if type of value is correct. Return false if any is empty

.. _doxid-classov_1_1_any_1a072cf1e9202ba31bd91ebd479488703c:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	std::enable_if<std::is_convertible<T, std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`>>::value, T>::type& as()

Dynamic cast to specified type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1a47fb76a9a6b2ebb3a337bd28fd58233b:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	std::enable_if<!std::is_convertible<T, std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`>>::value&&!std::is_same<T, std::string>::value&&std::is_default_constructible<T>::value&&(util::Istreamable<T>::value||util::Readable<T>::value), T>::type& as()

Dynamic cast to specified type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1abca7ca9cc2a65334542ae499c10eba22:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	std::enable_if<!std::is_convertible<T, std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`>>::value&&!std::is_same<T, std::string>::value&&(!std::is_default_constructible<T>::value||(!util::Istreamable<T>::value&&!util::Readable<T>::value)), T>::type& as()

Dynamic cast to specified type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1a97ce1d254630e010d868320a26e8a915:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	std::enable_if<std::is_same<T, std::string>::value, T>::type& as()

Dynamic cast to specified type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1a64a2c4cd070f1034001f354e584c2280:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	const T& as() const

Dynamic cast to specified type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

const reference to caster object

.. _doxid-classov_1_1_any_1aa56a0d0f39af9bb0d303117579918c0c:
.. index:: pair: function; operator T&

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	operator T& ()

Converts to specified type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1aa1896d2ab2f6cc6ed556b694aaafceaa:
.. index:: pair: function; operator const T &

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	operator const T & () const

Converts to specified type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1a20a4ea150e8096046df754a9a0afbd17:
.. index:: pair: function; operator T&

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	operator T& () const

Converts to specified type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type



.. rubric:: Returns:

casted object

.. _doxid-classov_1_1_any_1aac7fa257c998408f1a2018f34dfd93ee:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const Any& other) const

The comparison operator for the :ref:`Any <doxid-classov_1_1_any>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- object to compare



.. rubric:: Returns:

true if objects are equal

.. _doxid-classov_1_1_any_1a3ee2e37ac97549999e9312e7d18b4254:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const std::nullptr_t&) const

The comparison operator for the :ref:`Any <doxid-classov_1_1_any>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- object to compare



.. rubric:: Returns:

true if objects are equal

.. _doxid-classov_1_1_any_1af9cf12ee882baa3933293905f6e12928:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const Any& other) const

The comparison operator for the :ref:`Any <doxid-classov_1_1_any>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- object to compare



.. rubric:: Returns:

true if objects aren't equal

.. _doxid-classov_1_1_any_1a932810966339875065190a0765c9a298:
.. index:: pair: function; operator->

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Base \* operator -> ()

Standard pointer operator.



.. rubric:: Returns:

underlined interface

.. _doxid-classov_1_1_any_1a9c8303c41c1edfeeb64606672abf8bd4:
.. index:: pair: function; operator->

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const Base \* operator -> () const

Standard pointer operator.



.. rubric:: Returns:

underlined interface

.. _doxid-classov_1_1_any_1a8a6ea9926553ce4022146ebe644e9024:
.. index:: pair: function; print

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void print(std::ostream& stream) const

Prints underlying object to the given output stream. Uses operator<< if it is defined, leaves stream unchanged otherwise. In case of empty any or nullptr stream immediately returns.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- stream

		- :ref:`Output <doxid-classov_1_1_output>` stream object will be printed to.

.. _doxid-classov_1_1_any_1aafe927701e6e3ac927d2eedb90ef235b:
.. index:: pair: function; read

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void read(std::istream& stream)

Read into underlying object from the given input stream. Uses operator>> if it is defined, leaves stream unchanged otherwise. In case of empty any or nullptr stream immediately returns.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- stream

		- :ref:`Output <doxid-classov_1_1_output>` stream object will be printed to.

.. _doxid-classov_1_1_any_1ab13ba33d92154fdbdc049c9c65eca20b:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Base \* get()

Return pointer to underlined interface.



.. rubric:: Returns:

underlined interface

.. _doxid-classov_1_1_any_1a6245b5256802d838ca8393e7b9268b34:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const Base \* get() const

Return pointer to underlined interface.



.. rubric:: Returns:

underlined interface

.. _doxid-classov_1_1_any_1ad56d3b8df151800b57cc4bd8c63527d4:
.. index:: pair: function; addressof

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void \* addressof()

Returns address to internal value if any is not empty and ``nullptr`` instead.



.. rubric:: Returns:

address to internal stored value

.. _doxid-classov_1_1_any_1a4a7a330d4958ad7f6dd208bbeddd295b:
.. index:: pair: function; addressof

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const void \* addressof() const

Returns address to internal value if any is not empty and ``nullptr`` instead.



.. rubric:: Returns:

address to internal stored value

.. _doxid-classov_1_1_any_1aa3eb822d813dd392cda96829c0468872:
.. index:: pair: function; make

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename... Args>
	static Any make(Args&&... args)

Inplace value construction function.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- :ref:`Any <doxid-classov_1_1_any>` type

	*
		- Args

		- pack of paramter types passed to T constructor

	*
		- args

		- pack of paramters passed to T constructor


