.. index:: pair: group; XML helper utilities
.. _doxid-group__ie__dev__api__xml:

XML helper utilities
====================

.. toctree::
	:hidden:

	XMLParseUtils <namespaceXMLParseUtils.rst>
	parse_result <structparse_result.rst>

Overview
~~~~~~~~

A PUGIXML wrappers to safely extract values of requested type. :ref:`More...<details-group__ie__dev__api__xml>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`XMLParseUtils<doxid-namespace_x_m_l_parse_utils>`;

	// structs

	struct :ref:`parse_result<doxid-structparse__result>`;

	// global functions

	int :ref:`XMLParseUtils::GetIntAttr<doxid-group__ie__dev__api__xml_1gaaaa0740a272aeeef323ea0e139dcd8b7>`(const pugi::xml_node& node, const char \* str);

	int64_t :ref:`XMLParseUtils::GetInt64Attr<doxid-group__ie__dev__api__xml_1ga7a4c58242c4dcd0ea7ecd5e8fd80dcee>`(
		const pugi::xml_node& node,
		const char \* str
		);

	int64_t :ref:`XMLParseUtils::GetInt64Attr<doxid-group__ie__dev__api__xml_1ga27ed963cab7291538a628f98b4fc3568>`(
		const pugi::xml_node& node,
		const char \* str,
		int64_t defVal
		);

	uint64_t :ref:`XMLParseUtils::GetUInt64Attr<doxid-group__ie__dev__api__xml_1ga11e2888b0b9d69a9b4e5b369296b4a1a>`(
		const pugi::xml_node& node,
		const char \* str
		);

	uint64_t :ref:`XMLParseUtils::GetUInt64Attr<doxid-group__ie__dev__api__xml_1ga01a2fa47d2d7169220a29744b4269864>`(
		const pugi::xml_node& node,
		const char \* str,
		uint64_t defVal
		);

	unsigned int :ref:`XMLParseUtils::GetUIntAttr<doxid-group__ie__dev__api__xml_1gac7b7fde2364a041f61254e1e12d54d3b>`(
		const pugi::xml_node& node,
		const char \* str
		);

	unsigned int :ref:`XMLParseUtils::GetUIntAttr<doxid-group__ie__dev__api__xml_1gac21d80771b22c1c8936b3180628db084>`(
		const pugi::xml_node& node,
		const char \* str,
		unsigned int defVal
		);

	std::string :ref:`XMLParseUtils::GetStrAttr<doxid-group__ie__dev__api__xml_1ga9c0eefc9258781f344a03fcb542bdf8f>`(
		const pugi::xml_node& node,
		const char \* str
		);

	std::string :ref:`XMLParseUtils::GetStrAttr<doxid-group__ie__dev__api__xml_1gafbf16c013bba2cc620c1f2ababfe3466>`(
		const pugi::xml_node& node,
		const char \* str,
		const char \* def
		);

	bool :ref:`XMLParseUtils::GetBoolAttr<doxid-group__ie__dev__api__xml_1ga09cf84a1c0913223e647f973e988e4d0>`(const pugi::xml_node& node, const char \* str);

	bool :ref:`XMLParseUtils::GetBoolAttr<doxid-group__ie__dev__api__xml_1gaa4ce8eed10b14dccf115b3d6647a7980>`(
		const pugi::xml_node& node,
		const char \* str,
		const bool def
		);

	float :ref:`XMLParseUtils::GetFloatAttr<doxid-group__ie__dev__api__xml_1gacb654b6b218f8884181bd7499ad493a9>`(const pugi::xml_node& node, const char \* str);

	float :ref:`XMLParseUtils::GetFloatAttr<doxid-group__ie__dev__api__xml_1ga1f5244fcac69e4806f4b5d3e3f14006b>`(
		const pugi::xml_node& node,
		const char \* str,
		float defVal
		);

	:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` :ref:`XMLParseUtils::GetPrecisionAttr<doxid-group__ie__dev__api__xml_1gac853c8e081156241cc42111696a5f611>`(
		const pugi::xml_node& node,
		const char \* str
		);

	:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` :ref:`XMLParseUtils::GetPrecisionAttr<doxid-group__ie__dev__api__xml_1ga03f6e0d3b56ecba07ec27243b0c162cf>`(
		const pugi::xml_node& node,
		const char \* str,
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` def
		);

	int :ref:`XMLParseUtils::GetIntChild<doxid-group__ie__dev__api__xml_1ga1e0324aa74d0652b26b572e47c36cb78>`(
		const pugi::xml_node& node,
		const char \* str,
		int defVal
		);

	:ref:`parse_result<doxid-structparse__result>` :ref:`ParseXml<doxid-group__ie__dev__api__xml_1gae75292063abf9fa018da463f1960a846>`(const char \* file_path);

	// macros

	#define :ref:`FOREACH_CHILD<doxid-group__ie__dev__api__xml_1ga1ea10f15c23d651affba4c9ec3c910b4>`(c, p, tag)

