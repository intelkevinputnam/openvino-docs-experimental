.. index:: pair: struct; MemorySolver::Box
.. _doxid-struct_memory_solver_1_1_box:

struct MemorySolver::Box
========================



Overview
~~~~~~~~

Representation of edge (size and live time) :ref:`More...<details-struct_memory_solver_1_1_box>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <memory_solver.hpp>
	
	struct Box
	{
		// fields
	
		int :ref:`start<doxid-struct_memory_solver_1_1_box_1a568e031ad9dd0cc4ee5ea88b50f9bb06>`;
		int :ref:`finish<doxid-struct_memory_solver_1_1_box_1ac9f929c003a3d8dfe0dc6dc454281444>`;
		int64_t :ref:`size<doxid-struct_memory_solver_1_1_box_1a24e5b69c1765c6f5c01ab0a264e680cd>`;
		int64_t :ref:`id<doxid-struct_memory_solver_1_1_box_1a3144bac02a31ff5510d0a05c85f0d163>`;
	};
.. _details-struct_memory_solver_1_1_box:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Representation of edge (size and live time)

Fields
------

.. _doxid-struct_memory_solver_1_1_box_1a568e031ad9dd0cc4ee5ea88b50f9bb06:
.. index:: pair: variable; start

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int start

Execution order index of first use. The data will be produced here.

.. _doxid-struct_memory_solver_1_1_box_1ac9f929c003a3d8dfe0dc6dc454281444:
.. index:: pair: variable; finish

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int finish

The execution order index of last use. After that data will be released. -1 is a reserved value for "till to end". The data will be alive to very end of execution.

.. _doxid-struct_memory_solver_1_1_box_1a24e5b69c1765c6f5c01ab0a264e680cd:
.. index:: pair: variable; size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t size

Size of data. In abstract unit of measure (byte, simd, cache line, ...)

.. _doxid-struct_memory_solver_1_1_box_1a3144bac02a31ff5510d0a05c85f0d163:
.. index:: pair: variable; id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t id

:ref:`Box <doxid-struct_memory_solver_1_1_box>` identifier, unique for each box. Will be used to querying calculated offset.


