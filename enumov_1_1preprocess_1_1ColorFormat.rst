.. index:: pair: enum; ColorFormat
.. _doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707:

enum ov::preprocess::ColorFormat
================================

Overview
~~~~~~~~

Color format enumeration for conversion. :ref:`More...<details-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <color_format.hpp>

	enum ColorFormat
	{
	    :target:`UNDEFINED<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a0db45d2a4141101bdfe48e3314cfbca3>`,
	    :target:`NV12_SINGLE_PLANE<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707ac5e414dafffbbd14d331431a0c9bc7cb>`,
	    :ref:`NV12_TWO_PLANES<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a54f60c652650de96e9d118187b3ba25f>`,
	    :target:`I420_SINGLE_PLANE<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a309e9d55d58fcfb5699644cd63ee7fa6>`,
	    :ref:`I420_THREE_PLANES<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a96f935fdd26bb75a314084ef82623143>`,
	    :target:`RGB<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a889574aebacda6bfd3e534e2b49b8028>`,
	    :target:`BGR<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a2ad5640ebdec72fc79531d1778c6c2dc>`,
	    :ref:`RGBX<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a1c88184be3a67bdace60f24e371e0c96>`,
	    :ref:`BGRX<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707aebe38a01ae4fb28439bcfc44ca9accda>`,
	};

.. _details-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Color format enumeration for conversion.

Extra information about input color format for preprocessing.

Enum Values
-----------

.. _doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a54f60c652650de96e9d118187b3ba25f:
.. index:: pair: enumvalue; NV12_TWO_PLANES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NV12_TWO_PLANES

Image in NV12 format represented as separate tensors for Y and UV planes.

.. _doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a96f935fdd26bb75a314084ef82623143:
.. index:: pair: enumvalue; I420_THREE_PLANES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	I420_THREE_PLANES

Image in I420 format represented as separate tensors for Y, U and V planes.

.. _doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707a1c88184be3a67bdace60f24e371e0c96:
.. index:: pair: enumvalue; RGBX

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RGBX

Image in RGBX interleaved format (4 channels)

.. _doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707aebe38a01ae4fb28439bcfc44ca9accda:
.. index:: pair: enumvalue; BGRX

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BGRX

Image in BGRX interleaved format (4 channels)