.. _details-group__ie__dev__api__xml:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A PUGIXML wrappers to safely extract values of requested type.

Global Functions
----------------

.. _doxid-group__ie__dev__api__xml_1gaaaa0740a272aeeef323ea0e139dcd8b7:
.. index:: pair: function; GetIntAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int XMLParseUtils::GetIntAttr(const pugi::xml_node& node, const char \* str)

Gets the integer attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string



.. rubric:: Returns:

An integer value

.. _doxid-group__ie__dev__api__xml_1ga7a4c58242c4dcd0ea7ecd5e8fd80dcee:
.. index:: pair: function; GetInt64Attr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t XMLParseUtils::GetInt64Attr(
		const pugi::xml_node& node,
		const char \* str
		)

Gets the ``int64_t`` attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

An ``int64_t`` value

.. _doxid-group__ie__dev__api__xml_1ga27ed963cab7291538a628f98b4fc3568:
.. index:: pair: function; GetInt64Attr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t XMLParseUtils::GetInt64Attr(
		const pugi::xml_node& node,
		const char \* str,
		int64_t defVal
		)

Gets the ``int64_t`` attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- defVal

		- The default value



.. rubric:: Returns:

An ``int64_t`` value

.. _doxid-group__ie__dev__api__xml_1ga11e2888b0b9d69a9b4e5b369296b4a1a:
.. index:: pair: function; GetUInt64Attr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	uint64_t XMLParseUtils::GetUInt64Attr(
		const pugi::xml_node& node,
		const char \* str
		)

Gets the ``uint64_t`` attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

An ``uint64_t`` value

.. _doxid-group__ie__dev__api__xml_1ga01a2fa47d2d7169220a29744b4269864:
.. index:: pair: function; GetUInt64Attr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	uint64_t XMLParseUtils::GetUInt64Attr(
		const pugi::xml_node& node,
		const char \* str,
		uint64_t defVal
		)

Gets the ``uint64_t`` attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- defVal

		- The default value



.. rubric:: Returns:

An ``uint64_t`` value

.. _doxid-group__ie__dev__api__xml_1gac7b7fde2364a041f61254e1e12d54d3b:
.. index:: pair: function; GetUIntAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int XMLParseUtils::GetUIntAttr(
		const pugi::xml_node& node,
		const char \* str
		)

Gets the unsigned integer attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

An unsigned integer value

.. _doxid-group__ie__dev__api__xml_1gac21d80771b22c1c8936b3180628db084:
.. index:: pair: function; GetUIntAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned int XMLParseUtils::GetUIntAttr(
		const pugi::xml_node& node,
		const char \* str,
		unsigned int defVal
		)

Gets the unsigned integer attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- defVal

		- The default value



.. rubric:: Returns:

An unsigned integer value

.. _doxid-group__ie__dev__api__xml_1ga9c0eefc9258781f344a03fcb542bdf8f:
.. index:: pair: function; GetStrAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string XMLParseUtils::GetStrAttr(
		const pugi::xml_node& node,
		const char \* str
		)

Gets the string attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

A string value

.. _doxid-group__ie__dev__api__xml_1gafbf16c013bba2cc620c1f2ababfe3466:
.. index:: pair: function; GetStrAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string XMLParseUtils::GetStrAttr(
		const pugi::xml_node& node,
		const char \* str,
		const char \* def
		)

Gets the string attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- def

		- The default value



.. rubric:: Returns:

A string value

.. _doxid-group__ie__dev__api__xml_1ga09cf84a1c0913223e647f973e988e4d0:
.. index:: pair: function; GetBoolAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool XMLParseUtils::GetBoolAttr(const pugi::xml_node& node, const char \* str)

Gets the bool attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

A boolean value

.. _doxid-group__ie__dev__api__xml_1gaa4ce8eed10b14dccf115b3d6647a7980:
.. index:: pair: function; GetBoolAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool XMLParseUtils::GetBoolAttr(
		const pugi::xml_node& node,
		const char \* str,
		const bool def
		)

Gets the bool attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- def

		- The default value



.. rubric:: Returns:

A boolean value

.. _doxid-group__ie__dev__api__xml_1gacb654b6b218f8884181bd7499ad493a9:
.. index:: pair: function; GetFloatAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float XMLParseUtils::GetFloatAttr(const pugi::xml_node& node, const char \* str)

Gets the float attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

A single-precision floating point value

.. _doxid-group__ie__dev__api__xml_1ga1f5244fcac69e4806f4b5d3e3f14006b:
.. index:: pair: function; GetFloatAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float XMLParseUtils::GetFloatAttr(
		const pugi::xml_node& node,
		const char \* str,
		float defVal
		)

Gets the float attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- defVal

		- The default value



.. rubric:: Returns:

A single-precision floating point value

.. _doxid-group__ie__dev__api__xml_1gac853c8e081156241cc42111696a5f611:
.. index:: pair: function; GetPrecisionAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` XMLParseUtils::GetPrecisionAttr(
		const pugi::xml_node& node,
		const char \* str
		)

Gets the Precision attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name



.. rubric:: Returns:

A Precision value

.. _doxid-group__ie__dev__api__xml_1ga03f6e0d3b56ecba07ec27243b0c162cf:
.. index:: pair: function; GetPrecisionAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` XMLParseUtils::GetPrecisionAttr(
		const pugi::xml_node& node,
		const char \* str,
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` def
		)

Gets the Precision attribute from ``pugi::xml_node``



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string identifying value name

	*
		- def

		- The default value



.. rubric:: Returns:

A Precision value

.. _doxid-group__ie__dev__api__xml_1ga1e0324aa74d0652b26b572e47c36cb78:
.. index:: pair: function; GetIntChild

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int XMLParseUtils::GetIntChild(
		const pugi::xml_node& node,
		const char \* str,
		int defVal
		)

Gets the integer value located in a child node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node

	*
		- str

		- The string value identifying a child node

	*
		- defVal

		- The default value



.. rubric:: Returns:

An ingeter value located in a child node, ``devVal`` otherwise.

.. _doxid-group__ie__dev__api__xml_1gae75292063abf9fa018da463f1960a846:
.. index:: pair: function; ParseXml

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`parse_result<doxid-structparse__result>` ParseXml(const char \* file_path)

Parses a file and returns :ref:`parse_result <doxid-structparse__result>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- file_path

		- The file path



.. rubric:: Returns:

The :ref:`parse_result <doxid-structparse__result>`.

Macros
------

.. _doxid-group__ie__dev__api__xml_1ga1ea10f15c23d651affba4c9ec3c910b4:
.. index:: pair: define; FOREACH_CHILD

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define FOREACH_CHILD(c, p, tag)

Defines convinient for-each based cycle to iterate over node children.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- c

		- Child node name

	*
		- p

		- Parent node name

	*
		- tag

		- The tag represented as a string value

