.. index:: pair: class; ov::preprocess::OutputInfo
.. _doxid-classov_1_1preprocess_1_1_output_info:

class ov::preprocess::OutputInfo
================================



Overview
~~~~~~~~

Class holding postprocessing information for one output From postprocessing pipeline perspective, each output can be represented as: :ref:`More...<details-classov_1_1preprocess_1_1_output_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <output_info.hpp>
	
	class OutputInfo
	{
	public:
		// construction
	
		:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info_1a18881a95f92dddc83aa4db2895480ff1>`(OutputInfo&& other);

		// methods
	
		OutputInfo& :ref:`operator =<doxid-classov_1_1preprocess_1_1_output_info_1aaddad9ed3130ab564a6a1af27a373f3e>` (OutputInfo&& other);
		:ref:`OutputModelInfo<doxid-classov_1_1preprocess_1_1_output_model_info>`& :ref:`model<doxid-classov_1_1preprocess_1_1_output_info_1ac128c3e1696eecbffb3d63e0c2a60dd7>`();
		:ref:`PostProcessSteps<doxid-classov_1_1preprocess_1_1_post_process_steps>`& :ref:`postprocess<doxid-classov_1_1preprocess_1_1_output_info_1a53798941d4692c34f4a6d8bb1ec9fb99>`();
		:ref:`OutputTensorInfo<doxid-classov_1_1preprocess_1_1_output_tensor_info>`& :ref:`tensor<doxid-classov_1_1preprocess_1_1_output_info_1acb30494b416ef5296bbed9c64482abe4>`();
	};
.. _details-classov_1_1preprocess_1_1_output_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class holding postprocessing information for one output From postprocessing pipeline perspective, each output can be represented as:

* :ref:`Model <doxid-classov_1_1_model>` 's output info, (:ref:`OutputInfo::model <doxid-classov_1_1preprocess_1_1_output_info_1ac128c3e1696eecbffb3d63e0c2a60dd7>`)

* Postprocessing steps applied to user's input (:ref:`OutputInfo::postprocess <doxid-classov_1_1preprocess_1_1_output_info_1a53798941d4692c34f4a6d8bb1ec9fb99>`)

* User's desired output parameter information, which is a final one after preprocessing (:ref:`OutputInfo::tensor <doxid-classov_1_1preprocess_1_1_output_info_1acb30494b416ef5296bbed9c64482abe4>`)

Construction
------------

.. _doxid-classov_1_1preprocess_1_1_output_info_1a18881a95f92dddc83aa4db2895480ff1:
.. index:: pair: function; OutputInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OutputInfo(OutputInfo&& other)

Move constructor.

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_output_info_1aaddad9ed3130ab564a6a1af27a373f3e:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OutputInfo& operator = (OutputInfo&& other)

Move assignment operator.

.. _doxid-classov_1_1preprocess_1_1_output_info_1ac128c3e1696eecbffb3d63e0c2a60dd7:
.. index:: pair: function; model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputModelInfo<doxid-classov_1_1preprocess_1_1_output_model_info>`& model()

Get current output model information with ability to change original model's output data.



.. rubric:: Returns:

Reference to current model's output information structure

.. _doxid-classov_1_1preprocess_1_1_output_info_1a53798941d4692c34f4a6d8bb1ec9fb99:
.. index:: pair: function; postprocess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PostProcessSteps<doxid-classov_1_1preprocess_1_1_post_process_steps>`& postprocess()

Get current output post-process information with ability to add more post-processing steps.



.. rubric:: Returns:

Reference to current preprocess steps structure

.. _doxid-classov_1_1preprocess_1_1_output_info_1acb30494b416ef5296bbed9c64482abe4:
.. index:: pair: function; tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputTensorInfo<doxid-classov_1_1preprocess_1_1_output_tensor_info>`& tensor()

Get current output tensor information with ability to change specific data.



.. rubric:: Returns:

Reference to current output tensor structure


