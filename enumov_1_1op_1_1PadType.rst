.. index:: pair: enum; PadType
.. _doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d:

enum ov::op::PadType
====================

Overview
~~~~~~~~

Padding Type used for ``Convolution`` and ``Pooling`` :ref:`More...<details-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>

	enum PadType
	{
	    :target:`EXPLICIT<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50da440806ada035e97a59ec9d2ca6796cb3>`   = 0,
	    :target:`SAME_LOWER<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50daf08c70df2e892cd73d4c44b3c1f34dc9>`,
	    :target:`SAME_UPPER<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50da257c89fec8995dc50bc0e29c981ae0d6>`,
	    :target:`VALID<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50dac9f1a6384b1c466d4612f513bd8e13ea>`,
	    :target:`AUTO<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50dae1f2d5134ed2543d38a0de9751cf75d9>`       = SAME_UPPER,
	    :target:`NOTSET<doxid-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50da13394d6014d163e223e5cc7e0ebd0ec3>`     = EXPLICIT,
	};

.. _details-namespaceov_1_1op_1a287af03f211ecac2b876d35a1130e50d:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Padding Type used for ``Convolution`` and ``Pooling``

Follows ONNX padding type definitions EXPLICIT - Pad dimensions are explicity specified SAME_LOWER - Pad dimensions computed to match input shape Ceil(num_dims/2) at the beginning and Floor(num_dims/2) at the end SAME_UPPER - Pad dimensions computed to match input shape Floor(num_dims/2) at the beginning and Ceil(num_dims/2) at the end VALID - No padding AUTO - Deprecated. User should not use it in the future NOTSET - Deprecated. User should not use it in the future

