.. index:: pair: enum; AutoBroadcastType
.. _doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace:

enum ov::op::AutoBroadcastType
==============================

Overview
~~~~~~~~

Specifies the algorithm to use for implicit broadcasting of a tensor to align with another tensor. :ref:`More...<details-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>

	enum AutoBroadcastType
	{
	    :target:`NONE<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219aceab50339a10e1de285ac99d4c3990b8693>`     = 0,
	    :target:`EXPLICIT<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219acea440806ada035e97a59ec9d2ca6796cb3>` = NONE,
	    :target:`NUMPY<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219acead677ba7339dd3c0243cd3257b80be8f5>`,
	    :target:`PDPD<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219acea837f6a16db4fb3733ec2211baa44e56b>`,
	};

.. _details-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Specifies the algorithm to use for implicit broadcasting of a tensor to align with another tensor.

NONE - No implicit broadcasting of tensor NUMPY - Numpy-style implicit broadcasting (`https://docs.scipy.org/doc/numpy/user/basics.broadcasting.html <https://docs.scipy.org/doc/numpy/user/basics.broadcasting.html>`__) Right-align dimensions of the two tensors, with missing dimensions treated as size 1 dimensions. After alignment, for each dimension, their sizes should either match or one of them should be of size 1. Size 1 dimension will be implicitly broadcast to match the other size.

E.g., A: Shape(2, 1, 6) B: Shape(   3, 1) Result: Shape(2, 3, 6)

.. code-block:: cpp

	A: Shape(2, 1, 6)
	B: Shape(   3, 1)

Result: Shape(2, 3, 6) PDPD - PaddlePaddle-style implicit broadcasting (`https://github.com/PaddlePaddle/Paddle/blob/release/1.5/paddle/ <https://github.com/PaddlePaddle/Paddle/blob/release/1.5/paddle/>`__ fluid/operators/elementwise/elementwise_op.h#L126) Broadcast B to match the shape of A, where axis is the start dimension index to align B with A. If axis is -1 (default), i axis = rank(A) - rank(B). The trailing dimensions of size 1 for B will be ignored.

E.g., A: Shape(2, 3, 4, 5) B: Shape(   3, 4   ) with axis =1 Result: Shape(2, 3, 4, 5)

.. code-block:: cpp

	A: Shape(2, 3, 4, 5)
	B: Shape(   3, 1   ) with axis = 1

Result: Shape(2, 3, 4, 5)

