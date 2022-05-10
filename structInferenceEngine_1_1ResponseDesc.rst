.. index:: pair: struct; InferenceEngine::ResponseDesc
.. _doxid-struct_inference_engine_1_1_response_desc:

struct InferenceEngine::ResponseDesc
====================================



Overview
~~~~~~~~

Represents detailed information for an error. :ref:`More...<details-struct_inference_engine_1_1_response_desc>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>
	
	struct ResponseDesc
	{
		// fields
	
		char :ref:`msg<doxid-struct_inference_engine_1_1_response_desc_1a0dc42a68d648c442024701821cb3932b>`[4096] = {};
	};
.. _details-struct_inference_engine_1_1_response_desc:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents detailed information for an error.

Fields
------

.. _doxid-struct_inference_engine_1_1_response_desc_1a0dc42a68d648c442024701821cb3932b:
.. index:: pair: variable; msg

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	char msg[4096] = {}

A character buffer that holds the detailed information for an error.


