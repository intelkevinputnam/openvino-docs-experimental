.. index:: pair: namespace; ngraph::runtime::reference::internal
.. _doxid-namespacengraph_1_1runtime_1_1reference_1_1internal:

namespace ngraph::runtime::reference::internal
==============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace internal {

	// global functions

	void :target:`row_major_strides<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal_1a37439cce4bc8321722f949ffda47bea1>`(const :ref:`Shape<doxid-classov_1_1_shape>`& shape, size_t \* strides, size_t size);

	template <typename C, typename T>
	T :target:`value_with_padding_or<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal_1a8ac26d85053084bb1c5d1ac500cbb562>`(
		const :ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`& arr,
		size_t padding,
		size_t idx,
		T&& default_value
		);

	template <int A0, int A1, typename T, typename U, typename Functor>
	void :target:`numpy_autobroadcast_binop<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal_1af9db3955765493fe9249de2d2a826b23>`(
		const T \* arg0,
		const T \* arg1,
		U \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape0,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape1,
		const size_t \* strides0,
		const size_t \* strides1,
		const size_t padding0,
		const size_t padding1,
		const :ref:`Shape<doxid-classov_1_1_shape>`& output_shape,
		const size_t axis,
		const size_t stride,
		Functor elementwise_functor
		);

	size_t :target:`calculate_fixed_axis<doxid-namespacengraph_1_1runtime_1_1reference_1_1internal_1a72df6b3ad555af054ed76589cca2cea3>`(size_t axis, const size_t \* strides);

	} // namespace internal
