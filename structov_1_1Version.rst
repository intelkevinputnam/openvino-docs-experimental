.. index:: pair: struct; ov::Version
.. _doxid-structov_1_1_version:

struct ov::Version
==================



Overview
~~~~~~~~

Represents version information that describes plugins and the OpemVINO library. :ref:`More...<details-structov_1_1_version>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <version.hpp>
	
	struct Version
	{
		// fields
	
		const char \* :ref:`buildNumber<doxid-structov_1_1_version_1af4b8fa13dd9a0847837120cd5b08a8bc>`;
		const char \* :ref:`description<doxid-structov_1_1_version_1a5d91c6ffa11a91ca5b39d7e9bd539bd4>`;
	};
.. _details-structov_1_1_version:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents version information that describes plugins and the OpemVINO library.

Fields
------

.. _doxid-structov_1_1_version_1af4b8fa13dd9a0847837120cd5b08a8bc:
.. index:: pair: variable; buildNumber

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const char \* buildNumber

A null terminated string with build number.

.. _doxid-structov_1_1_version_1a5d91c6ffa11a91ca5b39d7e9bd539bd4:
.. index:: pair: variable; description

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const char \* description

A null terminated description string.


