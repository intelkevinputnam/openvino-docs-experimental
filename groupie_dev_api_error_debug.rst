.. index:: pair: group; Error handling and debug helpers
.. _doxid-group__ie__dev__api__error__debug:

Error handling and debug helpers
================================

.. toctree::
	:hidden:

	DescriptionBuffer <structInferenceEngine_1_1DescriptionBuffer.rst>

Overview
~~~~~~~~

Utility methods to works with errors or exceptional situations. :ref:`More...<details-group__ie__dev__api__error__debug>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// structs

	struct :ref:`InferenceEngine::DescriptionBuffer<doxid-struct_inference_engine_1_1_description_buffer>`;

	// global functions

	std::string :ref:`ov::util::trim<doxid-group__ie__dev__api__error__debug_1ga700ea66d016341ee5b492d0da92eb1a4>`(const std::string& s);

.. _details-group__ie__dev__api__error__debug:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Utility methods to works with errors or exceptional situations.

Global Functions
----------------

.. _doxid-group__ie__dev__api__error__debug_1ga700ea66d016341ee5b492d0da92eb1a4:
.. index:: pair: function; trim

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string ov::util::trim(const std::string& s)

Trims std::string from both ends (in place)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- s

		- A reference to a std::tring to trim



.. rubric:: Returns:

A reference to a trimmed std::string

