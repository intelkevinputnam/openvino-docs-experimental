.. index:: pair: struct; ov::util::FileTraits<char>
.. _doxid-structov_1_1util_1_1_file_traits_3_01char_01_4:

struct ov::util::FileTraits<char>
=================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <file_util.hpp>
	
	template <>
	struct FileTraits<char>
	{
		// fields
	
		static constexpr const auto :target:`file_separator<doxid-structov_1_1util_1_1_file_traits_3_01char_01_4_1ae002b8c84866ca6e2f29c31071d2672b>` =          '\\';
		static constexpr const auto :target:`dot_symbol<doxid-structov_1_1util_1_1_file_traits_3_01char_01_4_1acb7e286f9543f8a432a775bf951805be>` = '.';

		// methods
	
		static std::string :target:`library_ext<doxid-structov_1_1util_1_1_file_traits_3_01char_01_4_1aea4c764637f24dfee3c1954ffe82a77f>`();
		static std::string :target:`library_prefix<doxid-structov_1_1util_1_1_file_traits_3_01char_01_4_1a57f88f47f6fee7c06e6a6aec4a36baae>`();
	};

.. index:: pair: struct; ov::util::FileTraits
.. _doxid-structov_1_1util_1_1_file_traits:

struct ov::util::FileTraits
^^^^^^^^^^^^^^^^^^^^^^^^^^^



OS specific file traits.


.. index:: pair: struct; ov::util::FileTraits<wchar_t>
.. _doxid-structov_1_1util_1_1_file_traits_3_01wchar__t_01_4:

struct ov::util::FileTraits<wchar_t>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <file_util.hpp>
	
	template <>
	struct FileTraits<wchar_t>
	{
		// fields
	
		static constexpr const auto :target:`file_separator<doxid-structov_1_1util_1_1_file_traits_3_01wchar__t_01_4_1a20292a7655c7838efc4688ebadb04b75>` =          L'\\';
		static constexpr const auto :target:`dot_symbol<doxid-structov_1_1util_1_1_file_traits_3_01wchar__t_01_4_1aad43709681bb98d79fa008f6feacea41>` = L'.';

		// methods
	
		static std::wstring :target:`library_ext<doxid-structov_1_1util_1_1_file_traits_3_01wchar__t_01_4_1a523ac9bcf13041681bb02aa29e91474c>`();
		static std::wstring :target:`library_prefix<doxid-structov_1_1util_1_1_file_traits_3_01wchar__t_01_4_1ac51f7a790080ae100ff96892c79b3e62>`();
	};

