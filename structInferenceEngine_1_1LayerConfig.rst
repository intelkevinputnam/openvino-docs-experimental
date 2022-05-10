.. index:: pair: struct; InferenceEngine::LayerConfig
.. _doxid-struct_inference_engine_1_1_layer_config:

struct InferenceEngine::LayerConfig
===================================



Overview
~~~~~~~~

This structure describes Layer configuration. :ref:`More...<details-struct_inference_engine_1_1_layer_config>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iextension.h>
	
	struct LayerConfig
	{
		// fields
	
		bool :ref:`dynBatchSupport<doxid-struct_inference_engine_1_1_layer_config_1a31bd118feaf9c53b2532899c64fe44b5>` = false;
		std::vector<:ref:`DataConfig<doxid-struct_inference_engine_1_1_data_config>`> :ref:`inConfs<doxid-struct_inference_engine_1_1_layer_config_1a4e8a1dd13843a80704a093c2b138ebe3>`;
		std::vector<:ref:`DataConfig<doxid-struct_inference_engine_1_1_data_config>`> :ref:`outConfs<doxid-struct_inference_engine_1_1_layer_config_1af3aba853c047b1cf64788ddfc2d1b499>`;
	};
.. _details-struct_inference_engine_1_1_layer_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This structure describes Layer configuration.

Fields
------

.. _doxid-struct_inference_engine_1_1_layer_config_1a31bd118feaf9c53b2532899c64fe44b5:
.. index:: pair: variable; dynBatchSupport

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool dynBatchSupport = false

Supported dynamic batch. If false, dynamic batch is not supported.

.. _doxid-struct_inference_engine_1_1_layer_config_1a4e8a1dd13843a80704a093c2b138ebe3:
.. index:: pair: variable; inConfs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`DataConfig<doxid-struct_inference_engine_1_1_data_config>`> inConfs

Vector of input data configs.

.. _doxid-struct_inference_engine_1_1_layer_config_1af3aba853c047b1cf64788ddfc2d1b499:
.. index:: pair: variable; outConfs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`DataConfig<doxid-struct_inference_engine_1_1_data_config>`> outConfs

Vector of output data configs.


