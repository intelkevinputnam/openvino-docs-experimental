.. index:: pair: namespace; std
.. _doxid-namespacestd:

namespace std
=============

.. toctree::
	:hidden:

	hash <structstd_1_1hash.rst>
	numeric_limits <classstd_1_1numeric_limits.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace std {

	// structs

	template <>
	struct :ref:`hash<ov::DiscreteTypeInfo><doxid-structstd_1_1hash_3_01ov_1_1_discrete_type_info_01_4>`;

	// classes

	template <>
	class :ref:`numeric_limits<ov::bfloat16><doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4>`;
	template <>
	class :ref:`numeric_limits<ov::float16><doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4>`;

	// global functions

	template <typename T>
	std::shared_ptr<T> :target:`dynamic_pointer_cast<doxid-namespacestd_1a82eb93a9dfd89ad5f02995ad5b3ce45c>`(const :::ref:`ov::Any<doxid-classov_1_1_any>`& any);

	template <typename T>
	std::shared_ptr<T> :target:`static_pointer_cast<doxid-namespacestd_1aca5c4087ba227523f36c36637abba650>`(const :::ref:`ov::Any<doxid-classov_1_1_any>`& any);

	bool :ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` :target:`isnan<doxid-namespacestd_1a5af8486b6d036594d068cd8e64e9a2af>`(:ref:`ov::float16<doxid-classov_1_1float16>` x);

	} // namespace std
