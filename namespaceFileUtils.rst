.. index:: pair: namespace; FileUtils
.. _doxid-namespace_file_utils:

namespace FileUtils
===================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace FileUtils {

	// typedefs

	typedef typename std::enable_if<(std::is_same<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`, char>::value||std::is_same<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`, wchar_t>::value)>::type :ref:`enableIfSupportedChar<doxid-namespace_file_utils_1a3cb83c1e3e341822b16dfbc47e848ccd>`;

	// global functions

	std::string :ref:`absoluteFilePath<doxid-group__ie__dev__api__file__utils_1gab5f01382d64884da5217e7c5f601cb9c>`(const std::string& filePath);
	void :ref:`createDirectoryRecursive<doxid-group__ie__dev__api__file__utils_1ga101d402fde45ce98c55651eb5245ba8b>`(const std::string& dirPath);
	bool :ref:`directoryExists<doxid-group__ie__dev__api__file__utils_1gaffa64bc314fa520cee4be4973b04e31d>`(const std::string& path);
	long long :ref:`fileSize<doxid-group__ie__dev__api__file__utils_1ga155969b46347e15b22205880825a8633>`(const char \* fileName);

	template <typename C, typename = enableIfSupportedChar<C>>
	long long :ref:`fileSize<doxid-group__ie__dev__api__file__utils_1ga8b399af6fac41089783c025f3a96d8b8>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& f);

	template <typename C, typename = enableIfSupportedChar<C>>
	bool :ref:`fileExist<doxid-group__ie__dev__api__file__utils_1ga2da298baeb27b80819884a8addd78936>`(const :ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>` \* fileName);

	template <typename C, typename = enableIfSupportedChar<C>>
	bool :ref:`fileExist<doxid-group__ie__dev__api__file__utils_1gadcb7e04d0f5b6a1f164e56555a11e152>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& fileName);

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> :ref:`makePath<doxid-group__ie__dev__api__file__utils_1gad14432e51e0248c934fa65c25ae15d30>`(
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& folder,
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& file
		);

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> :ref:`fileExt<doxid-group__ie__dev__api__file__utils_1ga8bbdac777d162d794b74ddf83e80fad2>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& filename);

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> :target:`makePluginLibraryName<doxid-namespace_file_utils_1a26cb4f9bf92a9a4b2d35f7f0be962607>`(
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& path,
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& input
		);

	} // namespace FileUtils
.. _details-namespace_file_utils:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Typedefs
--------

.. _doxid-namespace_file_utils_1a3cb83c1e3e341822b16dfbc47e848ccd:
.. index:: pair: typedef; enableIfSupportedChar

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef typename std::enable_if<(std::is_same<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`, char>::value||std::is_same<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`, wchar_t>::value)>::type enableIfSupportedChar

Enables only ``char`` or ``wchar_t`` template specializations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- C

		- A char type

