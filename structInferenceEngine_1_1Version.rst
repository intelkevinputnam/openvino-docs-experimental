.. index:: pair: struct; InferenceEngine::Version
.. _doxid-struct_inference_engine_1_1_version:

struct InferenceEngine::Version
===============================

.. toctree::
	:hidden:

	ApiVersion <structInferenceEngine_1_1Version_1_1ApiVersion.rst>

Overview
~~~~~~~~

Represents version information that describes plugins and the inference engine runtime library. :ref:`More...<details-struct_inference_engine_1_1_version>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_version.hpp>
	
	struct Version
	{
		// structs
	
		struct :ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version>`;

		// fields
	
		:ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version>` :ref:`apiVersion<doxid-struct_inference_engine_1_1_version_1a67f6a06d9210b1b080e2547ef03f3859>`;
		const char \* :ref:`buildNumber<doxid-struct_inference_engine_1_1_version_1aa5f87bb79d0028b64bba724f67c02ec4>`;
		const char \* :ref:`description<doxid-struct_inference_engine_1_1_version_1acce46690f8fdd1b8ecf29c6915f8528b>`;
	};

	// direct descendants

	class :ref:`VersionStore<doxid-class_inference_engine_1_1_i_inference_plugin_1_1_version_store>`;
.. _details-struct_inference_engine_1_1_version:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents version information that describes plugins and the inference engine runtime library.

Fields
------

.. _doxid-struct_inference_engine_1_1_version_1a67f6a06d9210b1b080e2547ef03f3859:
.. index:: pair: variable; apiVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version>` apiVersion

An API version reflects the set of supported features.

.. _doxid-struct_inference_engine_1_1_version_1aa5f87bb79d0028b64bba724f67c02ec4:
.. index:: pair: variable; buildNumber

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const char \* buildNumber

A null terminated string with build number.

.. _doxid-struct_inference_engine_1_1_version_1acce46690f8fdd1b8ecf29c6915f8528b:
.. index:: pair: variable; description

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const char \* description

A null terminated description string.


