.. index:: pair: group; System configuration utilities
.. _doxid-group__ie__dev__api__system__conf:

System configuration utilities
==============================



Overview
~~~~~~~~

API to get information about the system, core processor capabilities. :ref:`More...<details-group__ie__dev__api__system__conf>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	bool :ref:`InferenceEngine::checkOpenMpEnvVars<doxid-group__ie__dev__api__system__conf_1gaa28c1b3e2f68e250f9b63e16926f928d>`(bool includeOMPNumThreads = true);
	std::vector<int> :ref:`InferenceEngine::getAvailableNUMANodes<doxid-group__ie__dev__api__system__conf_1ga52d33b4d51af9fa281065588e44e5db6>`();
	std::vector<int> :ref:`InferenceEngine::getAvailableCoresTypes<doxid-group__ie__dev__api__system__conf_1gab32f5b1f1bc6cd2cae978a59ed90b79f>`();
	int :ref:`InferenceEngine::getNumberOfCPUCores<doxid-group__ie__dev__api__system__conf_1ga7be4a12638aae29cc2bc7bde4cafe7a5>`(bool bigCoresOnly = false);
	int :ref:`InferenceEngine::getNumberOfLogicalCPUCores<doxid-group__ie__dev__api__system__conf_1ga622be8b8ccf1e73d9e2c7853de2cb5ef>`(bool bigCoresOnly = false);
	bool :ref:`InferenceEngine::with_cpu_x86_sse42<doxid-group__ie__dev__api__system__conf_1ga9bfd2d1684149c962a40aca5ac02305e>`();
	bool :ref:`InferenceEngine::with_cpu_x86_avx<doxid-group__ie__dev__api__system__conf_1gada020cb5069326ca18dff97b7564948a>`();
	bool :ref:`InferenceEngine::with_cpu_x86_avx2<doxid-group__ie__dev__api__system__conf_1gadf27a09b4f47d98f9162d5256f7bae4c>`();
	bool :ref:`InferenceEngine::with_cpu_x86_avx512f<doxid-group__ie__dev__api__system__conf_1ga865cfc186254bcc13cc0c39441879b8d>`();
	bool :ref:`InferenceEngine::with_cpu_x86_avx512_core<doxid-group__ie__dev__api__system__conf_1ga3cf444492c290b36e82267ff4e7d20a8>`();
	bool :ref:`InferenceEngine::with_cpu_x86_bfloat16<doxid-group__ie__dev__api__system__conf_1gad31c357806f14f6ccec66e102a0c32f3>`();

.. _details-group__ie__dev__api__system__conf:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

API to get information about the system, core processor capabilities.

Global Functions
----------------

.. _doxid-group__ie__dev__api__system__conf_1gaa28c1b3e2f68e250f9b63e16926f928d:
.. index:: pair: function; checkOpenMpEnvVars

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::checkOpenMpEnvVars(bool includeOMPNumThreads = true)

Checks whether OpenMP environment variables are defined.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- includeOMPNumThreads

		- Indicates if the omp number threads is included



.. rubric:: Returns:

``True`` if any OpenMP environment variable is defined, ``false`` otherwise

.. _doxid-group__ie__dev__api__system__conf_1ga52d33b4d51af9fa281065588e44e5db6:
.. index:: pair: function; getAvailableNUMANodes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> InferenceEngine::getAvailableNUMANodes()

Returns available CPU NUMA nodes (on Linux, and Windows [only with TBB], single node is assumed on all other OSes)



.. rubric:: Returns:

NUMA nodes

.. _doxid-group__ie__dev__api__system__conf_1gab32f5b1f1bc6cd2cae978a59ed90b79f:
.. index:: pair: function; getAvailableCoresTypes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> InferenceEngine::getAvailableCoresTypes()

Returns available CPU cores types (on Linux, and Windows) and ONLY with TBB, single core type is assumed otherwise.



.. rubric:: Returns:

Vector of core types

.. _doxid-group__ie__dev__api__system__conf_1ga7be4a12638aae29cc2bc7bde4cafe7a5:
.. index:: pair: function; getNumberOfCPUCores

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int InferenceEngine::getNumberOfCPUCores(bool bigCoresOnly = false)

Returns number of CPU physical cores on Linux/Windows (which is considered to be more performance friendly for servers) (on other OSes it simply relies on the original parallel API of choice, which usually uses the logical cores). call function with 'false' to get #phys cores of all types call function with 'true' to get #phys 'Big' cores number of 'Little' = 'all' - 'Big'.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bigCoresOnly

		- Additionally limits the number of reported cores to the 'Big' cores only.



.. rubric:: Returns:

Number of physical CPU cores.

.. _doxid-group__ie__dev__api__system__conf_1ga622be8b8ccf1e73d9e2c7853de2cb5ef:
.. index:: pair: function; getNumberOfLogicalCPUCores

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int InferenceEngine::getNumberOfLogicalCPUCores(bool bigCoresOnly = false)

Returns number of CPU logical cores on Linux/Windows (on other OSes it simply relies on the original parallel API of choice, which uses the 'all' logical cores). call function with 'false' to get #logical cores of all types call function with 'true' to get #logical 'Big' cores number of 'Little' = 'all' - 'Big'.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bigCoresOnly

		- Additionally limits the number of reported cores to the 'Big' cores only.



.. rubric:: Returns:

Number of logical CPU cores.

.. _doxid-group__ie__dev__api__system__conf_1ga9bfd2d1684149c962a40aca5ac02305e:
.. index:: pair: function; with_cpu_x86_sse42

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::with_cpu_x86_sse42()

Checks whether CPU supports SSE 4.2 capability.



.. rubric:: Returns:

``True`` is SSE 4.2 instructions are available, ``false`` otherwise

.. _doxid-group__ie__dev__api__system__conf_1gada020cb5069326ca18dff97b7564948a:
.. index:: pair: function; with_cpu_x86_avx

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::with_cpu_x86_avx()

Checks whether CPU supports AVX capability.



.. rubric:: Returns:

``True`` is AVX instructions are available, ``false`` otherwise

.. _doxid-group__ie__dev__api__system__conf_1gadf27a09b4f47d98f9162d5256f7bae4c:
.. index:: pair: function; with_cpu_x86_avx2

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::with_cpu_x86_avx2()

Checks whether CPU supports AVX2 capability.



.. rubric:: Returns:

``True`` is AVX2 instructions are available, ``false`` otherwise

.. _doxid-group__ie__dev__api__system__conf_1ga865cfc186254bcc13cc0c39441879b8d:
.. index:: pair: function; with_cpu_x86_avx512f

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::with_cpu_x86_avx512f()

Checks whether CPU supports AVX 512 capability.



.. rubric:: Returns:

``True`` is AVX512F (foundation) instructions are available, ``false`` otherwise

.. _doxid-group__ie__dev__api__system__conf_1ga3cf444492c290b36e82267ff4e7d20a8:
.. index:: pair: function; with_cpu_x86_avx512_core

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::with_cpu_x86_avx512_core()

Checks whether CPU supports AVX 512 capability.



.. rubric:: Returns:

``True`` is AVX512F, AVX512BW, AVX512DQ instructions are available, ``false`` otherwise

.. _doxid-group__ie__dev__api__system__conf_1gad31c357806f14f6ccec66e102a0c32f3:
.. index:: pair: function; with_cpu_x86_bfloat16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool InferenceEngine::with_cpu_x86_bfloat16()

Checks whether CPU supports BFloat16 capability.



.. rubric:: Returns:

``True`` is tAVX512_BF16 instructions are available, ``false`` otherwise

