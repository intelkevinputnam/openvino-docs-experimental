.. index:: pair: namespace; XMLParseUtils
.. _doxid-namespace_x_m_l_parse_utils:

namespace XMLParseUtils
=======================



Overview
~~~~~~~~

XML helpers function to extract values from ``pugi::xml_node`` :ref:`More...<details-namespace_x_m_l_parse_utils>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace XMLParseUtils {

	// global functions

	int :ref:`GetIntAttr<doxid-group__ie__dev__api__xml_1gaaaa0740a272aeeef323ea0e139dcd8b7>`(const pugi::xml_node& node, const char \* str);
	int :ref:`GetIntAttr<doxid-namespace_x_m_l_parse_utils_1ab5c06a93131de9bb94a3f9c148c794b1>`(const pugi::xml_node& node, const char \* str, int defVal);
	int64_t :ref:`GetInt64Attr<doxid-group__ie__dev__api__xml_1ga7a4c58242c4dcd0ea7ecd5e8fd80dcee>`(const pugi::xml_node& node, const char \* str);

	int64_t :ref:`GetInt64Attr<doxid-group__ie__dev__api__xml_1ga27ed963cab7291538a628f98b4fc3568>`(
		const pugi::xml_node& node,
		const char \* str,
		int64_t defVal
		);

	uint64_t :ref:`GetUInt64Attr<doxid-group__ie__dev__api__xml_1ga11e2888b0b9d69a9b4e5b369296b4a1a>`(const pugi::xml_node& node, const char \* str);

	uint64_t :ref:`GetUInt64Attr<doxid-group__ie__dev__api__xml_1ga01a2fa47d2d7169220a29744b4269864>`(
		const pugi::xml_node& node,
		const char \* str,
		uint64_t defVal
		);

	unsigned int :ref:`GetUIntAttr<doxid-group__ie__dev__api__xml_1gac7b7fde2364a041f61254e1e12d54d3b>`(const pugi::xml_node& node, const char \* str);

	unsigned int :ref:`GetUIntAttr<doxid-group__ie__dev__api__xml_1gac21d80771b22c1c8936b3180628db084>`(
		const pugi::xml_node& node,
		const char \* str,
		unsigned int defVal
		);

	std::string :ref:`GetStrAttr<doxid-group__ie__dev__api__xml_1ga9c0eefc9258781f344a03fcb542bdf8f>`(const pugi::xml_node& node, const char \* str);

	std::string :ref:`GetStrAttr<doxid-group__ie__dev__api__xml_1gafbf16c013bba2cc620c1f2ababfe3466>`(
		const pugi::xml_node& node,
		const char \* str,
		const char \* def
		);

	bool :ref:`GetBoolAttr<doxid-group__ie__dev__api__xml_1ga09cf84a1c0913223e647f973e988e4d0>`(const pugi::xml_node& node, const char \* str);
	bool :ref:`GetBoolAttr<doxid-group__ie__dev__api__xml_1gaa4ce8eed10b14dccf115b3d6647a7980>`(const pugi::xml_node& node, const char \* str, const bool def);
	float :ref:`GetFloatAttr<doxid-group__ie__dev__api__xml_1gacb654b6b218f8884181bd7499ad493a9>`(const pugi::xml_node& node, const char \* str);
	float :ref:`GetFloatAttr<doxid-group__ie__dev__api__xml_1ga1f5244fcac69e4806f4b5d3e3f14006b>`(const pugi::xml_node& node, const char \* str, float defVal);

	:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` :ref:`GetPrecisionAttr<doxid-group__ie__dev__api__xml_1gac853c8e081156241cc42111696a5f611>`(
		const pugi::xml_node& node,
		const char \* str
		);

	:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` :ref:`GetPrecisionAttr<doxid-group__ie__dev__api__xml_1ga03f6e0d3b56ecba07ec27243b0c162cf>`(
		const pugi::xml_node& node,
		const char \* str,
		:ref:`InferenceEngine::Precision<doxid-class_inference_engine_1_1_precision>` def
		);

	int :ref:`GetIntChild<doxid-group__ie__dev__api__xml_1ga1e0324aa74d0652b26b572e47c36cb78>`(const pugi::xml_node& node, const char \* str, int defVal);

	} // namespace XMLParseUtils
.. _details-namespace_x_m_l_parse_utils:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

XML helpers function to extract values from ``pugi::xml_node``

Global Functions
----------------

.. _doxid-namespace_x_m_l_parse_utils_1ab5c06a93131de9bb94a3f9c148c794b1:
.. index:: pair: function; GetIntAttr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int GetIntAttr(const pugi::xml_node& node, const char \* str, int defVal)

Gets the integer attribute from ``pugi::xml_node``



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

An integer value

