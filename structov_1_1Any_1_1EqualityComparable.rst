.. index:: pair: struct; ov::Any::EqualityComparable
.. _doxid-structov_1_1_any_1_1_equality_comparable:

struct ov::Any::EqualityComparable
==================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename T>
	struct EqualityComparable
	{
		// fields
	
		static constexpr static const bool :target:`value<doxid-structov_1_1_any_1_1_equality_comparable_1a1cfa8860eae99931a97a1cc3e25531bd>` = sizeof(test<T>(nullptr)) == sizeof(char);

		// methods
	
		static void \* :target:`conv<doxid-structov_1_1_any_1_1_equality_comparable_1a9e445a3d660879a6cfc090018b75da84>`(bool);
	
		template <typename U>
		static char :target:`test<doxid-structov_1_1_any_1_1_equality_comparable_1a049ed5bbb63720f0df5699fa9757afa3>`(decltype(conv(std::declval<U>()==std::declval<U>())));
	
		template <typename U>
		static long :target:`test<doxid-structov_1_1_any_1_1_equality_comparable_1a41ceea36f09706b2b955404a1fda8a4d>`(...);
	};

.. index:: pair: struct; ov::Any::EqualityComparable<std::map<T...>>
.. _doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1map_3_01_t_8_8_8_01_4_01_4:

struct ov::Any::EqualityComparable<std::map<T...>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename... T>
	struct EqualityComparable<std::map<T...>>
	{
		// fields
	
		static constexpr static const bool :target:`value<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1map_3_01_t_8_8_8_01_4_01_4_1a6c09cac05aae5e8eeebc8baee997ffd6>` = sizeof(test<std::map<T...>>(nullptr)) == sizeof(char);

		// methods
	
		static void \* :target:`conv<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1map_3_01_t_8_8_8_01_4_01_4_1ad7aa427cbaeef8579234f04971379ceb>`(bool);
	
		template <typename U>
		static char :target:`test<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1map_3_01_t_8_8_8_01_4_01_4_1ada443e62aff58938ef828e0e2a78d19e>`(decltype(conv(std::declval<typename U::key_type>()==std::declval<typename U::key_type>()&&std::declval<typename U::mapped_type>()==std::declval<typename U::mapped_type>())));
	
		template <typename U>
		static long :target:`test<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1map_3_01_t_8_8_8_01_4_01_4_1aa540ba8b7d380fde3aac173a2f660b83>`(...);
	};

.. index:: pair: struct; ov::Any::EqualityComparable<std::vector<T...>>
.. _doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1vector_3_01_t_8_8_8_01_4_01_4:

struct ov::Any::EqualityComparable<std::vector<T...>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename... T>
	struct EqualityComparable<std::vector<T...>>
	{
		// fields
	
		static constexpr static const bool :target:`value<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1vector_3_01_t_8_8_8_01_4_01_4_1ab94d42d519538c76004b753d55342bc5>` = sizeof(test<std::vector<T...>>(nullptr)) == sizeof(char);

		// methods
	
		static void \* :target:`conv<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1vector_3_01_t_8_8_8_01_4_01_4_1a4a24bc449dda22917c383ded10b1640d>`(bool);
	
		template <typename U>
		static char :target:`test<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1vector_3_01_t_8_8_8_01_4_01_4_1a35d29294ad490e90baf5f060bf8cbe0d>`(decltype(conv(std::declval<typename U::value_type>()==std::declval<typename U::value_type>())));
	
		template <typename U>
		static long :target:`test<doxid-structov_1_1_any_1_1_equality_comparable_3_01std_1_1vector_3_01_t_8_8_8_01_4_01_4_1a626c0ff6a273266ffad8570743bf4894>`(...);
	};

