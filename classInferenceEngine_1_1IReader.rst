.. index:: pair: class; InferenceEngine::IReader
.. _doxid-class_inference_engine_1_1_i_reader:

class InferenceEngine::IReader
==============================



Overview
~~~~~~~~

:ref:`IReader <doxid-class_inference_engine_1_1_i_reader>` an abstract interface for Inference Engine readers. :ref:`More...<details-class_inference_engine_1_1_i_reader>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_reader.hpp>
	
	class IReader: public std::enable_shared_from_this< IReader >
	{
	public:
		// methods
	
		virtual bool :ref:`supportModel<doxid-class_inference_engine_1_1_i_reader_1adf22406f29aac3b30a6275c6ce8f97ed>`(std::istream& model) const = 0;
	
		virtual :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`read<doxid-class_inference_engine_1_1_i_reader_1a630890143a7e47d3e33e3b348fd67344>`(
			std::istream& model,
			const std::vector<:ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>`>& exts
			) const = 0;
	
		virtual :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` :ref:`read<doxid-class_inference_engine_1_1_i_reader_1a174d4ac569e56c291aeda7be8e470f88>`(
			std::istream& model,
			const :ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`& weights,
			const std::vector<:ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>`>& exts
			) const = 0;
	
		virtual std::vector<std::string> :ref:`getDataFileExtensions<doxid-class_inference_engine_1_1_i_reader_1a292380a28105f7c457c529bb19292a89>`() const = 0;

	protected:
	};
.. _details-class_inference_engine_1_1_i_reader:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`IReader <doxid-class_inference_engine_1_1_i_reader>` an abstract interface for Inference Engine readers.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_reader_1adf22406f29aac3b30a6275c6ce8f97ed:
.. index:: pair: function; supportModel

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool supportModel(std::istream& model) const = 0

Checks that reader supports format of the model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- stream with model



.. rubric:: Returns:

true if format is supported

.. _doxid-class_inference_engine_1_1_i_reader_1a630890143a7e47d3e33e3b348fd67344:
.. index:: pair: function; read

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` read(
		std::istream& model,
		const std::vector<:ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>`>& exts
		) const = 0

Reads the model to :ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- stream with model

	*
		- exts

		- vector with extensions



.. rubric:: Returns:

:ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>`

.. _doxid-class_inference_engine_1_1_i_reader_1a174d4ac569e56c291aeda7be8e470f88:
.. index:: pair: function; read

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>` read(
		std::istream& model,
		const :ref:`Blob::CPtr<doxid-class_inference_engine_1_1_blob_1a22946ecdb18fd8a9e8394087930d2092>`& weights,
		const std::vector<:ref:`IExtensionPtr<doxid-namespace_inference_engine_1a7a4456ae150afbff5140be2d92680fa4>`>& exts
		) const = 0

Reads the model to :ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- stream with model

	*
		- weights

		- stream with binary data

	*
		- exts

		- vector with extensions



.. rubric:: Returns:

:ref:`CNNNetwork <doxid-class_inference_engine_1_1_c_n_n_network>`

.. _doxid-class_inference_engine_1_1_i_reader_1a292380a28105f7c457c529bb19292a89:
.. index:: pair: function; getDataFileExtensions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::string> getDataFileExtensions() const = 0

Returns all supported extensions for data files.



.. rubric:: Returns:

vector of file extensions, for example the reader for OpenVINO IR returns {"bin"}


