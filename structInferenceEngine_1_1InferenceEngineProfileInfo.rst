.. index:: pair: struct; InferenceEngine::InferenceEngineProfileInfo
.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info:

struct InferenceEngine::InferenceEngineProfileInfo
==================================================

.. toctree::
	:hidden:

	LayerStatus <enumInferenceEngine_1_1InferenceEngineProfileInfo_1_1LayerStatus.rst>

Overview
~~~~~~~~

Represents basic inference profiling information per layer. :ref:`More...<details-struct_inference_engine_1_1_inference_engine_profile_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>
	
	struct InferenceEngineProfileInfo
	{
		// enums
	
		enum :ref:`LayerStatus<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1>`;

		// fields
	
		:ref:`LayerStatus<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1>` :ref:`status<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a08c20f10575a838a22d339d05f03b35e>`;
		long long :ref:`realTime_uSec<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a38ebc89f685e65ffe28a9542b465eb82>`;
		long long :ref:`cpu_uSec<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a0647e922783e6b54859dad7cdc26f16c>`;
		char :ref:`exec_type<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1acfdae8c0fc022e09e872bc5ee9f981ba>`[256] = {};
		char :ref:`layer_type<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a5ad060fc227cdf5cf64970c156485c9d>`[256] = {};
		unsigned :ref:`execution_index<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1ab89fe5ad0f6e2f44b93e92de43a0d9c4>`;
	};
.. _details-struct_inference_engine_1_1_inference_engine_profile_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents basic inference profiling information per layer.

If the layer is executed using tiling, the sum time per each tile is indicated as the total execution time. Due to parallel execution, the total execution time for all layers might be greater than the total inference time.

Fields
------

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a08c20f10575a838a22d339d05f03b35e:
.. index:: pair: variable; status

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`LayerStatus<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1>` status

Defines a layer status.

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a38ebc89f685e65ffe28a9542b465eb82:
.. index:: pair: variable; realTime_uSec

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	long long realTime_uSec

The absolute time in microseconds that the layer ran (in total)

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a0647e922783e6b54859dad7cdc26f16c:
.. index:: pair: variable; cpu_uSec

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	long long cpu_uSec

The net host cpu time that the layer ran.

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1acfdae8c0fc022e09e872bc5ee9f981ba:
.. index:: pair: variable; exec_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	char exec_type[256] = {}

An execution type of unit.

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a5ad060fc227cdf5cf64970c156485c9d:
.. index:: pair: variable; layer_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	char layer_type[256] = {}

A layer type.

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1ab89fe5ad0f6e2f44b93e92de43a0d9c4:
.. index:: pair: variable; execution_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned execution_index

An execution index of the unit.


