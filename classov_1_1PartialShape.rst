.. index:: pair: class; ov::PartialShape
.. _doxid-classov_1_1_partial_shape:

class ov::PartialShape
======================



Overview
~~~~~~~~

Class representing a shape that may be partially or totally dynamic. :ref:`More...<details-classov_1_1_partial_shape>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <partial_shape.hpp>
	
	class PartialShape
	{
	public:
		// typedefs
	
		typedef Dimensions::iterator :target:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>`;
		typedef Dimensions::const_iterator :target:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>`;
		typedef Dimensions::reverse_iterator :target:`reverse_iterator<doxid-classov_1_1_partial_shape_1a6c82ffcb274c7ff68c714a8794071b3d>`;
		typedef Dimensions::const_reverse_iterator :target:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>`;

		// construction
	
		:ref:`PartialShape<doxid-classov_1_1_partial_shape_1a165fc9d95b5fb8fd18c09eae2e4762d2>`(std::initializer_list<:ref:`Dimension<doxid-classov_1_1_dimension>`> init);
		:ref:`PartialShape<doxid-classov_1_1_partial_shape_1ad76d4e197bd917f562fe264cb43cfbae>`(std::vector<:ref:`Dimension<doxid-classov_1_1_dimension>`> dimensions);
		:ref:`PartialShape<doxid-classov_1_1_partial_shape_1ae13e01620ffdad68f7ef994065f3a37e>`(const std::vector<:ref:`Dimension::value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>`>& dimensions);
		:ref:`PartialShape<doxid-classov_1_1_partial_shape_1aabe0312d22f9adc7036243da04b6ca82>`();
		:ref:`PartialShape<doxid-classov_1_1_partial_shape_1a9b5dbaeeb71d9d79fe1d3e639986faef>`(const :ref:`Shape<doxid-classov_1_1_shape>`& shape);

		// methods
	
		bool :ref:`is_static<doxid-classov_1_1_partial_shape_1ab022cd7a21aaae32919fd4e8b45bc8ad>`() const;
		bool :ref:`is_dynamic<doxid-classov_1_1_partial_shape_1a3c2f6e07a5415648ce1654831d6be035>`() const;
		:ref:`Rank<doxid-namespaceov_1a9e276f26decce686824844ce1c0a8993>` :ref:`rank<doxid-classov_1_1_partial_shape_1ab7a005146d7cf002f8ae5bd0e1921be5>`() const;
		bool :ref:`compatible<doxid-classov_1_1_partial_shape_1ac19392ad73930bdd1f03bf9ee28bc7cd>`(const PartialShape& s) const;
		bool :ref:`same_scheme<doxid-classov_1_1_partial_shape_1a2db6f42afc3a7826551b064608ed3f0a>`(const PartialShape& s) const;
		bool :ref:`relaxes<doxid-classov_1_1_partial_shape_1a47fb714957085d01646bb633344c16f4>`(const PartialShape& s) const;
		bool :ref:`refines<doxid-classov_1_1_partial_shape_1a44f771b339b315adbd52cdc4d99dfa78>`(const PartialShape& s) const;
		bool :ref:`merge_rank<doxid-classov_1_1_partial_shape_1a62a81b393eef8277c55c9c7fe5606b23>`(:ref:`Rank<doxid-namespaceov_1a9e276f26decce686824844ce1c0a8993>` r);
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`to_shape<doxid-classov_1_1_partial_shape_1a86a51bf8e243bb4f5552e23d5d1beb34>`() const;
		bool :ref:`all_non_negative<doxid-classov_1_1_partial_shape_1a5a1812cd0054e14e64eb9ac4ee614258>`() const;
		const :ref:`Dimension<doxid-classov_1_1_dimension>`& :ref:`operator []<doxid-classov_1_1_partial_shape_1a6f76f07d4e2f34c3c0084e889d62c815>` (size_t i) const;
		:ref:`Dimension<doxid-classov_1_1_dimension>`& :ref:`operator []<doxid-classov_1_1_partial_shape_1a1dec3ecf9e65fbe5b1837c50905af2de>` (size_t i);
		:ref:`operator std::vector< Dimension ><doxid-classov_1_1_partial_shape_1ac587e68cfd4e870d3e32998e233edb4b>` () const;
		bool :target:`operator ==<doxid-classov_1_1_partial_shape_1a91a77fc1f03aa86edf59ca397139b66e>` (const PartialShape& partial_shape) const;
		bool :target:`operator !=<doxid-classov_1_1_partial_shape_1adffa7c98ac2b81c3d7a428c7ebeae926>` (const PartialShape& partial_shape) const;
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`get_max_shape<doxid-classov_1_1_partial_shape_1a54130814ffbb4e6a4b1783ef539e64b0>`() const;
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`get_min_shape<doxid-classov_1_1_partial_shape_1a6985e6d7d149ae14e9cafc9a33fc41a3>`() const;
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`get_shape<doxid-classov_1_1_partial_shape_1a7973b448c76e208993190d2e1e5d7a4a>`() const;
		:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` :ref:`begin<doxid-classov_1_1_partial_shape_1aaae6030dc8b488f83b9cea97943dfc93>`();
		:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` :ref:`begin<doxid-classov_1_1_partial_shape_1a86572f67c8e69df6f00bae2580760ca2>`() const;
		:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` :ref:`end<doxid-classov_1_1_partial_shape_1ae6c88087ba1949f44a3301e7c4a5f9f9>`();
		:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` :ref:`end<doxid-classov_1_1_partial_shape_1a121aba44feedf4f9e6c294f168ba2379>`() const;
		:ref:`reverse_iterator<doxid-classov_1_1_partial_shape_1a6c82ffcb274c7ff68c714a8794071b3d>` :ref:`rbegin<doxid-classov_1_1_partial_shape_1a59e51ca3222328a2db5f8beff413c105>`();
		:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` :ref:`rbegin<doxid-classov_1_1_partial_shape_1ae0ce11b5db538d49e3bc118546a0bce0>`() const;
		:ref:`reverse_iterator<doxid-classov_1_1_partial_shape_1a6c82ffcb274c7ff68c714a8794071b3d>` :ref:`rend<doxid-classov_1_1_partial_shape_1a99d0ffdb0e27200716a4777929512178>`();
		:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` :ref:`rend<doxid-classov_1_1_partial_shape_1af44e33afa75694cbfe08aa2263aca533>`() const;
		:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` :ref:`cbegin<doxid-classov_1_1_partial_shape_1a968e1c462a907b8d61698771ef83d29e>`() const;
		:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` :ref:`cend<doxid-classov_1_1_partial_shape_1a3b9c9a9772a3e5337058cff468901049>`() const;
		:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` :ref:`crbegin<doxid-classov_1_1_partial_shape_1a6b9b1f94b554ecfe0a6398cc9464d9ba>`() const;
		:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` :ref:`crend<doxid-classov_1_1_partial_shape_1a74e7efddfabc60291dbeb227e1ad91d8>`() const;
		void :ref:`resize<doxid-classov_1_1_partial_shape_1a8a3a03bf6a2b89b5ba82b81b4fb931a7>`(size_t count);
		size_t :ref:`size<doxid-classov_1_1_partial_shape_1a3eca1b293998bed6c1cb0ea3d89a5434>`() const;
		:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` :ref:`insert<doxid-classov_1_1_partial_shape_1a6312690123f57bb9a912f6c086130cfd>`(:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` position, const :ref:`Dimension<doxid-classov_1_1_dimension>`& val);
		void :ref:`insert<doxid-classov_1_1_partial_shape_1a62c14043ff4a7dba75b199d41ddd7d3a>`(:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` position, size_t n, const :ref:`Dimension<doxid-classov_1_1_dimension>`& val);
	
		template <class InputIterator>
		void :ref:`insert<doxid-classov_1_1_partial_shape_1ad40f2f8d29ee0c8648b1bc4b1e828664>`(
			:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` position,
			InputIterator first,
			InputIterator last
			);
	
		void :ref:`reserve<doxid-classov_1_1_partial_shape_1a6f742eef340b8c0e06846aca431aa812>`(size_t n);
		void :ref:`push_back<doxid-classov_1_1_partial_shape_1afa7b5490e0d87e2c9bc8431320d07dc9>`(const :ref:`Dimension<doxid-classov_1_1_dimension>`& val);
		static PartialShape :ref:`dynamic<doxid-classov_1_1_partial_shape_1a5f8ce4b26f65232d9de8ab4e5e3b375d>`(:ref:`Rank<doxid-namespaceov_1a9e276f26decce686824844ce1c0a8993>` r = Rank::dynamic());
		static bool :ref:`merge_into<doxid-classov_1_1_partial_shape_1a471e7d43a8de59e4c019ee638ab10d83>`(PartialShape& dst, const PartialShape& src);
	
		static bool :ref:`broadcast_merge_into<doxid-classov_1_1_partial_shape_1a9c35fc751bc2479087ea2f2754ab29e7>`(
			PartialShape& dst,
			const PartialShape& src,
			const :ref:`ov::op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob
			);
	};
.. _details-classov_1_1_partial_shape:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class representing a shape that may be partially or totally dynamic.

A :ref:`PartialShape <doxid-classov_1_1_partial_shape>` may have:

* Dynamic rank. (Informal notation: ``?``)

* Static rank, but dynamic dimensions on some or all axes. (Informal notation examples: ``{1,2,?,4}``, ``{?,?,?}``)

* Static rank, and static dimensions on all axes. (Informal notation examples: ``{1,2,3,4}``, ``{6}``, ``{}``)

Construction
------------

.. _doxid-classov_1_1_partial_shape_1a165fc9d95b5fb8fd18c09eae2e4762d2:
.. index:: pair: function; PartialShape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PartialShape(std::initializer_list<:ref:`Dimension<doxid-classov_1_1_dimension>`> init)

Constructs a shape with static rank from an initializer list of :ref:`Dimension <doxid-classov_1_1_dimension>`.

Examples:

.. ref-code-block:: cpp

	:ref:`PartialShape <doxid-classov_1_1_partial_shape_1aabe0312d22f9adc7036243da04b6ca82>` :ref:`s <doxid-ie__preprocess__gapi_8cpp_1afc7998e50661eed237070df8aab0f2d6>`{2,3,4};                     // rank=3, all dimensions static
	:ref:`PartialShape <doxid-classov_1_1_partial_shape_1aabe0312d22f9adc7036243da04b6ca82>` :ref:`s <doxid-ie__preprocess__gapi_8cpp_1afc7998e50661eed237070df8aab0f2d6>`{};                          // rank=0
	:ref:`PartialShape <doxid-classov_1_1_partial_shape_1aabe0312d22f9adc7036243da04b6ca82>` :ref:`s <doxid-ie__preprocess__gapi_8cpp_1afc7998e50661eed237070df8aab0f2d6>`{2,:ref:`Dimension::dynamic <doxid-classov_1_1_dimension_1ae20d6e04468016921fc572308c712a20>`(),3};  // rank=3, dimension 1 dynamic



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- init

		- The :ref:`Dimension <doxid-classov_1_1_dimension>` values for the constructed shape.

.. _doxid-classov_1_1_partial_shape_1ad76d4e197bd917f562fe264cb43cfbae:
.. index:: pair: function; PartialShape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PartialShape(std::vector<:ref:`Dimension<doxid-classov_1_1_dimension>`> dimensions)

Constructs a :ref:`PartialShape <doxid-classov_1_1_partial_shape>` with static rank from a vector of :ref:`Dimension <doxid-classov_1_1_dimension>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dimensions

		- The :ref:`Dimension <doxid-classov_1_1_dimension>` values for the constructed shape.

.. _doxid-classov_1_1_partial_shape_1ae13e01620ffdad68f7ef994065f3a37e:
.. index:: pair: function; PartialShape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PartialShape(const std::vector<:ref:`Dimension::value_type<doxid-classov_1_1_dimension_1a76095c1e86db6498ac945c1ddd8b7b44>`>& dimensions)

Constructs a :ref:`PartialShape <doxid-classov_1_1_partial_shape>` with static rank from a vector of dimensions values.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dimensions

		- The :ref:`Dimension <doxid-classov_1_1_dimension>` values for the constructed shape.

.. _doxid-classov_1_1_partial_shape_1aabe0312d22f9adc7036243da04b6ca82:
.. index:: pair: function; PartialShape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PartialShape()

Constructs a static :ref:`PartialShape <doxid-classov_1_1_partial_shape>` with zero rank (the shape of a scalar).

.. _doxid-classov_1_1_partial_shape_1a9b5dbaeeb71d9d79fe1d3e639986faef:
.. index:: pair: function; PartialShape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PartialShape(const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

Constructs a static :ref:`PartialShape <doxid-classov_1_1_partial_shape>` from a :ref:`PartialShape <doxid-classov_1_1_partial_shape>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- shape

		- The :ref:`PartialShape <doxid-classov_1_1_partial_shape>` to convert into :ref:`PartialShape <doxid-classov_1_1_partial_shape>`.

Methods
-------

.. _doxid-classov_1_1_partial_shape_1ab022cd7a21aaae32919fd4e8b45bc8ad:
.. index:: pair: function; is_static

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_static() const

Check if this shape is static.

A shape is considered static if it has static rank, and all dimensions of the shape are static.



.. rubric:: Returns:

``true`` if this shape is static, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a3c2f6e07a5415648ce1654831d6be035:
.. index:: pair: function; is_dynamic

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_dynamic() const

Check if this shape is dynamic.

A shape is considered static if it has static rank, and all dimensions of the shape are static.



.. rubric:: Returns:

``false`` if this shape is static, else ``true``.

.. _doxid-classov_1_1_partial_shape_1ab7a005146d7cf002f8ae5bd0e1921be5:
.. index:: pair: function; rank

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Rank<doxid-namespaceov_1a9e276f26decce686824844ce1c0a8993>` rank() const

Get the rank of the shape.



.. rubric:: Returns:

The rank of the shape. This will be :ref:`Rank::dynamic() <doxid-classov_1_1_dimension_1ae20d6e04468016921fc572308c712a20>` if the rank of the shape is dynamic.

.. _doxid-classov_1_1_partial_shape_1ac19392ad73930bdd1f03bf9ee28bc7cd:
.. index:: pair: function; compatible

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool compatible(const PartialShape& s) const

Check whether this shape is compatible with the argument, i.e., whether it is possible to merge them.

Two shapes are compatible if

* one or both of them has dynamic rank, or

* both shapes have dynamic and equal rank, and their dimensions are elementwise compatible (see :ref:`Dimension::compatible() <doxid-classov_1_1_dimension_1a930fe268cb5c954ac8696c97a974ca5b>`).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- The shape to be checked for compatibility with this shape.



.. rubric:: Returns:

``true`` if this shape is compatible with ``s``, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a2db6f42afc3a7826551b064608ed3f0a:
.. index:: pair: function; same_scheme

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool same_scheme(const PartialShape& s) const

Check whether this shape represents the same scheme as the argument.

Two shapes ``s1`` and ``s2`` represent the same scheme if

* they both have dynamic rank, or

* they both have static and equal rank ``r``, and for every ``i`` from ``0`` to ``r-1``, ``s1[i]`` represents the same scheme as ``s2[i]`` (see :ref:`Dimension::same_scheme() <doxid-classov_1_1_dimension_1a8a463f7fdc62f36e22317d11b43d9f4c>`).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- The shape whose scheme is being compared with this shape.



.. rubric:: Returns:

``true`` if this shape represents the same scheme as ``s``, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a47fb714957085d01646bb633344c16f4:
.. index:: pair: function; relaxes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool relaxes(const PartialShape& s) const

Check whether this shape is a relaxation of the argument.

Intuitively, a :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s1`` is said to *relax* ``s2`` (or *is a relaxation* of ``s2``) if it is "more permissive" than ``s2``. In other words, ``s1`` is a relaxation of ``s2`` if anything you can form by plugging things into the dynamic dimensions of ``s2`` is also something you can form by plugging things into the dynamic dimensions of ``s1``, but not necessarily the other way around.

``s1.relaxes(s2)`` is equivalent to ``s2.refines(s1)``.

Formally, :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s1`` is said to *relax* :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s2`` if:

* For every ``i`` from ``0`` to ``r-1``, either ``s1[i]`` contains s2[i].



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- The shape which is being compared against this shape.



.. rubric:: Returns:

``true`` if this shape relaxes ``s``, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a44f771b339b315adbd52cdc4d99dfa78:
.. index:: pair: function; refines

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool refines(const PartialShape& s) const

Check whether this shape is a refinement of the argument.

Intuitively, a :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s1`` is said to *relax* ``s2`` (or *is a relaxation* of ``s2``) if it is "less permissive" than ``s2``. In other words, ``s1`` is a relaxation of ``s2`` if anything you can form by plugging things into the dynamic dimensions of ``s1`` is also something you can form by plugging things into the dynamic dimensions of ``s2``, but not necessarily the other way around.

``s1.refines(s2)`` is equivalent to ``s2.relaxes(s1)``.

Formally, :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s1`` is said to *refine* :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s2`` if:

* ``s2`` has dynamic rank, or

* ``s1`` and ``s2`` both have static rank ``r``, and for every ``i`` from ``0`` to ``r-1``, either ``s2[i]`` is dynamic, or ``s1[i]`` == ``s2[i]``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- The shape which is being compared against this shape.



.. rubric:: Returns:

``true`` if this shape refines ``s``, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a62a81b393eef8277c55c9c7fe5606b23:
.. index:: pair: function; merge_rank

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool merge_rank(:ref:`Rank<doxid-namespaceov_1a9e276f26decce686824844ce1c0a8993>` r)

Checks that this shape's rank is compatible with ``r``, and, if this shape's rank is dynamic and ``r`` is static, updates this shape to have a rank of ``r`` with dimensions all dynamic.



.. rubric:: Returns:

``true`` if this shape's rank is compatible with ``r``, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a86a51bf8e243bb4f5552e23d5d1beb34:
.. index:: pair: function; to_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Shape<doxid-classov_1_1_shape>` to_shape() const

Convert a static :ref:`PartialShape <doxid-classov_1_1_partial_shape>` to a :ref:`PartialShape <doxid-classov_1_1_partial_shape>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::invalid_argument

		- If this :ref:`PartialShape <doxid-classov_1_1_partial_shape>` is dynamic.



.. rubric:: Returns:

A new :ref:`PartialShape <doxid-classov_1_1_partial_shape>` ``s`` where ``s[i] = size_t((\*this)[i])``.

.. _doxid-classov_1_1_partial_shape_1a5a1812cd0054e14e64eb9ac4ee614258:
.. index:: pair: function; all_non_negative

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool all_non_negative() const

Returns ``true`` if all static dimensions of the tensor are non-negative, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a6f76f07d4e2f34c3c0084e889d62c815:
.. index:: pair: function; operator[]

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Dimension<doxid-classov_1_1_dimension>`& operator [] (size_t i) const

Index operator for :ref:`PartialShape <doxid-classov_1_1_partial_shape>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- i

		- The index of the dimension being selected.



.. rubric:: Returns:

A reference to the ``i`` th :ref:`Dimension <doxid-classov_1_1_dimension>` of this shape.

.. _doxid-classov_1_1_partial_shape_1a1dec3ecf9e65fbe5b1837c50905af2de:
.. index:: pair: function; operator[]

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Dimension<doxid-classov_1_1_dimension>`& operator [] (size_t i)

Index operator for :ref:`PartialShape <doxid-classov_1_1_partial_shape>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- i

		- The index of the dimension being selected.



.. rubric:: Returns:

A reference to the ``i`` th :ref:`Dimension <doxid-classov_1_1_dimension>` of this shape.

.. _doxid-classov_1_1_partial_shape_1ac587e68cfd4e870d3e32998e233edb4b:
.. index:: pair: function; operator std::vector< Dimension >

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator std::vector< Dimension > () const

Returns a vector of the dimensions. This has no meaning if dynamic.

.. _doxid-classov_1_1_partial_shape_1a54130814ffbb4e6a4b1783ef539e64b0:
.. index:: pair: function; get_max_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Shape<doxid-classov_1_1_shape>` get_max_shape() const

Get the max bounding shape.

.. _doxid-classov_1_1_partial_shape_1a6985e6d7d149ae14e9cafc9a33fc41a3:
.. index:: pair: function; get_min_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Shape<doxid-classov_1_1_shape>` get_min_shape() const

Get the min bounding shape.

.. _doxid-classov_1_1_partial_shape_1a7973b448c76e208993190d2e1e5d7a4a:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Shape<doxid-classov_1_1_shape>` get_shape() const

Get the unique shape.

.. _doxid-classov_1_1_partial_shape_1aaae6030dc8b488f83b9cea97943dfc93:
.. index:: pair: function; begin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` begin()

Returns a read/write iterator that points to the first element in the shape. Iteration is done in ordinary element order.

.. _doxid-classov_1_1_partial_shape_1a86572f67c8e69df6f00bae2580760ca2:
.. index:: pair: function; begin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` begin() const

Returns a read-only (constant) iterator that points to the first element in the shape. Iteration is done in ordinary element order.

.. _doxid-classov_1_1_partial_shape_1ae6c88087ba1949f44a3301e7c4a5f9f9:
.. index:: pair: function; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` end()

Returns a read/write iterator that points one past the last element in the shape. Iteration is done in ordinary element order.

.. _doxid-classov_1_1_partial_shape_1a121aba44feedf4f9e6c294f168ba2379:
.. index:: pair: function; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` end() const

Returns a read-only (constant) iterator that points one past the last element in the shape. Iteration is done in ordinary element order.

.. _doxid-classov_1_1_partial_shape_1a59e51ca3222328a2db5f8beff413c105:
.. index:: pair: function; rbegin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`reverse_iterator<doxid-classov_1_1_partial_shape_1a6c82ffcb274c7ff68c714a8794071b3d>` rbegin()

Returns a read/write reverse iterator that points to the last element in the shape. Iteration is done in reverse element order.

.. _doxid-classov_1_1_partial_shape_1ae0ce11b5db538d49e3bc118546a0bce0:
.. index:: pair: function; rbegin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` rbegin() const

Returns a read-only (constant) reverse iterator that points to the last element in the shape. Iteration is done in reverse element order.

.. _doxid-classov_1_1_partial_shape_1a99d0ffdb0e27200716a4777929512178:
.. index:: pair: function; rend

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`reverse_iterator<doxid-classov_1_1_partial_shape_1a6c82ffcb274c7ff68c714a8794071b3d>` rend()

Returns a read/write reverse iterator that points to one before the first element in the shape. Iteration is done in reverse element order.

.. _doxid-classov_1_1_partial_shape_1af44e33afa75694cbfe08aa2263aca533:
.. index:: pair: function; rend

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` rend() const

Returns a read-only (constant) reverse iterator that points to one before the first element in the shape. Iteration is done in reverse element order.

.. _doxid-classov_1_1_partial_shape_1a968e1c462a907b8d61698771ef83d29e:
.. index:: pair: function; cbegin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` cbegin() const

Returns a read-only (constant) iterator that points to the first element in the shape. Iteration is done in ordinary element order.

.. _doxid-classov_1_1_partial_shape_1a3b9c9a9772a3e5337058cff468901049:
.. index:: pair: function; cend

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_iterator<doxid-classov_1_1_partial_shape_1aef3881735e00d9cd967ece17b2a385e0>` cend() const

Returns a read-only (constant) iterator that points one past the last element in the shape. Iteration is done in ordinary element order.

.. _doxid-classov_1_1_partial_shape_1a6b9b1f94b554ecfe0a6398cc9464d9ba:
.. index:: pair: function; crbegin

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` crbegin() const

Returns a read-only (constant) reverse iterator that points to the last element in the shape. Iteration is done in reverse element order.

.. _doxid-classov_1_1_partial_shape_1a74e7efddfabc60291dbeb227e1ad91d8:
.. index:: pair: function; crend

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`const_reverse_iterator<doxid-classov_1_1_partial_shape_1a6b22f48500468c0a1079a355e5492453>` crend() const

Returns a read-only (constant) reverse iterator that points to one before the first element in the shape. Iteration is done in reverse element order.

.. _doxid-classov_1_1_partial_shape_1a8a3a03bf6a2b89b5ba82b81b4fb931a7:
.. index:: pair: function; resize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void resize(size_t count)

Resizes dimensions container to contain count elements.

.. _doxid-classov_1_1_partial_shape_1a3eca1b293998bed6c1cb0ea3d89a5434:
.. index:: pair: function; size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t size() const

Returns size of dimension vector. Requires rank to be static.

.. _doxid-classov_1_1_partial_shape_1a6312690123f57bb9a912f6c086130cfd:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` insert(:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` position, const :ref:`Dimension<doxid-classov_1_1_dimension>`& val)

Returns a read/write iterator that points to the inserted element in the shape.

.. _doxid-classov_1_1_partial_shape_1a62c14043ff4a7dba75b199d41ddd7d3a:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void insert(:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` position, size_t n, const :ref:`Dimension<doxid-classov_1_1_dimension>`& val)

Inserts count copies of the value before position.

.. _doxid-classov_1_1_partial_shape_1ad40f2f8d29ee0c8648b1bc4b1e828664:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class InputIterator>
	void insert(
		:ref:`iterator<doxid-classov_1_1_partial_shape_1aa4e53268e0a1a2b363f70b0d80ac59dd>` position,
		InputIterator first,
		InputIterator last
		)

Inserts elements from range [first, last) before position.

.. _doxid-classov_1_1_partial_shape_1a6f742eef340b8c0e06846aca431aa812:
.. index:: pair: function; reserve

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reserve(size_t n)

Requests that the dimensions vector capacity be enough to contain n elements.

.. _doxid-classov_1_1_partial_shape_1afa7b5490e0d87e2c9bc8431320d07dc9:
.. index:: pair: function; push_back

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void push_back(const :ref:`Dimension<doxid-classov_1_1_dimension>`& val)

push element to the end of partial shape

.. _doxid-classov_1_1_partial_shape_1a5f8ce4b26f65232d9de8ab4e5e3b375d:
.. index:: pair: function; dynamic

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static PartialShape dynamic(:ref:`Rank<doxid-namespaceov_1a9e276f26decce686824844ce1c0a8993>` r = Rank::dynamic())

Construct a :ref:`PartialShape <doxid-classov_1_1_partial_shape>` with the given rank and all dimensions (if any) dynamic.



.. rubric:: Returns:

A :ref:`PartialShape <doxid-classov_1_1_partial_shape>` with the given rank, and all dimensions (if any) dynamic.

.. _doxid-classov_1_1_partial_shape_1a471e7d43a8de59e4c019ee638ab10d83:
.. index:: pair: function; merge_into

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool merge_into(PartialShape& dst, const PartialShape& src)

Try to merge one shape into another.

Merges ``src`` into ``dst``, returning ``true`` on success and ``false`` on failure. If ``false`` is returned, the effect on ``dst`` is unspecified.

To merge two partial shapes ``s1`` and ``s2`` is to find the most permissive partial shape ``s`` that is no more permissive than ``s1`` or ``s2``, if ``s`` exists. For example:

.. ref-code-block:: cpp

	merge(?,?) -> ?
	merge(?,{?,?}) -> {?,?}
	merge({?,?},{?,?}) -> {?,?}
	merge({1,2,3,4},?) -> {1,2,3,4}
	merge({1,2},{1,?}) -> {1,2}
	merge({1,2,?,?},{1,?,3,?}) -> {1,2,3,?}
	merge({1,2,3},{1,2,3}) -> {1,2,3}
	
	merge({1,?},{2,?}) fails [dimension 0 constraints are inconsistent]
	merge({?,?},{?,?,?}) fails [ranks are inconsistent]

This function (merge_into) performs the "merge" operation described above on ``dst`` and ``src``, but overwrites ``dst`` with the result and returns ``true`` if merging is successful; if merging is unsuccessful, the function returns ``false`` and may make unspecified changes to ``dst``.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst

		- The shape that ``src`` will be merged into.

	*
		- src

		- The shape that will be merged into ``dst``.



.. rubric:: Returns:

``true`` if merging succeeds, else ``false``.

.. _doxid-classov_1_1_partial_shape_1a9c35fc751bc2479087ea2f2754ab29e7:
.. index:: pair: function; broadcast_merge_into

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool broadcast_merge_into(
		PartialShape& dst,
		const PartialShape& src,
		const :ref:`ov::op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob
		)

Try to merge one shape into another along with implicit broadcasting.


