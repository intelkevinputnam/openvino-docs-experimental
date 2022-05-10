.. index:: pair: class; openvino::itt::ScopedTask
.. _doxid-structopenvino_1_1itt_1_1_scoped_task:

class openvino::itt::ScopedTask
===============================



Overview
~~~~~~~~

Used to annotate section of code which would be named at runtime. :ref:`More...<details-structopenvino_1_1itt_1_1_scoped_task>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <itt.hpp>
	
	template <domain_t(\*)() domain>
	class ScopedTask
	{
	public:
		// construction
	
		:ref:`ScopedTask<doxid-structopenvino_1_1itt_1_1_scoped_task_1a09602c8651ada4d64dbc4d07c917036f>`(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` taskHandle);
		:target:`ScopedTask<doxid-structopenvino_1_1itt_1_1_scoped_task_1a5ac3fddd58e29a063800c2b7d40a861a>`(const ScopedTask&);

		// methods
	
		ScopedTask& :target:`operator =<doxid-structopenvino_1_1itt_1_1_scoped_task_1a2ba7252c68f2599f389def725c9b97a9>` (const ScopedTask&);
	};
.. _details-structopenvino_1_1itt_1_1_scoped_task:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Used to annotate section of code which would be named at runtime.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- The

		- ``domain`` parameter is domain type which shoud be defined with :ref:`OV_ITT_DOMAIN() <doxid-group__ie__dev__profiling_1ga83ad6f539c8e1aef944160e37fcfcb4d>` macro.

Construction
------------

.. _doxid-structopenvino_1_1itt_1_1_scoped_task_1a09602c8651ada4d64dbc4d07c917036f:
.. index:: pair: function; ScopedTask

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ScopedTask(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` taskHandle)

Construct :ref:`ScopedTask <doxid-structopenvino_1_1itt_1_1_scoped_task>` with defined annotation handle.


