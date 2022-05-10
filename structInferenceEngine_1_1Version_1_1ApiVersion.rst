.. index:: pair: struct; InferenceEngine::Version::ApiVersion
.. _doxid-struct_inference_engine_1_1_version_1_1_api_version:

struct InferenceEngine::Version::ApiVersion
===========================================



Overview
~~~~~~~~

An API version reflects the set of supported features. :ref:`More...<details-struct_inference_engine_1_1_version_1_1_api_version>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_version.hpp>
	
	struct ApiVersion
	{
		// fields
	
		int :ref:`major<doxid-struct_inference_engine_1_1_version_1_1_api_version_1ab6621bb6d99426cbe1528d14c6109483>`;
		int :ref:`minor<doxid-struct_inference_engine_1_1_version_1_1_api_version_1af92c64f1c99e3676ad822e5d5242d684>`;

		// construction
	
		:ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version_1af19c0b1ebe68400c8f75991a1166a5a9>`();
		:ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version_1a633b31286b08415c6b70f8f44ba14d04>`(const ApiVersion& v);
		:ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version_1a36213138b6787a6e06c0a016eb23cb13>`(int _major, int _minor);

		// methods
	
		ApiVersion& :ref:`operator =<doxid-struct_inference_engine_1_1_version_1_1_api_version_1ac0bf2e197290d274595c60e38454d32a>` (const ApiVersion& other);
	};
.. _details-struct_inference_engine_1_1_version_1_1_api_version:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An API version reflects the set of supported features.

Deprecated Use IE_VERSION_[MAJOR|MINOR|PATCH] definitions, buildNumber property

Fields
------

.. _doxid-struct_inference_engine_1_1_version_1_1_api_version_1ab6621bb6d99426cbe1528d14c6109483:
.. index:: pair: variable; major

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int major

A major version.

.. _doxid-struct_inference_engine_1_1_version_1_1_api_version_1af92c64f1c99e3676ad822e5d5242d684:
.. index:: pair: variable; minor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int minor

A minor version.

Construction
------------

.. _doxid-struct_inference_engine_1_1_version_1_1_api_version_1af19c0b1ebe68400c8f75991a1166a5a9:
.. index:: pair: function; ApiVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ApiVersion()

A default construtor.

.. _doxid-struct_inference_engine_1_1_version_1_1_api_version_1a633b31286b08415c6b70f8f44ba14d04:
.. index:: pair: function; ApiVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ApiVersion(const ApiVersion& v)

A default construtor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- v

		- A version to copy

.. _doxid-struct_inference_engine_1_1_version_1_1_api_version_1a36213138b6787a6e06c0a016eb23cb13:
.. index:: pair: function; ApiVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ApiVersion(int _major, int _minor)

A default construtor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _major

		- A major version to copy

	*
		- _minor

		- A minor version to copy

Methods
-------

.. _doxid-struct_inference_engine_1_1_version_1_1_api_version_1ac0bf2e197290d274595c60e38454d32a:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ApiVersion& operator = (const ApiVersion& other)

A copy operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- An object to copy



.. rubric:: Returns:

A copy


