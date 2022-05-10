.. index:: pair: namespace; ov::util
.. _doxid-namespaceov_1_1util:

namespace ov::util
==================

.. toctree::
	:hidden:

	LOG_TYPE <enumov_1_1util_1_1LOG_TYPE.rst>
	AsTypePtr <structov_1_1util_1_1AsTypePtr.rst>
	FileTraits <structov_1_1util_1_1FileTraits.rst>
	NullLogger <structov_1_1util_1_1NullLogger.rst>
	ConstString <classov_1_1util_1_1ConstString.rst>
	LogHelper <classov_1_1util_1_1LogHelper.rst>
	Logger <classov_1_1util_1_1Logger.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace util {

	// typedefs

	typedef std::string :target:`FilePath<doxid-namespaceov_1_1util_1ae0746e01ce425506d6d00729a988ae66>`;

	// enums

	enum :ref:`LOG_TYPE<doxid-namespaceov_1_1util_1a652c65f7fe5550a6d96d273d12fe0a13>`;

	// structs

	template <typename T>
	struct :ref:`AsTypePtr<doxid-structov_1_1util_1_1_as_type_ptr>`;
	template <typename In>
	struct :ref:`AsTypePtr<std::shared_ptr<In>><doxid-structov_1_1util_1_1_as_type_ptr_3_01std_1_1shared__ptr_3_01_in_01_4_01_4>`;
	template <>
	struct :ref:`FileTraits<char><doxid-structov_1_1util_1_1_file_traits_3_01char_01_4>`;
	template <class C>
	struct :ref:`FileTraits<doxid-structov_1_1util_1_1_file_traits>`;
	template <>
	struct :ref:`FileTraits<wchar_t><doxid-structov_1_1util_1_1_file_traits_3_01wchar__t_01_4>`;
	struct :ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`;

	// classes

	class :ref:`ConstString<doxid-classov_1_1util_1_1_const_string>`;
	class :ref:`LogHelper<doxid-classov_1_1util_1_1_log_helper>`;
	class :ref:`Logger<doxid-classov_1_1util_1_1_logger>`;

	// global functions

	template <typename T>
	std::string :target:`join<doxid-namespaceov_1_1util_1a860e0918a7b731ba9e886baf48434318>`(
		const T& v,
		const std::string& sep = ", "
		);

	template <typename T>
	std::string :target:`vector_to_string<doxid-namespaceov_1_1util_1a002be85bbec779beed4e19abae5ef5ff>`(const T& v);

	std::string :target:`to_lower<doxid-namespaceov_1_1util_1a894ad99c26c8a62fe53b8aeb08f083b2>`(const std::string& s);
	std::string :target:`to_upper<doxid-namespaceov_1_1util_1aaa069463b5e010bacba16fa683bff757>`(const std::string& s);
	size_t :target:`hash_combine<doxid-namespaceov_1_1util_1a4b47ce7fcc6ec8ed02f036d9304e6340>`(const std::vector<size_t>& list);
	std::string :ref:`ltrim<doxid-namespaceov_1_1util_1a0e499fed5e7878420107cd144b8541bf>`(const std::string& s);
	std::string :ref:`rtrim<doxid-namespaceov_1_1util_1a8f1ca2765864f5afc298b8fe45ff2cc3>`(const std::string& s);
	std::string :ref:`trim<doxid-group__ie__dev__api__error__debug_1ga700ea66d016341ee5b492d0da92eb1a4>`(const std::string& s);
	bool :ref:`ends_with<doxid-namespaceov_1_1util_1a40f8f44c490a6c7a59cc5e00964f4f67>`(const std::string& src, const char \* with);

	template <typename T>
	bool :ref:`ends_with<doxid-namespaceov_1_1util_1a6bd6af133a22acff0386cbec3d425ea2>`(
		const std::basic_string<T>& str,
		const std::basic_string<T>& suffix
		);

	std::vector<std::string> :target:`split<doxid-namespaceov_1_1util_1aa7286e4cc2f3fc985397a6839f1e02e6>`(
		const std::string& s,
		char delimiter,
		bool trim = false
		);

	template <typename T>
	T :target:`ceil_div<doxid-namespaceov_1_1util_1acd9b50e41dfe7678e2f1dea6dfac4d0b>`(const T& x, const T& y);

	template <typename T, typename A, typename V>
	bool :target:`contains<doxid-namespaceov_1_1util_1aa63ec0c8f3eb1d9ca97ca24f11d6cd9a>`(
		const std::vector<T, A>& vec,
		const V& v
		);

	std::string :ref:`getenv_string<doxid-namespaceov_1_1util_1a5bb448402429618782243067e4e0adca>`(const char \* env_var);
	int32_t :ref:`getenv_int<doxid-namespaceov_1_1util_1ab354cfe4c46fe95d8154301d58af96b6>`(const char \* env_var, int32_t default_value = -1);
	bool :ref:`getenv_bool<doxid-namespaceov_1_1util_1a6ea688c6a79a06ba5298e423dafed7b2>`(const char \* env_var, bool default_value = false);
	std::string :ref:`sanitize_path<doxid-namespaceov_1_1util_1ac0bc0a27515acfb0a132138ae87b9bbf>`(const std::string& path);
	std::string :ref:`get_file_name<doxid-namespaceov_1_1util_1a33b1c13b9c29556a58eea30ad130ee4e>`(const std::string& path);
	std::string :ref:`get_absolute_file_path<doxid-namespaceov_1_1util_1a3a4a51e920722e8da8ca0d69e23964ac>`(const std::string& path);
	void :ref:`create_directory_recursive<doxid-namespaceov_1_1util_1a10cd27c761cd558dae33de9d948a066e>`(const std::string& path);
	bool :ref:`directory_exists<doxid-namespaceov_1_1util_1ab1fe64b1fe239e83e7d5f2972fdb2827>`(const std::string& path);
	uint64_t :ref:`file_size<doxid-namespaceov_1_1util_1a97cb2406c14327abff71444aa164cdf2>`(const char \* path);
	uint64_t :ref:`file_size<doxid-namespaceov_1_1util_1a3ccd2ccfa992c472756d646a2a12609b>`(const std::string& path);

	template <
		typename C,
		typename = typename std::enable_if<(std::is_same<C, char>::value || std::is_same<C, wchar_t>::value)>::type
		>
	bool :ref:`file_exists<doxid-namespaceov_1_1util_1ab25c309f82fb271ff0ec4780b317dcb9>`(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& path);

	std::string :target:`get_file_ext<doxid-namespaceov_1_1util_1ae51580cdcd158939db72ef6dad35043a>`(const std::string& path);
	std::string :target:`get_directory<doxid-namespaceov_1_1util_1aa72a84726567818331040bd2a28a5d50>`(const std::string& path);
	std::string :target:`path_join<doxid-namespaceov_1_1util_1abbf2330339c5fad8411ed30959814f02>`(const std::vector<std::string>& paths);

	void :target:`iterate_files<doxid-namespaceov_1_1util_1a820280c3bfc6f689e3a59b5630dc556d>`(
		const std::string& path,
		const std::function<void(const std::string&file, bool is_dir)>& func,
		bool recurse = false,
		bool include_links = false
		);

	void :target:`convert_path_win_style<doxid-namespaceov_1_1util_1a773a25485beb2f3f096d78f536b05df5>`(std::string& path);
	std::string :target:`get_ov_lib_path<doxid-namespaceov_1_1util_1a3f9c80e86ec8a99ba84bd8dbf43729e0>`();
	std::string :target:`from_file_path<doxid-namespaceov_1_1util_1a85161723365e612c003e771624b949ac>`(const :ref:`FilePath<doxid-namespaceov_1_1util_1ae0746e01ce425506d6d00729a988ae66>`& path);
	:ref:`FilePath<doxid-namespaceov_1_1util_1ae0746e01ce425506d6d00729a988ae66>` :target:`to_file_path<doxid-namespaceov_1_1util_1a40d469b2ec1df9086ac8ef7c01afb16a>`(const std::string& path);
	std::string :target:`get_ov_library_path<doxid-namespaceov_1_1util_1ac42adc5a6fa493c4cd2e9bdcaa593863>`();

	template <
		typename C,
		typename = typename std::enable_if<(std::is_same<C, char>::value || std::is_same<C, wchar_t>::value)>::type
		>
	std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`> :target:`make_plugin_library_name<doxid-namespaceov_1_1util_1a777684d3a172e088da7727751a5cf7df>`(
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& path,
		const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& input
		);

	constexpr const char \* :target:`find_last<doxid-namespaceov_1_1util_1a45d9d899a6cd34681a5cdd29fc562867>`(:ref:`ConstString<doxid-classov_1_1util_1_1_const_string>` s, size_t offset, char ch);
	constexpr const char \* :target:`find_last<doxid-namespaceov_1_1util_1a85cc27b84c8095dfea7f5ea8503a3b47>`(:ref:`ConstString<doxid-classov_1_1util_1_1_const_string>` s, char ch);
	constexpr const char \* :target:`get_file_name<doxid-namespaceov_1_1util_1a165b3238a9504e8ccd69728139e360f4>`(:ref:`ConstString<doxid-classov_1_1util_1_1_const_string>` s);
	constexpr const char \* :target:`trim_file_name<doxid-namespaceov_1_1util_1a90b3cf5c3e46b1ee89171fdb0f38fbc5>`(:ref:`ConstString<doxid-classov_1_1util_1_1_const_string>` root, :ref:`ConstString<doxid-classov_1_1util_1_1_const_string>` s);
	void :target:`default_logger_handler_func<doxid-namespaceov_1_1util_1affab3df30575941f289d1328c0df4c44>`(const std::string& s);

	template <typename T>
	:ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`&& :target:`operator <<<doxid-namespaceov_1_1util_1a055096b77949d4bb1e78f80ab107585f>` (:ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`&& logger, T&&);

	template <typename T>
	:ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`&& :target:`operator <<<doxid-namespaceov_1_1util_1a81bf37743b9645bc20d172ed30fa6ef9>` (:ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`&& logger, const T&);

	:ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`&& :target:`operator <<<doxid-namespaceov_1_1util_1a317cdfc968e63b6c6a6f972daeabedde>` (
		:ref:`NullLogger<doxid-structov_1_1util_1_1_null_logger>`&& logger,
		std::basic_ostream<char, std::char_traits<char>>&&)(std::basic_ostream< char, std::char_traits< char >> &
		);

	std::shared_ptr<void> :ref:`load_shared_object<doxid-namespaceov_1_1util_1a428a8eb67f5dda711b862b0687d4a7f2>`(const char \* path);

	void \* :ref:`get_symbol<doxid-namespaceov_1_1util_1a287363e9dc24fbd68b2b7b8b3a4ac944>`(
		const std::shared_ptr<void>& shared_object,
		const char \* symbolName
		);

	} // namespace util
.. _details-namespaceov_1_1util:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespaceov_1_1util_1a0e499fed5e7878420107cd144b8541bf:
.. index:: pair: function; ltrim

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string ltrim(const std::string& s)

trim from start (in place)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- - string to trim

.. _doxid-namespaceov_1_1util_1a8f1ca2765864f5afc298b8fe45ff2cc3:
.. index:: pair: function; rtrim

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string rtrim(const std::string& s)

trim from end (in place)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- - string to trim

.. _doxid-namespaceov_1_1util_1a40f8f44c490a6c7a59cc5e00964f4f67:
.. index:: pair: function; ends_with

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool ends_with(const std::string& src, const char \* with)

check string end with given substring



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- src

		- - string to check

	*
		- with

		- - given substring



.. rubric:: Returns:

true if string end with given substring

.. _doxid-namespaceov_1_1util_1a6bd6af133a22acff0386cbec3d425ea2:
.. index:: pair: function; ends_with

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	bool ends_with(
		const std::basic_string<T>& str,
		const std::basic_string<T>& suffix
		)

check string/wstring end with given substring



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- src

		- - string/wstring to check

	*
		- with

		- - given substring



.. rubric:: Returns:

true if string end with given substring

.. _doxid-namespaceov_1_1util_1a5bb448402429618782243067e4e0adca:
.. index:: pair: function; getenv_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getenv_string(const char \* env_var)

Get the names environment variable as a string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- env_var

		- The string name of the environment variable to get.



.. rubric:: Returns:

Returns string by value or an empty string if the environment variable is not set.

.. _doxid-namespaceov_1_1util_1ab354cfe4c46fe95d8154301d58af96b6:
.. index:: pair: function; getenv_int

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int32_t getenv_int(const char \* env_var, int32_t default_value = -1)

Get the names environment variable as an integer. If the value is not a valid integer then an exception is thrown.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- env_var

		- The string name of the environment variable to get.

	*
		- default_value

		- The value to return if the environment variable is not set.



.. rubric:: Returns:

Returns value or default_value if the environment variable is not set.

.. _doxid-namespaceov_1_1util_1a6ea688c6a79a06ba5298e423dafed7b2:
.. index:: pair: function; getenv_bool

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool getenv_bool(const char \* env_var, bool default_value = false)

Get the names environment variable as a boolean. If the value is not a valid boolean then an exception is thrown. Valid booleans are one of 1, 0, on, off, true, false All values are case insensitive. If the environment variable is not set the default_value is returned.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- env_var

		- The string name of the environment variable to get.

	*
		- default_value

		- The value to return if the environment variable is not set.



.. rubric:: Returns:

Returns the boolean value of the environment variable.

.. _doxid-namespaceov_1_1util_1ac0bc0a27515acfb0a132138ae87b9bbf:
.. index:: pair: function; sanitize_path

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string sanitize_path(const std::string& path)

Remove path components which would allow traversing up a directory tree.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- A path to file



.. rubric:: Returns:

A sanitiazed path

.. _doxid-namespaceov_1_1util_1a33b1c13b9c29556a58eea30ad130ee4e:
.. index:: pair: function; get_file_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string get_file_name(const std::string& path)

Returns the name with extension for a given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to the output file

.. _doxid-namespaceov_1_1util_1a3a4a51e920722e8da8ca0d69e23964ac:
.. index:: pair: function; get_absolute_file_path

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string get_absolute_file_path(const std::string& path)

Interface function to get absolute path of file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- - path to file, can be relative to current working directory

	*
		- runtime_exception

		- if any error occurred



.. rubric:: Returns:

Absolute path of file

.. _doxid-namespaceov_1_1util_1a10cd27c761cd558dae33de9d948a066e:
.. index:: pair: function; create_directory_recursive

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void create_directory_recursive(const std::string& path)

Interface function to create directorty recursively by given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- - path to file, can be relative to current working directory

	*
		- runtime_exception

		- if any error occurred

.. _doxid-namespaceov_1_1util_1ab1fe64b1fe239e83e7d5f2972fdb2827:
.. index:: pair: function; directory_exists

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool directory_exists(const std::string& path)

Interface function to check if directory exists for given path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- - path to directory



.. rubric:: Returns:

true if directory exists, false otherwise

.. _doxid-namespaceov_1_1util_1a97cb2406c14327abff71444aa164cdf2:
.. index:: pair: function; file_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	uint64_t file_size(const char \* path)

Returns file size for file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The file name



.. rubric:: Returns:

file size

.. _doxid-namespaceov_1_1util_1a3ccd2ccfa992c472756d646a2a12609b:
.. index:: pair: function; file_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	uint64_t file_size(const std::string& path)

Returns file size for file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The file name



.. rubric:: Returns:

file size

.. _doxid-namespaceov_1_1util_1ab25c309f82fb271ff0ec4780b317dcb9:
.. index:: pair: function; file_exists

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename C,
		typename = typename std::enable_if<(std::is_same<C, char>::value || std::is_same<C, wchar_t>::value)>::type
		>
	bool file_exists(const std::basic_string<:ref:`C<doxid-ie__preprocess__gapi_8cpp_1a5464533d23b59ba11030432e73528730>`>& path)

Returns true if file exists.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- The path to file



.. rubric:: Returns:

true if file exists

.. _doxid-namespaceov_1_1util_1a428a8eb67f5dda711b862b0687d4a7f2:
.. index:: pair: function; load_shared_object

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<void> load_shared_object(const char \* path)

Loads a library with the name specified.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- path

		- Full or relative path to the plugin library



.. rubric:: Returns:

Reference to shared object

.. _doxid-namespaceov_1_1util_1a287363e9dc24fbd68b2b7b8b3a4ac944:
.. index:: pair: function; get_symbol

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void \* get_symbol(
		const std::shared_ptr<void>& shared_object,
		const char \* symbolName
		)

Searches for a function symbol in the loaded module.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- shared_object

		- shared object reference

	*
		- symbolName

		- Name of the function to find

	*
		- :ref:`Exception <doxid-classov_1_1_exception>`

		- if the function is not found



.. rubric:: Returns:

A pointer to the function if found

