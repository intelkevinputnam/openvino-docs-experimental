.. index:: pair: class; MemorySolver
.. _doxid-class_memory_solver:

class MemorySolver
==================

.. toctree::
	:hidden:

	Box <structMemorySolver_1_1Box.rst>

Overview
~~~~~~~~

Helps to solve issue of optimal memory allocation only for particular execution order. :ref:`More...<details-class_memory_solver>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <memory_solver.hpp>
	
	class MemorySolver
	{
	public:
		// structs
	
		struct :ref:`Box<doxid-struct_memory_solver_1_1_box>`;

		// construction
	
		:target:`MemorySolver<doxid-class_memory_solver_1a30ff529e745137c290d1608fe1baa917>`(const std::vector<:ref:`Box<doxid-struct_memory_solver_1_1_box>`>& boxes);

		// methods
	
		bool :target:`popupTogetherWith<doxid-class_memory_solver_1af1f9c8a6435fdaf1f7503a4fe90a5be6>`(
			:ref:`MemorySolver::Box<doxid-struct_memory_solver_1_1_box>`& box_new,
			const :ref:`MemorySolver::Box<doxid-struct_memory_solver_1_1_box>`& box_old
			);
	
		int64_t :ref:`solve<doxid-class_memory_solver_1ac0289140d33764fb5f36a60cce8391de>`();
		int64_t :ref:`getOffset<doxid-class_memory_solver_1a8fd139be2fcdbad3fb5767a03c15afdd>`(int id) const;
		int64_t :ref:`maxDepth<doxid-class_memory_solver_1ae18c2b60c51766bed3584d46fa36d01d>`();
		int64_t :ref:`maxTopDepth<doxid-class_memory_solver_1a17af133844cf6fa44afce21611738179>`();
	};
.. _details-class_memory_solver:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Helps to solve issue of optimal memory allocation only for particular execution order.

It works with abstract data description where

* Node is index in execution order

* Edge is :ref:`Box <doxid-struct_memory_solver_1_1_box>` object with size and start-finish indexes (live time)

Example:

Mem(offset) | |____| :ref:`Box <doxid-struct_memory_solver_1_1_box>` {4, 5} | |_____________| :ref:`Box <doxid-struct_memory_solver_1_1_box>` {2, 6} | |____| :ref:`Box <doxid-struct_memory_solver_1_1_box>` {3, 4} | |____| :ref:`Box <doxid-struct_memory_solver_1_1_box>` {2, 3} | |____| :ref:`Box <doxid-struct_memory_solver_1_1_box>` {6, 7} |_____________________________________ 1 2 3 4 5 6 7 8 9 ExecOrder

Boxes which has an ExecOrder-axis intersection should have no Mem-axis intersections. The goal is to define a minimal required memory blob to store all boxes with such constraints and specify all corresponding position on Mem axis(through offset field).

NOTE! Exec order is predefined.

Methods
-------

.. _doxid-class_memory_solver_1ac0289140d33764fb5f36a60cce8391de:
.. index:: pair: function; solve

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t solve()

Solve memory location with maximal reuse.



.. rubric:: Returns:

Size of common memory blob required for storing all

.. _doxid-class_memory_solver_1a8fd139be2fcdbad3fb5767a03c15afdd:
.. index:: pair: function; getOffset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t getOffset(int id) const

Provides calculated offset for specified box id

.. _doxid-class_memory_solver_1ae18c2b60c51766bed3584d46fa36d01d:
.. index:: pair: function; maxDepth

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t maxDepth()

Additional info. Max sum of box sizes required for any time stamp.

.. _doxid-class_memory_solver_1a17af133844cf6fa44afce21611738179:
.. index:: pair: function; maxTopDepth

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int64_t maxTopDepth()

Additional info. Max num of boxes required for any time stamp.


