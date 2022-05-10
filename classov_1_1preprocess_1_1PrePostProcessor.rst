.. index:: pair: class; ov::preprocess::PrePostProcessor
.. _doxid-classov_1_1preprocess_1_1_pre_post_processor:

class ov::preprocess::PrePostProcessor
======================================



Overview
~~~~~~~~

Main class for adding pre- and post- processing steps to existing :ref:`ov::Model <doxid-classov_1_1_model>`. :ref:`More...<details-classov_1_1preprocess_1_1_pre_post_processor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <pre_post_process.hpp>
	
	class PrePostProcessor
	{
	public:
		// construction
	
		:ref:`PrePostProcessor<doxid-classov_1_1preprocess_1_1_pre_post_processor_1adb3be58d378a5fa423a2b3db76c85868>`(const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& function);
		:ref:`PrePostProcessor<doxid-classov_1_1preprocess_1_1_pre_post_processor_1a90f84ba6e2589e7a65659497c6bcf14f>`(PrePostProcessor&&);

		// methods
	
		PrePostProcessor& :ref:`operator =<doxid-classov_1_1preprocess_1_1_pre_post_processor_1a902a9b056f7f3ba62952314f98ef1d28>` (PrePostProcessor&&);
		:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`& :ref:`input<doxid-classov_1_1preprocess_1_1_pre_post_processor_1aacaaece6f739eeabac7b5c31f141471c>`();
		:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`& :ref:`input<doxid-classov_1_1preprocess_1_1_pre_post_processor_1ab2f280beaa28aae9f340ac41a2edf884>`(const std::string& tensor_name);
		:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`& :ref:`input<doxid-classov_1_1preprocess_1_1_pre_post_processor_1aacda9b786b2187ca6ecb137bfb38e78a>`(size_t input_index);
		:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`& :ref:`output<doxid-classov_1_1preprocess_1_1_pre_post_processor_1a97c6918305914d79ab0f3e963284bd21>`();
		:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`& :ref:`output<doxid-classov_1_1preprocess_1_1_pre_post_processor_1a913971ff96886833dbac4f0f06859fee>`(const std::string& tensor_name);
		:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`& :ref:`output<doxid-classov_1_1preprocess_1_1_pre_post_processor_1ac6100cc37fad4109c6112e0cb243ff29>`(size_t output_index);
		std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`> :ref:`build<doxid-classov_1_1preprocess_1_1_pre_post_processor_1a62bde91535a3cd93cb2dcf5f416fe24a>`();
	};
.. _details-classov_1_1preprocess_1_1_pre_post_processor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Main class for adding pre- and post- processing steps to existing :ref:`ov::Model <doxid-classov_1_1_model>`.

This is a helper class for writing easy pre- and post- processing operations on :ref:`ov::Model <doxid-classov_1_1_model>` object assuming that any preprocess operation takes one input and produces one output.

For advanced preprocessing scenarios, like combining several functions with multiple inputs/outputs into one, client's code can use transformation passes over :ref:`ov::Model <doxid-classov_1_1_model>`

Construction
------------

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1adb3be58d378a5fa423a2b3db76c85868:
.. index:: pair: function; PrePostProcessor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PrePostProcessor(const std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`>& function)

Default constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- function

		- Existing function representing loaded model

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1a90f84ba6e2589e7a65659497c6bcf14f:
.. index:: pair: function; PrePostProcessor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PrePostProcessor(PrePostProcessor&&)

Default move constructor.

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1a902a9b056f7f3ba62952314f98ef1d28:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PrePostProcessor& operator = (PrePostProcessor&&)

Default move assignment operator.

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1aacaaece6f739eeabac7b5c31f141471c:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`& input()

Gets input pre-processing data structure. Should be used only if model/function has only one input Using returned structure application's code is able to set user's tensor data (e.g layout), preprocess steps, target model's data.



.. rubric:: Returns:

Reference to model's input information structure

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1ab2f280beaa28aae9f340ac41a2edf884:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`& input(const std::string& tensor_name)

Gets input pre-processing data structure for input identified by it's tensor name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- :ref:`Tensor <doxid-classov_1_1_tensor>` name of specific input. Throws if tensor name is not associated with any input in a model



.. rubric:: Returns:

Reference to model's input information structure

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1aacda9b786b2187ca6ecb137bfb38e78a:
.. index:: pair: function; input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`& input(size_t input_index)

Gets input pre-processing data structure for input identified by it's order in a model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_index

		- :ref:`Input <doxid-classov_1_1_input>` index of specific input. Throws if input index is out of range for associated function



.. rubric:: Returns:

Reference to model's input information structure

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1a97c6918305914d79ab0f3e963284bd21:
.. index:: pair: function; output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`& output()

Gets output post-processing data structure. Should be used only if model/function has only one output Using returned structure application's code is able to set model's output data, post-process steps, user's tensor data (e.g layout)



.. rubric:: Returns:

Reference to model's output information structure

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1a913971ff96886833dbac4f0f06859fee:
.. index:: pair: function; output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`& output(const std::string& tensor_name)

Gets output post-processing data structure for output identified by it's tensor name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor_name

		- :ref:`Tensor <doxid-classov_1_1_tensor>` name of specific output. Throws if tensor name is not associated with any input in a model



.. rubric:: Returns:

Reference to model's output information structure

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1ac6100cc37fad4109c6112e0cb243ff29:
.. index:: pair: function; output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`& output(size_t output_index)

Gets output post-processing data structure for output identified by it's order in a model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_index

		- :ref:`Output <doxid-classov_1_1_output>` index of specific output. Throws if output index is out of range for associated function



.. rubric:: Returns:

Reference to model's output information structure

.. _doxid-classov_1_1preprocess_1_1_pre_post_processor_1a62bde91535a3cd93cb2dcf5f416fe24a:
.. index:: pair: function; build

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Model<doxid-classov_1_1_model>`> build()

Adds pre/post-processing operations to function passed in constructor.



.. rubric:: Returns:

Function with added pre/post-processing operations


