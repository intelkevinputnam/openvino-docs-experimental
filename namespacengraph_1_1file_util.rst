.. index:: pair: namespace; ngraph::file_util
.. _doxid-namespacengraph_1_1file__util:

namespace ngraph::file_util
===========================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace file_util {

	// global functions

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`get_file_name<doxid-namespacengraph_1_1file__util_1ae2d7de7fabfb899d8b1725635544f890>`(const std::string& path);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`get_file_ext<doxid-namespacengraph_1_1file__util_1a56b88b1d79d0871e90f083816a408051>`(const std::string& path);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`get_directory<doxid-namespacengraph_1_1file__util_1a38d858d8a967e8866177c98aa52914d1>`(const std::string& path);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`path_join<doxid-namespacengraph_1_1file__util_1a2f06b57a5bfb37e9c23cb927182e7b3b>`(const std::string& s1, const std::string& s2);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :target:`path_join<doxid-namespacengraph_1_1file__util_1a7a658839eac242664d4feab059e7b5f8>`(
		const std::string& s1,
		const std::string& s2,
		const std::string& s3
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :target:`path_join<doxid-namespacengraph_1_1file__util_1a9924183ce7963b5e698be18d1c70bbc4>`(
		const std::string& s1,
		const std::string& s2,
		const std::string& s3,
		const std::string& s4
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :ref:`iterate_files<doxid-namespacengraph_1_1file__util_1a272d5eae9358a6660f1f15e2b63bc993>`(
		const std::string& path,
		std::function<void(const std::string&file, bool is_dir)> func,
		bool recurse = false,
		bool include_links = false
		);

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void :ref:`convert_path_win_style<doxid-namespacengraph_1_1file__util_1a6b7d450fd05fd89aab24e9550be65c4c>`(std::string& path);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`wstring_to_string<doxid-namespacengraph_1_1file__util_1a5b4e08079b528866b28c77793e78c812>`(const std::wstring& wstr);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::wstring :ref:`multi_byte_char_to_wstring<doxid-namespacengraph_1_1file__util_1aa17836a940768c3d6ad5e93da198e0d7>`(const char \* str);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`sanitize_path<doxid-namespacengraph_1_1file__util_1a06a0c019c2a4964f583359c1350ff3a7>`(const std::string& path);

	} // namespace file_util
.. _details-namespacengraph_1_1file__util:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespacengraph_1_1file__util_1ae2d7de7fabfb899d8b1725635544f890:
.. index:: pair: function; get_file_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string get_file_name(const std::string& path)

Returns the name with extension for a given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to the output file

.. _doxid-namespacengraph_1_1file__util_1a56b88b1d79d0871e90f083816a408051:
.. index:: pair: function; get_file_ext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string get_file_ext(const std::string& path)

Returns the file extension.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to the output file

.. _doxid-namespacengraph_1_1file__util_1a38d858d8a967e8866177c98aa52914d1:
.. index:: pair: function; get_directory

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string get_directory(const std::string& path)

Returns the directory portion of the given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to the output file

.. _doxid-namespacengraph_1_1file__util_1a2f06b57a5bfb37e9c23cb927182e7b3b:
.. index:: pair: function; path_join

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string path_join(const std::string& s1, const std::string& s2)

Joins multiple paths into a single path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s1

		- Left side of path

	*
		- s2

		- Right side of path

.. _doxid-namespacengraph_1_1file__util_1a272d5eae9358a6660f1f15e2b63bc993:
.. index:: pair: function; iterate_files

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void iterate_files(
		const std::string& path,
		std::function<void(const std::string&file, bool is_dir)> func,
		bool recurse = false,
		bool include_links = false
		)

Iterate through files and optionally directories. Symbolic links are skipped.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to iterate over

	*
		- func

		- A callback function called with each file or directory encountered

	*
		- recurse

		- Optional parameter to enable recursing through path

.. _doxid-namespacengraph_1_1file__util_1a6b7d450fd05fd89aab24e9550be65c4c:
.. index:: pair: function; convert_path_win_style

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` void convert_path_win_style(std::string& path)

Change Linux-style path ('/') to Windows-style ('\')



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to change file separator

.. _doxid-namespacengraph_1_1file__util_1a5b4e08079b528866b28c77793e78c812:
.. index:: pair: function; wstring_to_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string wstring_to_string(const std::wstring& wstr)

Conversion from wide character string to a single-byte chain.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- wstr

		- A wide-char string



.. rubric:: Returns:

A multi-byte string

.. _doxid-namespacengraph_1_1file__util_1aa17836a940768c3d6ad5e93da198e0d7:
.. index:: pair: function; multi_byte_char_to_wstring

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::wstring multi_byte_char_to_wstring(const char \* str)

Conversion from single-byte chain to wide character string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- str

		- A null-terminated string



.. rubric:: Returns:

A wide-char string

.. _doxid-namespacengraph_1_1file__util_1a06a0c019c2a4964f583359c1350ff3a7:
.. index:: pair: function; sanitize_path

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string sanitize_path(const std::string& path)

Remove path components which would allow traversing up a directory tree.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- A path to file



.. rubric:: Returns:

A sanitiazed path

