.. index:: pair: enum; ePrecision
.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5:

enum InferenceEngine::Precision::ePrecision
===========================================

Overview
~~~~~~~~

Enum to specify of different :ref:`More...<details-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_precision.hpp>

	enum ePrecision
	{
	    :ref:`UNSPECIFIED<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ae27ff65d395667d17067e83d932a2045>` = 255,
	    :ref:`MIXED<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ab67b94da53b4d2647cdfa29f57bea362>`       = 0,
	    :ref:`FP32<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a6b062312b968a46ae0baf14cc3665e1e>`        = 10,
	    :ref:`FP16<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a084e737560206865337ee681e1ab3f5a>`        = 11,
	    :ref:`BF16<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ace458a2eaf16d910e3e0e6e2a5966d2f>`        = 12,
	    :ref:`FP64<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a05bded0b5cd274b929954f845bdee385>`        = 13,
	    :ref:`Q78<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5abaa262d8c717d8b16ff085b62f68d163>`         = 20,
	    :ref:`I16<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5acb529fb6affc93bd897333da1756e54b>`         = 30,
	    :ref:`U4<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a2cd927591fb6d9c2e4041c5fb726a057>`          = 39,
	    :ref:`U8<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a046eaf31a4345f526ed54271c9fcd39c>`          = 40,
	    :ref:`I4<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a40b682c77a46aa61ca5f038772616b2a>`          = 49,
	    :ref:`I8<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a8a21a034db6e5da6861616dd892aed2a>`          = 50,
	    :ref:`U16<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5af08511de719988ce14d1467d837392fb>`         = 60,
	    :ref:`I32<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a5eaacac79637b058ffbb485829175d4c>`         = 70,
	    :ref:`U32<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a75a3621c5cc0ee94276a5e6648531987>`         = 74,
	    :ref:`I64<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a76288d38cc52b68fb2127a4eb84b3b80>`         = 72,
	    :ref:`U64<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a73a312dd48d0a518058957e9274032e4>`         = 73,
	    :ref:`BIN<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a04340bc865507e636c5d68c02ab52f6a>`         = 71,
	    :ref:`BOOL<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5aface3f3b02da8cb34d69df843ab7cdf2>`        = 41,
	    :ref:`CUSTOM<doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ab07bc8316c525eaca480427e2bd134bd>`      = 80,
	};

.. _details-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to specify of different

Enum Values
-----------

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ae27ff65d395667d17067e83d932a2045:
.. index:: pair: enumvalue; UNSPECIFIED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	UNSPECIFIED

Unspecified value. Used by default

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ab67b94da53b4d2647cdfa29f57bea362:
.. index:: pair: enumvalue; MIXED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MIXED

Mixed value. Can be received from network. No applicable for tensors

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a6b062312b968a46ae0baf14cc3665e1e:
.. index:: pair: enumvalue; FP32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FP32

32bit floating point value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a084e737560206865337ee681e1ab3f5a:
.. index:: pair: enumvalue; FP16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FP16

16bit floating point value, 5 bit for exponent, 10 bit for mantisa

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ace458a2eaf16d910e3e0e6e2a5966d2f:
.. index:: pair: enumvalue; BF16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BF16

16bit floating point value, 8 bit for exponent, 7 bit for mantisa

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a05bded0b5cd274b929954f845bdee385:
.. index:: pair: enumvalue; FP64

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FP64

64bit floating point value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5abaa262d8c717d8b16ff085b62f68d163:
.. index:: pair: enumvalue; Q78

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Q78

16bit specific signed fixed point precision

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5acb529fb6affc93bd897333da1756e54b:
.. index:: pair: enumvalue; I16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I16

16bit signed integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a2cd927591fb6d9c2e4041c5fb726a057:
.. index:: pair: enumvalue; U4

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U4

4bit unsigned integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a046eaf31a4345f526ed54271c9fcd39c:
.. index:: pair: enumvalue; U8

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U8

8bit unsigned integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a40b682c77a46aa61ca5f038772616b2a:
.. index:: pair: enumvalue; I4

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I4

4bit signed integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a8a21a034db6e5da6861616dd892aed2a:
.. index:: pair: enumvalue; I8

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I8

8bit signed integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5af08511de719988ce14d1467d837392fb:
.. index:: pair: enumvalue; U16

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U16

16bit unsigned integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a5eaacac79637b058ffbb485829175d4c:
.. index:: pair: enumvalue; I32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I32

32bit signed integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a75a3621c5cc0ee94276a5e6648531987:
.. index:: pair: enumvalue; U32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U32

32bit unsigned integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a76288d38cc52b68fb2127a4eb84b3b80:
.. index:: pair: enumvalue; I64

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I64

64bit signed integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a73a312dd48d0a518058957e9274032e4:
.. index:: pair: enumvalue; U64

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U64

64bit unsigned integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5a04340bc865507e636c5d68c02ab52f6a:
.. index:: pair: enumvalue; BIN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BIN

1bit integer value

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5aface3f3b02da8cb34d69df843ab7cdf2:
.. index:: pair: enumvalue; BOOL

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BOOL

8bit bool type

.. _doxid-class_inference_engine_1_1_precision_1ade75bd7073b4aa966c0dda4025bcd0f5ab07bc8316c525eaca480427e2bd134bd:
.. index:: pair: enumvalue; CUSTOM

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CUSTOM

custom precision has it's own name and size of elements

