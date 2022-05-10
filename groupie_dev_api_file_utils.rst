.. index:: pair: group; File utilities
.. _doxid-group__ie__dev__api__file__utils:

File utilities
==============

.. toctree::
	:hidden:

	FileUtils <namespaceFileUtils.rst>

Overview
~~~~~~~~

Utility functions to work with files, UNICODE support. :ref:`More...<details-group__ie__dev__api__file__utils>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`FileUtils<doxid-namespace_file_utils>`;

	// global functions

	std::string :ref:`FileUtils::absoluteFilePath<doxid-group__ie__dev__api__file__utils_1gab5f01382d64884da5217e7c5f601cb9c>`(const std::string& filePath);
	void :ref:`FileUtils::createDirectoryRecursive<doxid-group__ie__dev__api__file__utils_1ga101d402fde45ce98c55651eb5245ba8b>`(const std::string& dirPath);
	bool :ref:`FileUtils::directoryExists<doxid-group__ie__dev__api__file__utils_1gaffa64bc314fa520cee4be4973b04e31d>`(const std::string& path);
	long long :ref:`FileUtils::fileSize<doxid-group__ie__dev__api__file__utils_1ga155969b46347e15b22205880825a8633>`(const char \* fileName);

	template <typename C, typename = enableIfSupportedChar<C>>
	long long :ref:`FileUtils::fileSize<doxid-group__ie__dev__api__file__utils_1ga8b399af6fac41089783c025f3a96d8b8>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& f);

	template <typename C, typename = enableIfSupportedChar<C>>
	bool :ref:`FileUtils::fileExist<doxid-group__ie__dev__api__file__utils_1ga2da298baeb27b80819884a8addd78936>`(const :ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>` \* fileName);

	template <typename C, typename = enableIfSupportedChar<C>>
	bool :ref:`FileUtils::fileExist<doxid-group__ie__dev__api__file__utils_1gadcb7e04d0f5b6a1f164e56555a11e152>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& fileName);

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> :ref:`FileUtils::makePath<doxid-group__ie__dev__api__file__utils_1gad14432e51e0248c934fa65c25ae15d30>`(
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& folder,
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& file
		);

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> :ref:`FileUtils::fileExt<doxid-group__ie__dev__api__file__utils_1ga8bbdac777d162d794b74ddf83e80fad2>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& filename);

	std::string :ref:`InferenceEngine::getIELibraryPath<doxid-group__ie__dev__api__file__utils_1ga15d24bbab01b2c9b18d3eba65d72ed93>`();

.. _details-group__ie__dev__api__file__utils:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Utility functions to work with files, UNICODE support.

Global Functions
----------------

.. _doxid-group__ie__dev__api__file__utils_1gab5f01382d64884da5217e7c5f601cb9c:
.. index:: pair: function; absoluteFilePath

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string FileUtils::absoluteFilePath(const std::string& filePath)

Interface function to get absolute path of file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- filePath

		- - path to file, can be relative to current working directory

	*
		- :ref:`InferenceEngine::Exception <doxid-struct_inference_engine_1_1_exception>`

		- if any error occurred



.. rubric:: Returns:

Absolute path of file

.. _doxid-group__ie__dev__api__file__utils_1ga101d402fde45ce98c55651eb5245ba8b:
.. index:: pair: function; createDirectoryRecursive

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void FileUtils::createDirectoryRecursive(const std::string& dirPath)

Interface function to create directorty recursively by given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dirPath

		- - path to file, can be relative to current working directory

	*
		- :ref:`InferenceEngine::Exception <doxid-struct_inference_engine_1_1_exception>`

		- if any error occurred

.. _doxid-group__ie__dev__api__file__utils_1gaffa64bc314fa520cee4be4973b04e31d:
.. index:: pair: function; directoryExists

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool FileUtils::directoryExists(const std::string& path)

Interface function to check if directory exists for given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- - path to directory



.. rubric:: Returns:

true if directory exists, false otherwise

.. _doxid-group__ie__dev__api__file__utils_1ga155969b46347e15b22205880825a8633:
.. index:: pair: function; fileSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	long long FileUtils::fileSize(const char \* fileName)

Interface function to get the size of a file. The function supports UNICODE path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- fileName

		- - name of the file



.. rubric:: Returns:

size of the file

.. _doxid-group__ie__dev__api__file__utils_1ga8b399af6fac41089783c025f3a96d8b8:
.. index:: pair: function; fileSize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename C, typename = enableIfSupportedChar<C>>
	long long FileUtils::fileSize(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& f)

Function to get the size of a file. The function supports UNICODE path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- f

		- - string name of the file



.. rubric:: Returns:

size of the file

.. _doxid-group__ie__dev__api__file__utils_1ga2da298baeb27b80819884a8addd78936:
.. index:: pair: function; fileExist

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename C, typename = enableIfSupportedChar<C>>
	bool FileUtils::fileExist(const :ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>` \* fileName)

check if file with a given filename exists. The function supports UNICODE path



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- fileName

		- - given filename



.. rubric:: Returns:

true is exists

.. _doxid-group__ie__dev__api__file__utils_1gadcb7e04d0f5b6a1f164e56555a11e152:
.. index:: pair: function; fileExist

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename C, typename = enableIfSupportedChar<C>>
	bool FileUtils::fileExist(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& fileName)

check if file with a given filename exists. The function supports UNICODE path



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- fileName

		- - string with a given filename



.. rubric:: Returns:

true is exists

.. _doxid-group__ie__dev__api__file__utils_1gad14432e51e0248c934fa65c25ae15d30:
.. index:: pair: function; makePath

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> FileUtils::makePath(
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& folder,
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& file
		)

CPP Interface function to combint path with filename. The function supports UNICODE path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- folder

		- - path to add filename to

	*
		- file

		- - filename to add to path



.. rubric:: Returns:

string with combination of the path and the filename divided by file separator

.. _doxid-group__ie__dev__api__file__utils_1ga8bbdac777d162d794b74ddf83e80fad2:
.. index:: pair: function; fileExt

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename C, typename = enableIfSupportedChar<C>>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> FileUtils::fileExt(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& filename)

CPP Interface function to extract extension from filename.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- filename

		- - string with the name of the file which extension should be extracted



.. rubric:: Returns:

string with extracted file extension

.. _doxid-group__ie__dev__api__file__utils_1ga15d24bbab01b2c9b18d3eba65d72ed93:
.. index:: pair: function; getIELibraryPath

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string InferenceEngine::getIELibraryPath()

Returns a path to Inference Engine library.



.. rubric:: Returns:

A ``std::string`` path to Inference Engine library

