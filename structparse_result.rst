.. index:: pair: struct; parse_result
.. _doxid-structparse__result:

struct parse_result
===================



Overview
~~~~~~~~

A XML parse result structure with an error message and the ``pugi::xml_document`` document. :ref:`More...<details-structparse__result>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <xml_parse_utils.h>
	
	struct parse_result
	{
		// fields
	
		std::unique_ptr<pugi::xml_document> :ref:`xml<doxid-structparse__result_1a5ff808094789bd2cf74f010c41a00cc3>`;
		std::string :ref:`error_msg<doxid-structparse__result_1ae3d2974a321a5e1fac4045f83708d863>` {};

		// construction
	
		:ref:`parse_result<doxid-structparse__result_1aa88fae2a12c333d7ea57fcb96558c09b>`(std::unique_ptr<pugi::xml_document>&& xml, std::string error_msg);
	};
.. _details-structparse__result:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A XML parse result structure with an error message and the ``pugi::xml_document`` document.

Fields
------

.. _doxid-structparse__result_1a5ff808094789bd2cf74f010c41a00cc3:
.. index:: pair: variable; xml

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::unique_ptr<pugi::xml_document> xml

A XML document.

.. _doxid-structparse__result_1ae3d2974a321a5e1fac4045f83708d863:
.. index:: pair: variable; error_msg

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string error_msg {}

An error message.

Construction
------------

.. _doxid-structparse__result_1aa88fae2a12c333d7ea57fcb96558c09b:
.. index:: pair: function; parse_result

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	parse_result(std::unique_ptr<pugi::xml_document>&& xml, std::string error_msg)

Constructs :ref:`parse_result <doxid-structparse__result>` with ``pugi::xml_document`` and an error message.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- xml

		- The ``pugi::xml_document``

	*
		- error_msg

		- The error message


