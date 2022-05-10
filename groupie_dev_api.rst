.. index:: pair: group; Inference Engine Plugin API
.. _doxid-group__ie__dev__api:

Inference Engine Plugin API
===========================

.. toctree::
	:hidden:

	groupie_dev_api_async_infer_request_api.rst
	groupie_dev_api_memory.rst
	groupie_dev_api_error_debug.rst
	groupie_dev_api_exec_network_api.rst
	groupie_dev_exec_graph.rst
	groupie_dev_api_precision.rst
	groupie_dev_api_file_utils.rst
	groupie_dev_profiling.rst
	groupie_dev_api_infer_request_api.rst
	groupie_dev_api_plugin_api.rst
	groupie_dev_api_preproc_api.rst
	groupie_dev_api_system_conf.rst
	groupie_dev_api_threading.rst
	groupie_dev_api_variable_state_api.rst
	groupie_dev_api_xml.rst

Overview
~~~~~~~~

Defines Inference Engine Plugin API which can be used in plugin development. :ref:`More...<details-group__ie__dev__api>`

|	:ref:`Asynchronous Inference Request base classes<doxid-group__ie__dev__api__async__infer__request__api>`
|	:ref:`Blob creation and memory utilities<doxid-group__ie__dev__api__memory>`
|	:ref:`Error handling and debug helpers<doxid-group__ie__dev__api__error__debug>`
|	:ref:`Executable Network base classes<doxid-group__ie__dev__api__exec__network__api>`
|	:ref:`Execution graph utilities<doxid-group__ie__dev__exec__graph>`
|	:ref:`FP16 to FP32 precision utilities<doxid-group__ie__dev__api__precision>`
|	:ref:`File utilities<doxid-group__ie__dev__api__file__utils>`
|	:ref:`ITT profiling utilities<doxid-group__ie__dev__profiling>`
|	:ref:`Inference Request base classes<doxid-group__ie__dev__api__infer__request__api>`
|	:ref:`Plugin base classes<doxid-group__ie__dev__api__plugin__api>`
|	:ref:`Preprocessing API<doxid-group__ie__dev__api__preproc__api>`
|	:ref:`System configuration utilities<doxid-group__ie__dev__api__system__conf>`
|	:ref:`Threading utilities<doxid-group__ie__dev__api__threading>`
|	:ref:`Variable state base classes<doxid-group__ie__dev__api__variable__state__api>`
|	:ref:`XML helper utilities<doxid-group__ie__dev__api__xml>`



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// macros

	#define :ref:`IE_SET_METRIC_RETURN<doxid-group__ie__dev__api_1gad59db954d9dfcbd6f490d5cbadd3a91d>`(name, ...)

.. _details-group__ie__dev__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Defines Inference Engine Plugin API which can be used in plugin development.

Macros
------

.. _doxid-group__ie__dev__api_1gad59db954d9dfcbd6f490d5cbadd3a91d:
.. index:: pair: define; IE_SET_METRIC_RETURN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define IE_SET_METRIC_RETURN(name, ...)

Return metric value with specified ``name`` and arguments ``...``. Example:

.. ref-code-block:: cpp

	IE_SET_METRIC_RETURN(SUPPORTED_CONFIG_KEYS, configKeys);



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- The metric name

	*
		- ...

		- A metric value



.. rubric:: Returns:

A metric value wrapped with Parameter and returned to a calling function

