.. index:: pair: class; ov::preprocess::OutputModelInfo
.. _doxid-classov_1_1preprocess_1_1_output_model_info:

class ov::preprocess::OutputModelInfo
=====================================



Overview
~~~~~~~~

Information about model's output tensor. If all information is already included to loaded model, this info may not be needed. However it can be set to specify additional information about model's output, like 'layout'. :ref:`More...<details-classov_1_1preprocess_1_1_output_model_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <output_model_info.hpp>
	
	class OutputModelInfo
	{
	public:
		// methods
	
		OutputModelInfo& :ref:`set_layout<doxid-classov_1_1preprocess_1_1_output_model_info_1a0c3e2f9b6fdbd1153d89b109e8993261>`(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout);
	};
.. _details-classov_1_1preprocess_1_1_output_model_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Information about model's output tensor. If all information is already included to loaded model, this info may not be needed. However it can be set to specify additional information about model's output, like 'layout'.

Example of usage of model's 'layout': Suppose model has output result with shape {1, 3, 224, 224} and ``NHWC`` layout. User may need to transpose output picture to interleaved format {1, 224, 224, 3}. This can be done with the following code

.. ref-code-block:: cpp

	<:ref:`model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` has output :ref:`result <doxid-namespacengraph_1_1runtime_1_1reference_1a9f63c4359f72e8f64b3d6ff4883447f0>` with shape {1, 3, 224, 224}>
	auto proc = PrePostProcessor(function);
	proc.output().model().set_layout("NCHW");
	proc.output().postprocess().convert_layout("NHWC");
	function = proc.build();

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_output_model_info_1a0c3e2f9b6fdbd1153d89b109e8993261:
.. index:: pair: function; set_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OutputModelInfo& set_layout(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout)

Set layout for model's output tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layout

		- :ref:`Layout <doxid-classov_1_1_layout>` for model's output tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner


