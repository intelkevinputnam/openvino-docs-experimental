.. index:: pair: group; Element types
.. _doxid-group__ov__element__cpp__api:

Element types
=============

.. toctree::
	:hidden:

	Type_t <enumov_1_1element_1_1Type_t.rst>
	Type <classov_1_1element_1_1Type.rst>

Overview
~~~~~~~~

OpenVINO Element API to work with OpenVINO element types :ref:`More...<details-group__ov__element__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// enums

	enum :ref:`ov::element::Type_t<doxid-group__ov__element__cpp__api_1gac13a83fdcf171bd2c98577bfcd37f2f1>`;

	// classes

	class :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`;

	// global functions

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::undefined<doxid-group__ov__element__cpp__api_1gacf78890bb8ddb7762dd8b697c6d63eea>`(Type_t::undefined);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::dynamic<doxid-group__ov__element__cpp__api_1ga771959a6fb52f9f6497a5e057b2a16a6>`(Type_t::dynamic);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::boolean<doxid-group__ov__element__cpp__api_1gad0bad64613ee227cdb757f16dcf5724e>`(Type_t::boolean);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::bf16<doxid-group__ov__element__cpp__api_1ga57b838ff7f62e66151e0b53b24c27819>`(Type_t::bf16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::f16<doxid-group__ov__element__cpp__api_1ga2a30b8bad0c8cb5c76a4947c9d5074d1>`(Type_t::f16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::f32<doxid-group__ov__element__cpp__api_1gadc8a5dda3244028a5c0b024897215d43>`(Type_t::f32);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::f64<doxid-group__ov__element__cpp__api_1gae1d6966ab61642f2b84118c877e403e4>`(Type_t::f64);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::i4<doxid-group__ov__element__cpp__api_1ga8d215b67178db8292eb6897a62fa4d0d>`(Type_t::i4);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::i8<doxid-group__ov__element__cpp__api_1gaae12d14b28baf46d3c6f76c55b05fb42>`(Type_t::i8);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::i16<doxid-group__ov__element__cpp__api_1ga0b138dad04f6dd2b6c69f944a2e191c7>`(Type_t::i16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`(Type_t::i32);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::i64<doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>`(Type_t::i64);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::u1<doxid-group__ov__element__cpp__api_1gae05cf21807b1a4af9a5426a7b1425cce>`(Type_t::u1);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::u4<doxid-group__ov__element__cpp__api_1gae9f6cad3bf6f31c05c004e6c62366d4e>`(Type_t::u4);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::u8<doxid-group__ov__element__cpp__api_1gaaf60c536d3e295285f6a899eb3d29e2f>`(Type_t::u8);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::u16<doxid-group__ov__element__cpp__api_1gadf6f550c6268ebff7b1356d2c9b3eee0>`(Type_t::u16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::u32<doxid-group__ov__element__cpp__api_1ga03cd2fb04151d523674214b350fcc641>`(Type_t::u32);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`ov::element::u64<doxid-group__ov__element__cpp__api_1ga891f312615ade52dff4026c4e956463e>`(:ref:`Type_t::u64<doxid-group__ov__element__cpp__api_1ggac13a83fdcf171bd2c98577bfcd37f2f1a5e543256c480ac577d30f76f9120eb74>`);

.. _details-group__ov__element__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

OpenVINO Element API to work with OpenVINO element types

Global Functions
----------------

.. _doxid-group__ov__element__cpp__api_1gacf78890bb8ddb7762dd8b697c6d63eea:
.. index:: pair: function; undefined

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::undefined(Type_t::undefined)

undefined element type

.. _doxid-group__ov__element__cpp__api_1ga771959a6fb52f9f6497a5e057b2a16a6:
.. index:: pair: function; dynamic

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::dynamic(Type_t::dynamic)

dynamic element type

.. _doxid-group__ov__element__cpp__api_1gad0bad64613ee227cdb757f16dcf5724e:
.. index:: pair: function; boolean

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::boolean(Type_t::boolean)

boolean element type

.. _doxid-group__ov__element__cpp__api_1ga57b838ff7f62e66151e0b53b24c27819:
.. index:: pair: function; bf16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::bf16(Type_t::bf16)

bf16 element type

.. _doxid-group__ov__element__cpp__api_1ga2a30b8bad0c8cb5c76a4947c9d5074d1:
.. index:: pair: function; f16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::f16(Type_t::f16)

f16 element type

.. _doxid-group__ov__element__cpp__api_1gadc8a5dda3244028a5c0b024897215d43:
.. index:: pair: function; f32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::f32(Type_t::f32)

f32 element type

.. _doxid-group__ov__element__cpp__api_1gae1d6966ab61642f2b84118c877e403e4:
.. index:: pair: function; f64

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::f64(Type_t::f64)

f64 element type

.. _doxid-group__ov__element__cpp__api_1ga8d215b67178db8292eb6897a62fa4d0d:
.. index:: pair: function; i4

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::i4(Type_t::i4)

i4 element type

.. _doxid-group__ov__element__cpp__api_1gaae12d14b28baf46d3c6f76c55b05fb42:
.. index:: pair: function; i8

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::i8(Type_t::i8)

i8 element type

.. _doxid-group__ov__element__cpp__api_1ga0b138dad04f6dd2b6c69f944a2e191c7:
.. index:: pair: function; i16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::i16(Type_t::i16)

i16 element type

.. _doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323:
.. index:: pair: function; i32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::i32(Type_t::i32)

i32 element type

.. _doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6:
.. index:: pair: function; i64

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::i64(Type_t::i64)

i64 element type

.. _doxid-group__ov__element__cpp__api_1gae05cf21807b1a4af9a5426a7b1425cce:
.. index:: pair: function; u1

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::u1(Type_t::u1)

binary element type

.. _doxid-group__ov__element__cpp__api_1gae9f6cad3bf6f31c05c004e6c62366d4e:
.. index:: pair: function; u4

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::u4(Type_t::u4)

u4 element type

.. _doxid-group__ov__element__cpp__api_1gaaf60c536d3e295285f6a899eb3d29e2f:
.. index:: pair: function; u8

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::u8(Type_t::u8)

u8 element type

.. _doxid-group__ov__element__cpp__api_1gadf6f550c6268ebff7b1356d2c9b3eee0:
.. index:: pair: function; u16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::u16(Type_t::u16)

u16 element type

.. _doxid-group__ov__element__cpp__api_1ga03cd2fb04151d523674214b350fcc641:
.. index:: pair: function; u32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::u32(Type_t::u32)

u32 element type

.. _doxid-group__ov__element__cpp__api_1ga891f312615ade52dff4026c4e956463e:
.. index:: pair: function; u64

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` ov::element::u64(:ref:`Type_t::u64<doxid-group__ov__element__cpp__api_1ggac13a83fdcf171bd2c98577bfcd37f2f1a5e543256c480ac577d30f76f9120eb74>`)

u64 element type

