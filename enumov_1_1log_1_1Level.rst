.. index:: pair: enum; Level
.. _doxid-group__ov__runtime__cpp__prop__api_1ga9868e1ed6b0286d17cdb0ab85b2cc66b:

enum ov::log::Level
===================

Overview
~~~~~~~~

Enum to define possible log levels. :ref:`More...<details-group__ov__runtime__cpp__prop__api_1ga9868e1ed6b0286d17cdb0ab85b2cc66b>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>

	enum Level
	{
	    :ref:`NO<doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66bac2f3f489a00553e7a01d369c103c7251>`      = -1,
	    :ref:`ERR<doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66bacd22bad976363fdd1bfbf6759fede482>`     = 0,
	    :ref:`WARNING<doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66ba059e9861e0400dfbe05c98a841f3f96b>` = 1,
	    :ref:`INFO<doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66ba551b723eafd6a31d444fcb2f5920fbd3>`    = 2,
	    :ref:`DEBUG<doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66badc30ec20708ef7b0f641ef78b7880a15>`   = 3,
	    :ref:`TRACE<doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66ba2d3e4144aa384b18849ab9a8abad74d6>`   = 4,
	};

.. _details-group__ov__runtime__cpp__prop__api_1ga9868e1ed6b0286d17cdb0ab85b2cc66b:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define possible log levels.

Enum Values
-----------

.. _doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66bac2f3f489a00553e7a01d369c103c7251:
.. index:: pair: enumvalue; NO

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NO

disable any logging

.. _doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66bacd22bad976363fdd1bfbf6759fede482:
.. index:: pair: enumvalue; ERR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ERR

error events that might still allow the application to continue running

.. _doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66ba059e9861e0400dfbe05c98a841f3f96b:
.. index:: pair: enumvalue; WARNING

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	WARNING

potentially harmful situations which may further lead to ERROR

.. _doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66ba551b723eafd6a31d444fcb2f5920fbd3:
.. index:: pair: enumvalue; INFO

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	INFO

informational messages that display the progress of the application at coarse-grained level

.. _doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66badc30ec20708ef7b0f641ef78b7880a15:
.. index:: pair: enumvalue; DEBUG

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DEBUG

fine-grained events that are most useful to debug an application.

.. _doxid-group__ov__runtime__cpp__prop__api_1gga9868e1ed6b0286d17cdb0ab85b2cc66ba2d3e4144aa384b18849ab9a8abad74d6:
.. index:: pair: enumvalue; TRACE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TRACE

finer-grained informational events than the DEBUG

