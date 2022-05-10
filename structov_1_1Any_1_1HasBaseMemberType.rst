.. index:: pair: struct; ov::Any::HasBaseMemberType
.. _doxid-structov_1_1_any_1_1_has_base_member_type:

struct ov::Any::HasBaseMemberType
=================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename T>
	struct HasBaseMemberType
	{
		// fields
	
		static constexpr static const auto :target:`value<doxid-structov_1_1_any_1_1_has_base_member_type_1ade2c278f1d643dae44871be3c7c0147c>` = std::is_same<std::true_type, decltype(test<T>(nullptr))>::value;

		// methods
	
		template <class U>
		static auto :target:`test<doxid-structov_1_1_any_1_1_has_base_member_type_1af42d29d6fd26a378189f99c26e1cc05e>`(U \*);
	
		template <typename>
		static auto :target:`test<doxid-structov_1_1_any_1_1_has_base_member_type_1a1b15c9b2150632ec6f08fb36c14ee9af>`(...);
	};

