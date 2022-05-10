.. index:: pair: group; ITT profiling utilities
.. _doxid-group__ie__dev__profiling:

ITT profiling utilities
=======================

.. toctree::
	:hidden:

	openvino <namespaceopenvino.rst>
	ScopedTask <classopenvino_1_1itt_1_1ScopedTask.rst>
	TaskChain <classopenvino_1_1itt_1_1TaskChain.rst>

Overview
~~~~~~~~

Configurable macro wrappers for ITT profiling. :ref:`More...<details-group__ie__dev__profiling>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`openvino<doxid-namespaceopenvino>`;
		namespace :ref:`openvino::cc<doxid-namespaceopenvino_1_1cc>`;
			namespace :ref:`openvino::cc::internal<doxid-namespaceopenvino_1_1cc_1_1internal>`;
		namespace :ref:`openvino::itt<doxid-namespaceopenvino_1_1itt>`;

	// typedefs

	typedef struct :ref:`openvino::itt::domain_<doxid-structopenvino_1_1itt_1_1domain__>` \* :ref:`openvino::itt::domain_t<doxid-group__ie__dev__profiling_1gaf592f242d12fecb8f6bd3391ae8bf52a>`;
	typedef struct :ref:`openvino::itt::handle_<doxid-structopenvino_1_1itt_1_1handle__>` \* :ref:`openvino::itt::handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>`;

	// classes

	template <domain_t(\*)() domain>
	class :ref:`openvino::itt::ScopedTask<doxid-structopenvino_1_1itt_1_1_scoped_task>`;
	template <domain_t(\*)() domain>
	class :ref:`openvino::itt::TaskChain<doxid-classopenvino_1_1itt_1_1_task_chain>`;

	// global functions

	void :ref:`openvino::itt::threadName<doxid-group__ie__dev__profiling_1gaf246080ccfe9616f6fa6853e684dee45>`(const char \* name);
	:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` :ref:`openvino::itt::handle<doxid-group__ie__dev__profiling_1ga8579f29ef5313d519bcaee20dd543a1b>`(char const \* name);

	// macros

	#define :ref:`OV_ITT_DOMAIN<doxid-group__ie__dev__profiling_1ga83ad6f539c8e1aef944160e37fcfcb4d>`(...)
	#define :ref:`OV_ITT_SCOPE<doxid-group__ie__dev__profiling_1gab36eff302250b41b12848597e5684d68>`(group, ...)
	#define :ref:`OV_ITT_SCOPED_TASK<doxid-group__ie__dev__profiling_1gac1e4b5bdc6097e2afd26b75d05dfe1ef>`(...)
	#define :ref:`OV_ITT_SCOPE_NEXT<doxid-group__ie__dev__profiling_1ga47367f3d199b8f71534fd3f7fb9b2464>`(group, ...)
	#define :ref:`OV_ITT_SCOPE_SKIP<doxid-group__ie__dev__profiling_1gadde35caedd8df731ec882463b4f812be>`(group, chainId)
	#define :ref:`OV_ITT_TASK_CHAIN<doxid-group__ie__dev__profiling_1gaa9f15503cbc6a9fe20091ded356e17dd>`(...)
	#define :ref:`OV_ITT_TASK_NEXT<doxid-group__ie__dev__profiling_1ga319de5d71d3550d2638188e9fb7be3b5>`(...)
	#define :ref:`OV_ITT_TASK_SKIP<doxid-group__ie__dev__profiling_1ga1381f651372b35303eea8009a7ebbd2e>`(chainId)

.. _details-group__ie__dev__profiling:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Configurable macro wrappers for ITT profiling.

Typedefs
--------

.. _doxid-group__ie__dev__profiling_1gaf592f242d12fecb8f6bd3391ae8bf52a:
.. index:: pair: typedef; domain_t

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef struct :ref:`openvino::itt::domain_<doxid-structopenvino_1_1itt_1_1domain__>` \* openvino::itt::domain_t

A domain type which enables tagging trace data for different modules or libraries in a program.

.. _doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7:
.. index:: pair: typedef; handle_t

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef struct :ref:`openvino::itt::handle_<doxid-structopenvino_1_1itt_1_1handle__>` \* openvino::itt::handle_t

Annotation handle for section of code which would be named at runtime.

Global Functions
----------------

.. _doxid-group__ie__dev__profiling_1gaf246080ccfe9616f6fa6853e684dee45:
.. index:: pair: function; threadName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void openvino::itt::threadName(const char \* name)

Set thread name using a char string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- [in] The thread name

