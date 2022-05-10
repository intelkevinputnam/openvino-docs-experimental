.. index:: pair: struct; InferenceEngine::QueryNetworkResult
.. _doxid-struct_inference_engine_1_1_query_network_result:

struct InferenceEngine::QueryNetworkResult
==========================================



Overview
~~~~~~~~

Response structure encapsulating information about supported layer. :ref:`More...<details-struct_inference_engine_1_1_query_network_result>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>
	
	struct QueryNetworkResult
	{
		// fields
	
		std::map<std::string, std::string> :ref:`supportedLayersMap<doxid-struct_inference_engine_1_1_query_network_result_1aff431e5d7451f364dee1c1c54ca78333>`;
		:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`rc<doxid-struct_inference_engine_1_1_query_network_result_1a4cc512d1eb0806ecf1d0b79c7f6283e2>` = :ref:`OK<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>`;
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` :ref:`resp<doxid-struct_inference_engine_1_1_query_network_result_1a61620288e17695f9c5a6761fde1c828e>`;
	};
.. _details-struct_inference_engine_1_1_query_network_result:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Response structure encapsulating information about supported layer.

Fields
------

.. _doxid-struct_inference_engine_1_1_query_network_result_1aff431e5d7451f364dee1c1c54ca78333:
.. index:: pair: variable; supportedLayersMap

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, std::string> supportedLayersMap

A map of supported layers:

* key - a layer name

* value - a device name on which layer is assigned

.. _doxid-struct_inference_engine_1_1_query_network_result_1a4cc512d1eb0806ecf1d0b79c7f6283e2:
.. index:: pair: variable; rc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` rc = :ref:`OK<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>`

A status code.

.. _doxid-struct_inference_engine_1_1_query_network_result_1a61620288e17695f9c5a6761fde1c828e:
.. index:: pair: variable; resp

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` resp

Response message.


