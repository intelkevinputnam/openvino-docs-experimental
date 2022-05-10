.. index:: pair: class; ov::preprocess::InputModelInfo
.. _doxid-classov_1_1preprocess_1_1_input_model_info:

class ov::preprocess::InputModelInfo
====================================



Overview
~~~~~~~~

Information about model's input tensor. If all information is already included to loaded model, this info may not be needed. However it can be set to specify additional information about model, like 'layout'. :ref:`More...<details-classov_1_1preprocess_1_1_input_model_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <input_model_info.hpp>
	
	class InputModelInfo
	{
	public:
		// methods
	
		InputModelInfo& :ref:`set_layout<doxid-classov_1_1preprocess_1_1_input_model_info_1aeac53aa90be5b8a6b86def31fab396b4>`(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout);
	};
.. _details-classov_1_1preprocess_1_1_input_model_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Information about model's input tensor. If all information is already included to loaded model, this info may not be needed. However it can be set to specify additional information about model, like 'layout'.

Example of usage of model 'layout': Support model has input parameter with shape {1, 3, 224, 224} and user needs to resize input image to model's dimensions. It can be done like this

.. ref-code-block:: cpp

	<:ref:`model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` has input parameter with shape {1, 3, 224, 224}>
	auto proc = PrePostProcessor(function);
	proc.input().preprocess().resize(ResizeAlgorithm::RESIZE_LINEAR);
	proc.input().model().set_layout("NCHW");

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_input_model_info_1aeac53aa90be5b8a6b86def31fab396b4:
.. index:: pair: function; set_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputModelInfo& set_layout(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout)

Set layout for model's input tensor This version allows chaining for Lvalue objects.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layout

		- :ref:`Layout <doxid-classov_1_1_layout>` for model's input tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner


