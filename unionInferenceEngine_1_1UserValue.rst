.. index:: pair: union; InferenceEngine::UserValue
.. _doxid-union_inference_engine_1_1_user_value:

union InferenceEngine::UserValue
================================



Overview
~~~~~~~~

The method holds the user values to enable binding of data per graph node. :ref:`More...<details-union_inference_engine_1_1_user_value>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>
	
	union UserValue
	{
		// fields
	
		int :ref:`v_int<doxid-union_inference_engine_1_1_user_value_1acd6cc4ba808973ca4e84313edd62c153>`;
		float :ref:`v_float<doxid-union_inference_engine_1_1_user_value_1aa8c0eaa29652972259ea2794efcc7422>`;
		void \* :ref:`v_ptr<doxid-union_inference_engine_1_1_user_value_1a15067d736dde3d62c0bcb3a8ba138bd7>`;
	};
.. _details-union_inference_engine_1_1_user_value:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

The method holds the user values to enable binding of data per graph node.

Fields
------

.. _doxid-union_inference_engine_1_1_user_value_1acd6cc4ba808973ca4e84313edd62c153:
.. index:: pair: variable; v_int

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int v_int

An integer value.

.. _doxid-union_inference_engine_1_1_user_value_1aa8c0eaa29652972259ea2794efcc7422:
.. index:: pair: variable; v_float

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	float v_float

A floating point value.

.. _doxid-union_inference_engine_1_1_user_value_1a15067d736dde3d62c0bcb3a8ba138bd7:
.. index:: pair: variable; v_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void \* v_ptr

A pointer to a void.


