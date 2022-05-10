.. index:: pair: group; Execution graph utilities
.. _doxid-group__ie__dev__exec__graph:

Execution graph utilities
=========================

.. toctree::
	:hidden:

	ExecGraphInfoSerialization <namespaceExecGraphInfoSerialization.rst>
	ExecutionNode <classExecGraphInfoSerialization_1_1ExecutionNode.rst>

Overview
~~~~~~~~

Contains ``ExecutionNode`` and its properties. :ref:`More...<details-group__ie__dev__exec__graph>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`ExecGraphInfoSerialization<doxid-namespace_exec_graph_info_serialization>`;

	// classes

	class :ref:`ExecGraphInfoSerialization::ExecutionNode<doxid-class_exec_graph_info_serialization_1_1_execution_node>`;

	// global variables

	static const char :ref:`ExecGraphInfoSerialization::ORIGINAL_NAMES<doxid-group__ie__dev__exec__graph_1gaf81db1d9eb4732d48ab5dbfa78d9e238>`[] = "originalLayersNames";
	static const char :ref:`ExecGraphInfoSerialization::IMPL_TYPE<doxid-group__ie__dev__exec__graph_1ga9e563af5a735a50f00db6aaf0b637f20>`[] = "primitiveType";
	static const char :ref:`ExecGraphInfoSerialization::OUTPUT_PRECISIONS<doxid-group__ie__dev__exec__graph_1ga9404c4010efbba1234c898d83539326a>`[] = "outputPrecisions";
	static const char :ref:`ExecGraphInfoSerialization::PERF_COUNTER<doxid-group__ie__dev__exec__graph_1ga94fe83ba1c48c33804219b0f5a4303f0>`[] = "execTimeMcs";
	static const char :ref:`ExecGraphInfoSerialization::OUTPUT_LAYOUTS<doxid-group__ie__dev__exec__graph_1ga7e9a63a77266338179a131f290a291be>`[] = "outputLayouts";
	static const char :ref:`ExecGraphInfoSerialization::EXECUTION_ORDER<doxid-group__ie__dev__exec__graph_1ga68ee1085f7ce85d6fdb4a7b3570bbeac>`[] = "execOrder";
	static const char :ref:`ExecGraphInfoSerialization::LAYER_TYPE<doxid-group__ie__dev__exec__graph_1ga10c7fd3a4016b25f347391aa4fe589e9>`[] = "layerType";
	static const char :ref:`ExecGraphInfoSerialization::RUNTIME_PRECISION<doxid-group__ie__dev__exec__graph_1ga56b675ce34cb7a58a79a21694fa63896>`[] = "runtimePrecision";

.. _details-group__ie__dev__exec__graph:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Contains ``ExecutionNode`` and its properties.

Global Variables
----------------

.. _doxid-group__ie__dev__exec__graph_1gaf81db1d9eb4732d48ab5dbfa78d9e238:
.. index:: pair: variable; ORIGINAL_NAMES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::ORIGINAL_NAMES[] = "originalLayersNames"

Used to get a string of layer names separated by a comma from the original IR, which were fused/merged to the current executable primitive.

.. _doxid-group__ie__dev__exec__graph_1ga9e563af5a735a50f00db6aaf0b637f20:
.. index:: pair: variable; IMPL_TYPE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::IMPL_TYPE[] = "primitiveType"

Used to get a type of the executable primitive.

.. _doxid-group__ie__dev__exec__graph_1ga9404c4010efbba1234c898d83539326a:
.. index:: pair: variable; OUTPUT_PRECISIONS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::OUTPUT_PRECISIONS[] = "outputPrecisions"

Used to get output precisions of the executable primitive.

.. _doxid-group__ie__dev__exec__graph_1ga94fe83ba1c48c33804219b0f5a4303f0:
.. index:: pair: variable; PERF_COUNTER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::PERF_COUNTER[] = "execTimeMcs"

Used to get a value of execution time of the executable primitive.

.. _doxid-group__ie__dev__exec__graph_1ga7e9a63a77266338179a131f290a291be:
.. index:: pair: variable; OUTPUT_LAYOUTS

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::OUTPUT_LAYOUTS[] = "outputLayouts"

Used to get output layouts of primitive.

.. _doxid-group__ie__dev__exec__graph_1ga68ee1085f7ce85d6fdb4a7b3570bbeac:
.. index:: pair: variable; EXECUTION_ORDER

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::EXECUTION_ORDER[] = "execOrder"

Used to get an execution order of primitive.

.. _doxid-group__ie__dev__exec__graph_1ga10c7fd3a4016b25f347391aa4fe589e9:
.. index:: pair: variable; LAYER_TYPE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::LAYER_TYPE[] = "layerType"

Used to get a type of primitive.

.. _doxid-group__ie__dev__exec__graph_1ga56b675ce34cb7a58a79a21694fa63896:
.. index:: pair: variable; RUNTIME_PRECISION

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const char ExecGraphInfoSerialization::RUNTIME_PRECISION[] = "runtimePrecision"

Used to get runtime precision of the executable primitive.

