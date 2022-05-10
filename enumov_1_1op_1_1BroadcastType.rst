.. index:: pair: enum; BroadcastType
.. _doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea:

enum ov::op::BroadcastType
==========================

Overview
~~~~~~~~

BroadcastType specifies rules used for mapping of input tensor axes to output shape axes. :ref:`More...<details-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>

	enum BroadcastType
	{
	    :target:`NONE<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdeaab50339a10e1de285ac99d4c3990b8693>`,
	    :target:`EXPLICIT<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdeaa440806ada035e97a59ec9d2ca6796cb3>`      = NONE,
	    :target:`NUMPY<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdeaad677ba7339dd3c0243cd3257b80be8f5>`,
	    :target:`PDPD<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdeaa837f6a16db4fb3733ec2211baa44e56b>`,
	    :target:`BIDIRECTIONAL<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdeaa01ca2e75004bdf2618045f428595ef08>`,
	};

.. _details-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

BroadcastType specifies rules used for mapping of input tensor axes to output shape axes.

Broadcasting rules are different for Broadcast op and for element-wise ops. :ref:`AutoBroadcastType::NUMPY <doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219acead677ba7339dd3c0243cd3257b80be8f5>` is equivalent of :ref:`BroadcastType::BIDIRECTIONAL <doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdeaab50339a10e1de285ac99d4c3990b8693>` according to spec.

EXPLICIT - Mapping of the input data shape to output shape based on axes_mapping input. NUMPY - Numpy broadcasting rules, aligned with ONNX Broadcasting. (`https://github.com/onnx/onnx/blob/master/docs/Broadcasting.md <https://github.com/onnx/onnx/blob/master/docs/Broadcasting.md>`__) PDPD - PaddlePaddle-style implicit broadcasting. For more informaction see AutoBroadcastType documentation. BIDIRECTIONAL - The broadcast rule is similar to numpy.array(input) \* numpy.ones(target_shape). Dimensions are right alignment.

