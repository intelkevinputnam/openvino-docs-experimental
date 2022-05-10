.. index:: pair: enum; Layout
.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8:

enum InferenceEngine::Layout
============================

Overview
~~~~~~~~

Layouts that the inference engine supports. :ref:`More...<details-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_common.h>

	enum Layout
	{
	    :ref:`ANY<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a890528943ea12cf9832d7f437ea149b5>`     = 0,
	    :ref:`NCHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ad6021da38189a289671c55a105a5ffbf>`    = 1,
	    :ref:`NHWC<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8aa5bfc87d4f0e3d8d55738659e9f54a0f>`    = 2,
	    :ref:`NCDHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a99c99dce2cb7b30d7c69b2b058de0d87>`   = 3,
	    :ref:`NDHWC<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac6cf2a893e09ee2ea7343fd93d0a146c>`   = 4,
	    :ref:`OIHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac14bc14ceb9b39273e2b83b768f2fafa>`    = 64,
	    :ref:`GOIHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ab81e1bde83f50eac529f30a72f55463e>`   = 65,
	    :ref:`OIDHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a4a15f724d7cbe5b4bf1dc1387924e4af>`   = 66,
	    :ref:`GOIDHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8acd758bb9f8af977368583e069325eb45>`  = 67,
	    :ref:`SCALAR<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8af281cba35713ae233c47fb6b99fa69cc>`  = 95,
	    :ref:`C<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a7b88edf4f396b44d0748255cdb960628>`       = 96,
	    :ref:`CHW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a1bf5ff1864222bfb50fc81c85ec9fa4c>`     = 128,
	    :ref:`HWC<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a66d18f9391c19ec8d451596180448e2f>`     = 129,
	    :ref:`HW<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac6dc6ca3b7fe32d0d959ee64429aec83>`      = 192,
	    :ref:`NC<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ae290c8fb65bf200d54aa8755d8a38bc4>`      = 193,
	    :ref:`CN<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac95e7e70cb42310b36e35dd73703db39>`      = 194,
	    :ref:`BLOCKED<doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ad12952da1945a1aeb63686ae211b50ff>` = 200,
	};

.. _details-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Layouts that the inference engine supports.

Enum Values
-----------

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a890528943ea12cf9832d7f437ea149b5:
.. index:: pair: enumvalue; ANY

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ANY

"any" layout

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ad6021da38189a289671c55a105a5ffbf:
.. index:: pair: enumvalue; NCHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NCHW

NCHW layout for input / output blobs.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8aa5bfc87d4f0e3d8d55738659e9f54a0f:
.. index:: pair: enumvalue; NHWC

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NHWC

NHWC layout for input / output blobs.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a99c99dce2cb7b30d7c69b2b058de0d87:
.. index:: pair: enumvalue; NCDHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NCDHW

NCDHW layout for input / output blobs.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac6cf2a893e09ee2ea7343fd93d0a146c:
.. index:: pair: enumvalue; NDHWC

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NDHWC

NDHWC layout for input / output blobs.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac14bc14ceb9b39273e2b83b768f2fafa:
.. index:: pair: enumvalue; OIHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OIHW

NDHWC layout for operation weights.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ab81e1bde83f50eac529f30a72f55463e:
.. index:: pair: enumvalue; GOIHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GOIHW

NDHWC layout for operation weights.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a4a15f724d7cbe5b4bf1dc1387924e4af:
.. index:: pair: enumvalue; OIDHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OIDHW

NDHWC layout for operation weights.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8acd758bb9f8af977368583e069325eb45:
.. index:: pair: enumvalue; GOIDHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GOIDHW

NDHWC layout for operation weights.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8af281cba35713ae233c47fb6b99fa69cc:
.. index:: pair: enumvalue; SCALAR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SCALAR

A scalar layout.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a7b88edf4f396b44d0748255cdb960628:
.. index:: pair: enumvalue; C

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	C

A bias layout for operation.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a1bf5ff1864222bfb50fc81c85ec9fa4c:
.. index:: pair: enumvalue; CHW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CHW

A single image layout (e.g. for mean image)

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8a66d18f9391c19ec8d451596180448e2f:
.. index:: pair: enumvalue; HWC

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HWC

A single image layout (e.g. for mean image)

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac6dc6ca3b7fe32d0d959ee64429aec83:
.. index:: pair: enumvalue; HW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HW

HW 2D layout.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ae290c8fb65bf200d54aa8755d8a38bc4:
.. index:: pair: enumvalue; NC

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NC

NC 2D layout.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ac95e7e70cb42310b36e35dd73703db39:
.. index:: pair: enumvalue; CN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CN

CN 2D layout.

.. _doxid-namespace_inference_engine_1a246d143abc5ca07da8d2cadeeb88fdb8ad12952da1945a1aeb63686ae211b50ff:
.. index:: pair: enumvalue; BLOCKED

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BLOCKED

A blocked layout.

