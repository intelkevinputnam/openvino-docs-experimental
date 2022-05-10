.. index:: pair: class; InferenceEngine::IPreProcessData
.. _doxid-class_inference_engine_1_1_i_pre_process_data:

class InferenceEngine::IPreProcessData
======================================



Overview
~~~~~~~~

This class stores pre-process information for exact input. :ref:`More...<details-class_inference_engine_1_1_i_pre_process_data>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess_data.hpp>
	
	class IPreProcessData: public std::enable_shared_from_this< IPreProcessData >
	{
	public:
		// methods
	
		virtual void :ref:`setRoiBlob<doxid-class_inference_engine_1_1_i_pre_process_data_1aeaaaf00323f07e987efa981791e5285b>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& blob) = 0;
		virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :ref:`getRoiBlob<doxid-class_inference_engine_1_1_i_pre_process_data_1a116d414da46921609f53e96fb97cfe11>`() const = 0;
	
		virtual void :ref:`execute<doxid-class_inference_engine_1_1_i_pre_process_data_1a66e05d0ec1319e835e9735dbfba1e91c>`(
			:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& preprocessedBlob,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info,
			bool serial,
			int batchSize = -1
			) = 0;
	
		virtual void :target:`isApplicable<doxid-class_inference_engine_1_1_i_pre_process_data_1a51b123a4725d38a01f46e2aee5b694aa>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& src, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& dst) = 0;

	protected:
	};

	// direct descendants

	class :ref:`PreProcessData<doxid-class_inference_engine_1_1_pre_process_data>`;
.. _details-class_inference_engine_1_1_i_pre_process_data:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class stores pre-process information for exact input.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_pre_process_data_1aeaaaf00323f07e987efa981791e5285b:
.. index:: pair: function; setRoiBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setRoiBlob(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& blob) = 0

Sets :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` blob to be resized and placed to the default input blob during pre-processing.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- blob

		- :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` blob.

.. _doxid-class_inference_engine_1_1_i_pre_process_data_1a116d414da46921609f53e96fb97cfe11:
.. index:: pair: function; getRoiBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` getRoiBlob() const = 0

Gets pointer to the :ref:`ROI <doxid-struct_inference_engine_1_1_r_o_i>` blob used for a given input.



.. rubric:: Returns:

:ref:`Blob <doxid-class_inference_engine_1_1_blob>` pointer.

.. _doxid-class_inference_engine_1_1_i_pre_process_data_1a66e05d0ec1319e835e9735dbfba1e91c:
.. index:: pair: function; execute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& preprocessedBlob,
		const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info,
		bool serial,
		int batchSize = -1
		) = 0

Executes input pre-processing with a given pre-processing information.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outBlob

		- pre-processed output blob to be used for inference.

	*
		- info

		- pre-processing info that specifies resize algorithm and color format.

	*
		- serial

		- disable OpenMP threading if the value set to true.

	*
		- batchSize

		- batch size for pre-processing.


