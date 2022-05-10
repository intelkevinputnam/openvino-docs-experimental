.. index:: pair: struct; ov::ProfilingInfo
.. _doxid-structov_1_1_profiling_info:

struct ov::ProfilingInfo
========================

.. toctree::
	:hidden:

	Status <enumov_1_1ProfilingInfo_1_1Status.rst>

Overview
~~~~~~~~

Represents basic inference profiling information per operation. :ref:`More...<details-structov_1_1_profiling_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <profiling_info.hpp>
	
	struct ProfilingInfo
	{
		// enums
	
		enum :ref:`Status<doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7>`;

		// fields
	
		:ref:`Status<doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7>` :ref:`status<doxid-structov_1_1_profiling_info_1a8e0ec4319e7b6e3b05e49b4ef1028d9e>`;
		std::chrono::microseconds :ref:`real_time<doxid-structov_1_1_profiling_info_1a481564f9de7a933535ff48d3b535307b>`;
		std::chrono::microseconds :ref:`cpu_time<doxid-structov_1_1_profiling_info_1aa013e3f58e82a4debfa9fa56940915a5>`;
		std::string :ref:`node_name<doxid-structov_1_1_profiling_info_1af10e703055803c894dfe70695aee2d5f>`;
		std::string :ref:`exec_type<doxid-structov_1_1_profiling_info_1ab47c33cd02422e215d5d5c4d2021bb59>`;
		std::string :ref:`node_type<doxid-structov_1_1_profiling_info_1a72f849b69a91ea1312aa98a78ebebf6d>`;
	};
.. _details-structov_1_1_profiling_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents basic inference profiling information per operation.

If the operation is executed using tiling, the sum time per each tile is indicated as the total execution time. Due to parallel execution, the total execution time for all nodes might be greater than the total inference time.

Fields
------

.. _doxid-structov_1_1_profiling_info_1a8e0ec4319e7b6e3b05e49b4ef1028d9e:
.. index:: pair: variable; status

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Status<doxid-structov_1_1_profiling_info_1ac035f26c2e5a11a5126be894de2ad4f7>` status

Defines the node status.

.. _doxid-structov_1_1_profiling_info_1a481564f9de7a933535ff48d3b535307b:
.. index:: pair: variable; real_time

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::chrono::microseconds real_time

The absolute time, in microseconds, that the node ran (in total).

.. _doxid-structov_1_1_profiling_info_1aa013e3f58e82a4debfa9fa56940915a5:
.. index:: pair: variable; cpu_time

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::chrono::microseconds cpu_time

The net host CPU time that the node ran.

.. _doxid-structov_1_1_profiling_info_1af10e703055803c894dfe70695aee2d5f:
.. index:: pair: variable; node_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string node_name

Name of a node.

.. _doxid-structov_1_1_profiling_info_1ab47c33cd02422e215d5d5c4d2021bb59:
.. index:: pair: variable; exec_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string exec_type

Execution type of a unit.

.. _doxid-structov_1_1_profiling_info_1a72f849b69a91ea1312aa98a78ebebf6d:
.. index:: pair: variable; node_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string node_type

:ref:`Node <doxid-classov_1_1_node>` type.