.. _doxid-group__ie__dev__profiling_1ga8579f29ef5313d519bcaee20dd543a1b:
.. index:: pair: function; handle

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` openvino::itt::handle(char const \* name)

Create annotation handle with a given name.

If template function is instantiated with a tag, the handle is created as a singleton.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- [in] The annotation name

Macros
------

.. _doxid-group__ie__dev__profiling_1ga83ad6f539c8e1aef944160e37fcfcb4d:
.. index:: pair: define; OV_ITT_DOMAIN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_DOMAIN(...)

Declare domain with a given name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- domainName

		- [in] Known at compile time name of module or library (the domain name).

	*
		- domainDisplayName

		- [in] Domain name used as the ITT counter name and displayed in Intel VTune. Parameter is optional.

.. _doxid-group__ie__dev__profiling_1gab36eff302250b41b12848597e5684d68:
.. index:: pair: define; OV_ITT_SCOPE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_SCOPE(group, ...)

Annotate section of code till scope exit to be profiled using known ``handle`` or ``taskName`` as section id.

In case if handle or taskName absent, the current function name is used.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- group

		- [in] ITT counter group name used for enabling/disabling at compile time.

	*
		- domainName

		- [in] Known at compile time name of module or library (the domain name).

	*
		- handleOrTaskName

		- [in] The annotation name or handle for section of code. Parameter is optional.

.. _doxid-group__ie__dev__profiling_1gac1e4b5bdc6097e2afd26b75d05dfe1ef:
.. index:: pair: define; OV_ITT_SCOPED_TASK

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_SCOPED_TASK(...)

Annotate section of code till scope exit to be profiled using known ``handle`` or ``taskName`` as section id.

In case if handle or taskName absent, the current function name is used.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- domainName

		- [in] Known at compile time name of module or library (the domain name).

	*
		- handleOrTaskName

		- [in] The annotation name or handle for section of code. Parameter is optional.

.. _doxid-group__ie__dev__profiling_1ga47367f3d199b8f71534fd3f7fb9b2464:
.. index:: pair: define; OV_ITT_SCOPE_NEXT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_SCOPE_NEXT(group, ...)

Inserts new annotated section of code to tasks chain using ``taskName`` as section id.

If taskName is missing, the current chain index is used.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- group

		- [in] ITT counter group name used for enabling/disabling at compile time.

	*
		- chainId

		- [in] The tasks chain identifier.

	*
		- taskOrTaskName

		- [in] The annotation name or handle for section of code. Parameter is optional.

.. _doxid-group__ie__dev__profiling_1gadde35caedd8df731ec882463b4f812be:
.. index:: pair: define; OV_ITT_SCOPE_SKIP

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_SCOPE_SKIP(group, chainId)

Skips the remaining task scope.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- group

		- [in] ITT counter group name used for enabling/disabling at compile time.

	*
		- chainId

		- [in] The tasks chain identifier.

.. _doxid-group__ie__dev__profiling_1gaa9f15503cbc6a9fe20091ded356e17dd:
.. index:: pair: define; OV_ITT_TASK_CHAIN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_TASK_CHAIN(...)

Begins the sequrence of an annotated sections of code using ``prefix`` and ``taskName`` as section id.

In case if prefix absent, the current function name is used, if taskName absent, the first chain index is used, i.e 1. In case if prefix absent, the current function name is used, if taskName absent, the first chain index is used, i.e 1.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- group

		- [in] ITT counter group name used for enabling/disabling at compile time.

	*
		- chainId

		- [in] The tasks chain identifier.

	*
		- domainName

		- [in] Known at compile time name of module or library (the domain name).

	*
		- prefix

		- [in] The task chain name prefix. The task name starts with this prefix. Parameter is optional.

	*
		- taskName

		- [in] The annotation name for section of code. Parameter is optional.

	*
		- chainId

		- [in] The tasks chain identifier.

	*
		- domainName

		- [in] Known at compile time name of module or library (the domain name).

	*
		- prefix

		- [in] The task chain name prefix. The task name starts with this prefix. Parameter is optional.

	*
		- taskName

		- [in] The annotation name for section of code. Parameter is optional.

.. _doxid-group__ie__dev__profiling_1ga319de5d71d3550d2638188e9fb7be3b5:
.. index:: pair: define; OV_ITT_TASK_NEXT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_TASK_NEXT(...)

Inserts new annotated section of code to tasks chain using ``taskName`` as section id.

If taskName is missing, the current chain index is used.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- chainId

		- [in] The tasks chain identifier.

	*
		- taskOrTaskName

		- [in] The annotation name or handle for section of code. Parameter is optional.

.. _doxid-group__ie__dev__profiling_1ga1381f651372b35303eea8009a7ebbd2e:
.. index:: pair: define; OV_ITT_TASK_SKIP

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define OV_ITT_TASK_SKIP(chainId)

Skips the remaining task scope.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- chainId

		- [in] The tasks chain identifier.

