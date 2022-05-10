.. index:: pair: struct; InferenceEngine::DataConfig
.. _doxid-struct_inference_engine_1_1_data_config:

struct InferenceEngine::DataConfig
==================================



Overview
~~~~~~~~

This structure describes data configuration. :ref:`More...<details-struct_inference_engine_1_1_data_config>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iextension.h>
	
	struct DataConfig
	{
		// fields
	
		:ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>` :ref:`desc<doxid-struct_inference_engine_1_1_data_config_1af43e585030006f91039e0144292b575f>`;
		int :ref:`inPlace<doxid-struct_inference_engine_1_1_data_config_1afe6f8028187d9e6e4473a51b0a637bc3>` = -1;
		bool :ref:`constant<doxid-struct_inference_engine_1_1_data_config_1a750da88291507f561b20f41c10872a11>` = false;
	};
.. _details-struct_inference_engine_1_1_data_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This structure describes data configuration.

Fields
------

.. _doxid-struct_inference_engine_1_1_data_config_1af43e585030006f91039e0144292b575f:
.. index:: pair: variable; desc

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>` desc

Format of memory descriptor.

.. _doxid-struct_inference_engine_1_1_data_config_1afe6f8028187d9e6e4473a51b0a637bc3:
.. index:: pair: variable; inPlace

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int inPlace = -1

Index of in-place memory. If -1 memory cannot be in-place.

.. _doxid-struct_inference_engine_1_1_data_config_1a750da88291507f561b20f41c10872a11:
.. index:: pair: variable; constant

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool constant = false

Flag for determination of the constant memory. If layer contains all constant memory we can calculate it on the load stage.


