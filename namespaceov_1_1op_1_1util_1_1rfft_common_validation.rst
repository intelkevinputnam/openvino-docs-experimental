.. index:: pair: namespace; ov::op::util::rfft_common_validation
.. _doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation:

namespace ov::op::util::rfft_common_validation
==============================================

.. toctree::
	:hidden:

	RFFTKind <enumov_1_1op_1_1util_1_1rfft_common_validation_1_1RFFTKind.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace rfft_common_validation {

	// enums

	enum :ref:`RFFTKind<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1aa6e4395bbf259793266f622f9ef92bac>`;

	// global functions

	template <class T>
	void :target:`validate_input_rank<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1ab8cca24ea0f5a30620000a2727b80ac6>`(
		const :ref:`ov::op::util::FFTBase<doxid-classov_1_1op_1_1util_1_1_f_f_t_base>` \* op,
		const T& input_shape,
		const T& axes_shape,
		size_t input_rank,
		:ref:`RFFTKind<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1aa6e4395bbf259793266f622f9ef92bac>` rfft_kind
		);

	template <class T>
	void :target:`validate_axes<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1afbbd6971f26a540c60d8fd299745d179>`(
		const :ref:`ov::op::util::FFTBase<doxid-classov_1_1op_1_1util_1_1_f_f_t_base>` \* op,
		const T& axes_shape,
		std::vector<int64_t>& axes,
		size_t input_rank,
		bool axes_are_known,
		:ref:`RFFTKind<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1aa6e4395bbf259793266f622f9ef92bac>` rfft_kind
		);

	template <class T>
	void :target:`validate_signal_size<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1a042bd252317e5611eb9c277676701ffa>`(
		const :ref:`ov::op::util::FFTBase<doxid-classov_1_1op_1_1util_1_1_f_f_t_base>` \* op,
		const T& axes_shape,
		const T& signal_size_shape
		);

	template <class T>
	void :target:`shape_validation<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1a3cb66de6ba627b106f65a2a107d4ab4c>`(
		const :ref:`ov::op::util::FFTBase<doxid-classov_1_1op_1_1util_1_1_f_f_t_base>` \* op,
		const std::vector<T>& input_shapes,
		std::vector<int64_t>& axes,
		bool axes_are_known,
		:ref:`RFFTKind<doxid-namespaceov_1_1op_1_1util_1_1rfft__common__validation_1aa6e4395bbf259793266f622f9ef92bac>` rfft_kind
		);

	} // namespace rfft_common_validation
