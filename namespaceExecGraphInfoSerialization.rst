.. index:: pair: namespace; ExecGraphInfoSerialization
.. _doxid-namespace_exec_graph_info_serialization:

namespace ExecGraphInfoSerialization
====================================

.. toctree::
	:hidden:

A namespace with const values for Execution Graph parameters names.

Executable Graph Info is represented in CNNNetwork format with general :ref:`ExecutionNode <doxid-class_exec_graph_info_serialization_1_1_execution_node>` nodes inside including connections between the nodes. Each node describes an executable hardware-specific primitive and stores its parameters within :ref:`ExecutionNode::get_rt_info <doxid-classov_1_1_node_1a5c73794fbc47e510198261d61682fe79>` map. There is a list of general keys for the parameters map.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace ExecGraphInfoSerialization {

	// classes

	class :ref:`ExecutionNode<doxid-class_exec_graph_info_serialization_1_1_execution_node>`;

	// global variables

	static const char :ref:`ORIGINAL_NAMES<doxid-group__ie__dev__exec__graph_1gaf81db1d9eb4732d48ab5dbfa78d9e238>`[] = "originalLayersNames";
	static const char :ref:`IMPL_TYPE<doxid-group__ie__dev__exec__graph_1ga9e563af5a735a50f00db6aaf0b637f20>`[] = "primitiveType";
	static const char :ref:`OUTPUT_PRECISIONS<doxid-group__ie__dev__exec__graph_1ga9404c4010efbba1234c898d83539326a>`[] = "outputPrecisions";
	static const char :ref:`PERF_COUNTER<doxid-group__ie__dev__exec__graph_1ga94fe83ba1c48c33804219b0f5a4303f0>`[] = "execTimeMcs";
	static const char :ref:`OUTPUT_LAYOUTS<doxid-group__ie__dev__exec__graph_1ga7e9a63a77266338179a131f290a291be>`[] = "outputLayouts";
	static const char :ref:`EXECUTION_ORDER<doxid-group__ie__dev__exec__graph_1ga68ee1085f7ce85d6fdb4a7b3570bbeac>`[] = "execOrder";
	static const char :ref:`LAYER_TYPE<doxid-group__ie__dev__exec__graph_1ga10c7fd3a4016b25f347391aa4fe589e9>`[] = "layerType";
	static const char :ref:`RUNTIME_PRECISION<doxid-group__ie__dev__exec__graph_1ga56b675ce34cb7a58a79a21694fa63896>`[] = "runtimePrecision";

	} // namespace ExecGraphInfoSerialization
