.. index:: pair: enum; LayerStatus
.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1:

enum InferenceEngine::InferenceEngineProfileInfo::LayerStatus
=============================================================

Overview
~~~~~~~~

Defines the general status of the layer. :ref:`More...<details-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>

	enum LayerStatus
	{
	    :ref:`NOT_RUN<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1a2c811afb1bb9571abaffb3fab305e77e>`,
	    :ref:`OPTIMIZED_OUT<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1a57014341061bbea3f549beb414954eae>`,
	    :ref:`EXECUTED<doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1aa243218826d16402f45a1355f72dea2b>`,
	};

.. _details-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Defines the general status of the layer.

Enum Values
-----------

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1a2c811afb1bb9571abaffb3fab305e77e:
.. index:: pair: enumvalue; NOT_RUN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NOT_RUN

A layer is not executed.

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1a57014341061bbea3f549beb414954eae:
.. index:: pair: enumvalue; OPTIMIZED_OUT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OPTIMIZED_OUT

A layer is optimized out during graph optimization phase.

.. _doxid-struct_inference_engine_1_1_inference_engine_profile_info_1a7f91020e3d0aac48028e9af8532f2ec1aa243218826d16402f45a1355f72dea2b:
.. index:: pair: enumvalue; EXECUTED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	EXECUTED

A layer is executed.

