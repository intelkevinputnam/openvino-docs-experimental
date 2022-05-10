.. index:: pair: enum; Status
.. _doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7:

enum ov::ProfilingInfo::Status
==============================

Overview
~~~~~~~~

Defines the general status of a node. :ref:`More...<details-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <profiling_info.hpp>

	enum Status
	{
	    :ref:`NOT_RUN<doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7ad3cbb6cb9043ad908cdd5414236e6603>`,
	    :ref:`OPTIMIZED_OUT<doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7a5adb00eba7600209d8917595429638c3>`,
	    :ref:`EXECUTED<doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7aca966251f856595642d61bfa4026b086>`,
	};

.. _details-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Defines the general status of a node.

Enum Values
-----------

.. _doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7ad3cbb6cb9043ad908cdd5414236e6603:
.. index:: pair: enumvalue; NOT_RUN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NOT_RUN

A node is not executed.

.. _doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7a5adb00eba7600209d8917595429638c3:
.. index:: pair: enumvalue; OPTIMIZED_OUT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OPTIMIZED_OUT

A node is optimized out during graph optimization phase.

.. _doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7aca966251f856595642d61bfa4026b086:
.. index:: pair: enumvalue; EXECUTED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	EXECUTED

A node is executed.

