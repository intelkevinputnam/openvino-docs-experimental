.. index:: pair: namespace; ov::element
.. _doxid-namespaceov_1_1element:

namespace ov::element
=====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace element {

	// typedefs

	typedef std::vector<:ref:`Type<doxid-classov_1_1element_1_1_type>`> :target:`TypeVector<doxid-namespaceov_1_1element_1a7f46cb660ffbefcd50cfa90d8bfe0824>`;

	// enums

	enum :ref:`Type_t<doxid-group__ov__element__cpp__api_1gac13a83fdcf171bd2c98577bfcd37f2f1>`;

	// classes

	class :ref:`Type<doxid-classov_1_1element_1_1_type>`;

	// global functions

	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`undefined<doxid-group__ov__element__cpp__api_1gacf78890bb8ddb7762dd8b697c6d63eea>`(Type_t::undefined);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`dynamic<doxid-group__ov__element__cpp__api_1ga771959a6fb52f9f6497a5e057b2a16a6>`(Type_t::dynamic);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`boolean<doxid-group__ov__element__cpp__api_1gad0bad64613ee227cdb757f16dcf5724e>`(Type_t::boolean);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`bf16<doxid-group__ov__element__cpp__api_1ga57b838ff7f62e66151e0b53b24c27819>`(Type_t::bf16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`f16<doxid-group__ov__element__cpp__api_1ga2a30b8bad0c8cb5c76a4947c9d5074d1>`(Type_t::f16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`f32<doxid-group__ov__element__cpp__api_1gadc8a5dda3244028a5c0b024897215d43>`(Type_t::f32);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`f64<doxid-group__ov__element__cpp__api_1gae1d6966ab61642f2b84118c877e403e4>`(Type_t::f64);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`i4<doxid-group__ov__element__cpp__api_1ga8d215b67178db8292eb6897a62fa4d0d>`(Type_t::i4);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`i8<doxid-group__ov__element__cpp__api_1gaae12d14b28baf46d3c6f76c55b05fb42>`(Type_t::i8);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`i16<doxid-group__ov__element__cpp__api_1ga0b138dad04f6dd2b6c69f944a2e191c7>`(Type_t::i16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`i32<doxid-group__ov__element__cpp__api_1ga53dd97bfbd724cee3266cc80d758f323>`(Type_t::i32);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`i64<doxid-group__ov__element__cpp__api_1ga6c86a9a54d44fc205ad9cbf28ca556a6>`(Type_t::i64);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`u1<doxid-group__ov__element__cpp__api_1gae05cf21807b1a4af9a5426a7b1425cce>`(Type_t::u1);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`u4<doxid-group__ov__element__cpp__api_1gae9f6cad3bf6f31c05c004e6c62366d4e>`(Type_t::u4);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`u8<doxid-group__ov__element__cpp__api_1gaaf60c536d3e295285f6a899eb3d29e2f>`(Type_t::u8);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`u16<doxid-group__ov__element__cpp__api_1gadf6f550c6268ebff7b1356d2c9b3eee0>`(Type_t::u16);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`u32<doxid-group__ov__element__cpp__api_1ga03cd2fb04151d523674214b350fcc641>`(Type_t::u32);
	constexpr :ref:`Type<doxid-classov_1_1element_1_1_type>` :ref:`u64<doxid-group__ov__element__cpp__api_1ga891f312615ade52dff4026c4e956463e>`(:ref:`Type_t::u64<doxid-group__ov__element__cpp__api_1ggac13a83fdcf171bd2c98577bfcd37f2f1a5e543256c480ac577d30f76f9120eb74>`);

	template <typename T>
	:ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from<doxid-namespaceov_1_1element_1a68eec286fe6010586ed3eeccf014346d>`();

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< char ><doxid-namespaceov_1_1element_1a1ce7a90716cc8a765e91ba97c1074ae0>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< bool ><doxid-namespaceov_1_1element_1a1cfbb9ef21e904696bfe98dd129da13d>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< float ><doxid-namespaceov_1_1element_1a2e5638a5f1469a8122689400afbc52b4>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< double ><doxid-namespaceov_1_1element_1abf3c992885c4714500af61ec02a763b3>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< int8_t ><doxid-namespaceov_1_1element_1a79622479f9283fc05cfcb05f91b377f2>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< int16_t ><doxid-namespaceov_1_1element_1ac45703f925d2fc716f93fce62ebcd1c4>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< int32_t ><doxid-namespaceov_1_1element_1a90e4032826d924a0af3ab40ccaf4055c>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< int64_t ><doxid-namespaceov_1_1element_1aae0b88be782c6bcb23515870746c97e4>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< uint8_t ><doxid-namespaceov_1_1element_1aa650708861112de6b9fc5b3f31d2e965>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< uint16_t ><doxid-namespaceov_1_1element_1a8f84f7c09ca1e3ab5b0b8f80ae620477>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< uint32_t ><doxid-namespaceov_1_1element_1a37de7c40c571fd4cb089e8811d06eff6>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< uint64_t ><doxid-namespaceov_1_1element_1ac39526ef0dff8fdbdddf2cfe54b38952>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< ov::bfloat16 ><doxid-namespaceov_1_1element_1afa0ac1196fd33ab602ec5b2e6c0245e6>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`from< ov::float16 ><doxid-namespaceov_1_1element_1a70684802cd717d4661090c04f6480b8a>`();
	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :ref:`Type<doxid-classov_1_1element_1_1_type>` :target:`fundamental_type_for<doxid-namespaceov_1_1element_1a2aaae78d8f862b877ae9484cafd2eeac>`(const :ref:`Type<doxid-classov_1_1element_1_1_type>`& type);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :target:`operator <<<doxid-namespaceov_1_1element_1a35aacb99da28316524c8e956ddb86eb7>` (
		std::ostream& out,
		const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& obj
		);

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::istream& :target:`operator >><doxid-namespaceov_1_1element_1a421d7b78fd397edc7e3911fecfc9702e>` (
		std::istream& out,
		:ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& obj
		);

	} // namespace element
