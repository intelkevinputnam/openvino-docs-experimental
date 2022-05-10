.. index:: pair: enum; ThreadBindingType
.. _doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872:

enum InferenceEngine::IStreamsExecutor::ThreadBindingType
=========================================================

Overview
~~~~~~~~

Defines inference thread binding type. :ref:`More...<details-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_istreams_executor.hpp>

	enum ThreadBindingType
	{
	    :ref:`NONE<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872aadf5cef616d97b604fe6e58bc2a3545c>`,
	    :ref:`CORES<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872ac31f62d8f7987f4816c5fbfffb26429f>`,
	    :ref:`NUMA<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872a1deb6641aa625f0a536f880ebb21ebec>`,
	    :ref:`HYBRID_AWARE<doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872a1a7a5d64f7a66531b134c7caf524ad81>`,
	};

.. _details-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Defines inference thread binding type.

Enum Values
-----------

.. _doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872aadf5cef616d97b604fe6e58bc2a3545c:
.. index:: pair: enumvalue; NONE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NONE

Don't bind the inference threads.

.. _doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872ac31f62d8f7987f4816c5fbfffb26429f:
.. index:: pair: enumvalue; CORES

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CORES

Bind inference threads to the CPU cores (round-robin)

.. _doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872a1deb6641aa625f0a536f880ebb21ebec:
.. index:: pair: enumvalue; NUMA

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NUMA

Bind to the NUMA nodes (default mode for the non-hybrid CPUs on the Win/MacOS, where the 'CORES' is not implemeneted)

.. _doxid-class_inference_engine_1_1_i_streams_executor_1ac87e784e6e176865ef4518b8e957a872a1a7a5d64f7a66531b134c7caf524ad81:
.. index:: pair: enumvalue; HYBRID_AWARE

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HYBRID_AWARE

Let the runtime bind the inference threads depending on the cores type (default mode for the hybrid CPUs)

