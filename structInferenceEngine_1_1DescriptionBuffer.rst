.. index:: pair: struct; InferenceEngine::DescriptionBuffer
.. _doxid-struct_inference_engine_1_1_description_buffer:

struct InferenceEngine::DescriptionBuffer
=========================================



Overview
~~~~~~~~

A description buffer wrapping StatusCode and :ref:`ResponseDesc <doxid-struct_inference_engine_1_1_response_desc>`. :ref:`More...<details-struct_inference_engine_1_1_description_buffer>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <description_buffer.hpp>
	
	struct DescriptionBuffer: public std::basic_streambuf< char, std::char_traits< char > >
	{
		// construction
	
		:ref:`DescriptionBuffer<doxid-struct_inference_engine_1_1_description_buffer_1a4491a8b0c51b1d6a2f3c5659bfea6e44>`(:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` err, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* desc);
		:ref:`DescriptionBuffer<doxid-struct_inference_engine_1_1_description_buffer_1abd1e11b649f0609193347e45fd0d0c53>`(:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` err);
		:ref:`DescriptionBuffer<doxid-struct_inference_engine_1_1_description_buffer_1a77ae9665ba40b87f7f40436bb05a75b9>`(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* desc);
		:ref:`DescriptionBuffer<doxid-struct_inference_engine_1_1_description_buffer_1ac77c72abb813c07660e8eb6ae10f9ac2>`(char \* pBuffer, size_t len);
		:ref:`DescriptionBuffer<doxid-struct_inference_engine_1_1_description_buffer_1aff0d753c4b2f03ff840259ce7d39eedd>`(:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` err, char \* pBuffer, size_t len);

		// methods
	
		template <class T>
		DescriptionBuffer& :ref:`operator <<<doxid-struct_inference_engine_1_1_description_buffer_1af29c6c33b011e3937907ce4df846f471>` (const T& obj);
	
		:ref:`operator StatusCode<doxid-struct_inference_engine_1_1_description_buffer_1a85a46a6c87d12ea4eb1260f7081147b6>` () const;
	};
.. _details-struct_inference_engine_1_1_description_buffer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A description buffer wrapping StatusCode and :ref:`ResponseDesc <doxid-struct_inference_engine_1_1_response_desc>`.

Construction
------------

.. _doxid-struct_inference_engine_1_1_description_buffer_1a4491a8b0c51b1d6a2f3c5659bfea6e44:
.. index:: pair: function; DescriptionBuffer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DescriptionBuffer(:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` err, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* desc)

Creeates a description buffer with parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- err

		- The error code

	*
		- desc

		- The response desc to write an error message to

.. _doxid-struct_inference_engine_1_1_description_buffer_1abd1e11b649f0609193347e45fd0d0c53:
.. index:: pair: function; DescriptionBuffer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DescriptionBuffer(:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` err)

Constructs with StatusCode.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- err

		- The StatusCode value

.. _doxid-struct_inference_engine_1_1_description_buffer_1a77ae9665ba40b87f7f40436bb05a75b9:
.. index:: pair: function; DescriptionBuffer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DescriptionBuffer(:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* desc)

Constructs with :ref:`ResponseDesc <doxid-struct_inference_engine_1_1_response_desc>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- desc

		- The :ref:`ResponseDesc <doxid-struct_inference_engine_1_1_response_desc>` pointer

.. _doxid-struct_inference_engine_1_1_description_buffer_1ac77c72abb813c07660e8eb6ae10f9ac2:
.. index:: pair: function; DescriptionBuffer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DescriptionBuffer(char \* pBuffer, size_t len)

Constructs with parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pBuffer

		- The buffer to wrtie to.

	*
		- len

		- The length of ``pBuffer``

.. _doxid-struct_inference_engine_1_1_description_buffer_1aff0d753c4b2f03ff840259ce7d39eedd:
.. index:: pair: function; DescriptionBuffer

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DescriptionBuffer(:ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` err, char \* pBuffer, size_t len)

Constructs with parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- err

		- The StatusCode value

	*
		- pBuffer

		- The buffer to wrtie to.

	*
		- len

		- The length of ``pBuffer``

Methods
-------

.. _doxid-struct_inference_engine_1_1_description_buffer_1af29c6c33b011e3937907ce4df846f471:
.. index:: pair: function; operator<<

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	DescriptionBuffer& operator << (const T& obj)

Writes to :ref:`ResponseDesc <doxid-struct_inference_engine_1_1_response_desc>` stream.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- obj

		- The object to write to stream

	*
		- T

		- An object type



.. rubric:: Returns:

A reference to itself

.. _doxid-struct_inference_engine_1_1_description_buffer_1a85a46a6c87d12ea4eb1260f7081147b6:
.. index:: pair: function; operator StatusCode

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator StatusCode () const

Converts to StatusCode.



.. rubric:: Returns:

A StatusCode value


