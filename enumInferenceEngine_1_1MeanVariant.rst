.. index:: pair: enum; MeanVariant
.. _doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161:

enum InferenceEngine::MeanVariant
=================================

Overview
~~~~~~~~

Defines available types of mean. :ref:`More...<details-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess.hpp>

	enum MeanVariant
	{
	    :ref:`MEAN_IMAGE<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161af315f9b5a0eb9506207af6e447f54826>`,
	    :ref:`MEAN_VALUE<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161a782a36934a315c43f504c04924ca5f26>`,
	    :ref:`NONE<doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161a4b32cd7cd2feb3378015fcf7bde23692>`,
	};

.. _details-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Defines available types of mean.

Enum Values
-----------

.. _doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161af315f9b5a0eb9506207af6e447f54826:
.. index:: pair: enumvalue; MEAN_IMAGE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MEAN_IMAGE

mean value is specified for each input pixel

.. _doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161a782a36934a315c43f504c04924ca5f26:
.. index:: pair: enumvalue; MEAN_VALUE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MEAN_VALUE

mean value is specified for each input channel

.. _doxid-namespace_inference_engine_1a02a50369bd2f3354578072f5e4e98161a4b32cd7cd2feb3378015fcf7bde23692:
.. index:: pair: enumvalue; NONE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NONE

no mean value specified

