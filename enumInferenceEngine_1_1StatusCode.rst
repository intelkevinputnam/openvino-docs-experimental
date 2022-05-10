.. index:: pair: enum; StatusCode
.. _doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421:

enum InferenceEngine::StatusCode
================================

This enum contains codes for all possible return values of the interface functions.

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>

	enum StatusCode
	{
	    :target:`OK<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a084fcaf510851d3281e7bd45db802c6a>`                 = 0,
	    :target:`GENERAL_ERROR<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421ac5630ab9af84851fe197378f485af3f1>`      = -1,
	    :target:`NOT_IMPLEMENTED<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a9b40bf6694a2919cf1d03effbd80ec19>`    = -2,
	    :target:`NETWORK_NOT_LOADED<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421acf6bce4716b01d7ba223f837227e9f05>` = -3,
	    :target:`PARAMETER_MISMATCH<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a10cdc8dcea92a1bbea47ceb441872612>` = -4,
	    :target:`NOT_FOUND<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a53a45e2ce37e8ea26c4331989fa56649>`          = -5,
	    :target:`OUT_OF_BOUNDS<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a3ce0772e6367175b5a7434dbaa618378>`      = -6,
	    :target:`UNEXPECTED<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a9bcb08519b3e8ea3828770e4990da53e>`         = -7,
	    :target:`REQUEST_BUSY<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a51ec51acb7cae028fcce0f8832b587bb>`       = -8,
	    :target:`RESULT_NOT_READY<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a83d9d02bebb41b37eda89b5f3ed1f988>`   = -9,
	    :target:`NOT_ALLOCATED<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421aa8e8a8f0000a5fba549f12f603ac18b9>`      = -10,
	    :target:`INFER_NOT_STARTED<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421af61241a8558327b003e5f71615eab3cf>`  = -11,
	    :target:`NETWORK_NOT_READ<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421aa216881847c0e7fe3e94d3efbd46c29b>`   = -12,
	    :target:`INFER_CANCELLED<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421a9a1fe5d76aaedcf943c9b04488f92b55>`    = -13,
	};

