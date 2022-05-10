.. index:: pair: namespace; ngraph::runtime::reference::detail
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1detail:

namespace ngraph::runtime::reference::detail
============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace detail {

	// global functions

	void :target:`set_u1<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1a1a3bb5167808aba04315515657439dc2>`(uint8_t \* buf, size_t idx, uint8_t val);
	uint8_t :target:`get_u1<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1a759f204197163d40148e2b5bf37f93cb>`(const uint8_t \* buf, size_t idx);
	void :target:`set_u4<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1acf2ded984c9b591e31efebfbfe10e579>`(uint8_t \* buf, size_t idx, uint8_t val);
	uint8_t :target:`get_u4<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1a4354ef8d52f9d1f67376668f1d6f09ca>`(const uint8_t \* buf, size_t idx);
	void :target:`set_i4<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1a586db79340c58d8795147e0ab4c6aaea>`(uint8_t \* buf, size_t idx, int8_t val);
	int8_t :target:`get_i4<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1ae693b075bbad75ca242c796195bd2274>`(const uint8_t \* buf, size_t idx);

	template <typename TO, typename TI>
	TO :target:`get_value<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1ad9c8e24a4553eea531ddd4cbfcbc2610>`(
		const uint8_t \* buf,
		size_t idx,
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` from_type
		);

	template <typename TI, typename TO>
	void :target:`lp_convert<doxid-namespacengraph_1_1runtime_1_1reference_1_1detail_1a98ebdf7193fa115ee5e90ef45b3e1eef>`(
		const TI \* arg,
		TO \* out,
		size_t count,
		element::Type_t src_type,
		element::Type_t dst_type
		);

	} // namespace detail
