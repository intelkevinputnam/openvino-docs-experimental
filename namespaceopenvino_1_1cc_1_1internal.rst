.. index:: pair: namespace; openvino::cc::internal
.. _doxid-namespaceopenvino_1_1cc_1_1internal:

namespace openvino::cc::internal
================================

.. toctree::
	:hidden:

	case_wrapper <structopenvino_1_1cc_1_1internal_1_1case_wrapper.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace internal {

	// structs

	template <typename C, typename T>
	struct :ref:`case_wrapper<doxid-structopenvino_1_1cc_1_1internal_1_1case__wrapper>`;

	// global functions

	template <typename T, typename C>
	:ref:`case_wrapper<doxid-structopenvino_1_1cc_1_1internal_1_1case__wrapper>`<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`, T> :target:`make_case_wrapper<doxid-namespaceopenvino_1_1cc_1_1internal_1acfe37a64e408998e004f714bd57bb427>`(:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`&& val);

	template <template<typename...> class Fn, typename Ctx, typename T, typename Case>
	bool :target:`match<doxid-namespaceopenvino_1_1cc_1_1internal_1ae85ad2baf2156c42ef873d4deb3c63c3>`(
		Ctx&& ctx,
		T&& val,
		Case&& cs
		);

	template <
		template<typename...> class Fn,
		typename Ctx,
		typename T,
		typename Case,
		typename... Cases
		>
	bool :target:`match<doxid-namespaceopenvino_1_1cc_1_1internal_1a35f103c9d6d1cf66c9b621719b9af27c>`(
		Ctx&& ctx,
		T&& val,
		Case&& cs,
		Cases&&... cases
		);

	} // namespace internal
