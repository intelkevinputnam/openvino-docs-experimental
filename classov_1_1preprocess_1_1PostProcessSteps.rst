.. index:: pair: class; ov::preprocess::PostProcessSteps
.. _doxid-classov_1_1preprocess_1_1_post_process_steps:

class ov::preprocess::PostProcessSteps
======================================



Overview
~~~~~~~~

Postprocessing steps. Each step typically intends adding of some operation to output parameter User application can specify sequence of postprocessing steps in a builder-like manner. :ref:`More...<details-classov_1_1preprocess_1_1_post_process_steps>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <postprocess_steps.hpp>
	
	class PostProcessSteps
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>&node)> :ref:`CustomPostprocessOp<doxid-classov_1_1preprocess_1_1_post_process_steps_1a862ab1665043b63c361ee99dc3721973>`;

		// methods
	
		PostProcessSteps& :ref:`convert_element_type<doxid-classov_1_1preprocess_1_1_post_process_steps_1a9acf86e4956ec2c8263732d51bc0015f>`(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type = {});
		PostProcessSteps& :ref:`convert_layout<doxid-classov_1_1preprocess_1_1_post_process_steps_1ad03132637307eeb01d734bd5175f2e4e>`(const :ref:`Layout<doxid-classov_1_1_layout>`& dst_layout = {});
		PostProcessSteps& :ref:`convert_layout<doxid-classov_1_1preprocess_1_1_post_process_steps_1aaf7d00f913cda7fb08d7e2448b487b0d>`(const std::vector<uint64_t>& dims);
		PostProcessSteps& :ref:`custom<doxid-classov_1_1preprocess_1_1_post_process_steps_1addc7cfdb5b10c97dc1a6fa40d9d149c5>`(const :ref:`CustomPostprocessOp<doxid-classov_1_1preprocess_1_1_post_process_steps_1a862ab1665043b63c361ee99dc3721973>`& postprocess_cb);
	};
.. _details-classov_1_1preprocess_1_1_post_process_steps:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Postprocessing steps. Each step typically intends adding of some operation to output parameter User application can specify sequence of postprocessing steps in a builder-like manner.

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	proc.output().postprocess().convert_element_type(:ref:`element::u8 <doxid-group__ov__element__cpp__api_1gaaf60c536d3e295285f6a899eb3d29e2f>`);
	function = proc.build();

Typedefs
--------

.. _doxid-classov_1_1preprocess_1_1_post_process_steps_1a862ab1665043b63c361ee99dc3721973:
.. index:: pair: typedef; CustomPostprocessOp

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>(const :ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>&node)> CustomPostprocessOp

Signature for custom postprocessing operation. Custom postprocessing operation takes one output node and produces one output node. For more advanced cases, client's code can use transformation passes over :ref:`ov::Model <doxid-classov_1_1_model>` directly.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- :ref:`Output <doxid-classov_1_1_output>` node for custom post-processing operation



.. rubric:: Returns:

New node after applying custom post-processing operation

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_post_process_steps_1a9acf86e4956ec2c8263732d51bc0015f:
.. index:: pair: function; convert_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PostProcessSteps& convert_element_type(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type = {})

Add convert element type post-process operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Desired type of output. If not specified, type will be obtained from 'tensor' output information



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_post_process_steps_1ad03132637307eeb01d734bd5175f2e4e:
.. index:: pair: function; convert_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PostProcessSteps& convert_layout(const :ref:`Layout<doxid-classov_1_1_layout>`& dst_layout = {})

Add 'convert layout' operation to specified layout.

Adds appropriate 'transpose' operation between model layout and user's desired layout. Current implementation requires source and destination layout to have same number of dimensions

Example: when model data has output in 'NCHW' layout ([1, 3, 224, 224]) but user needs interleaved output image ('NHWC', [1, 224, 224, 3]). Post-processing may look like this:

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	proc.output().model(OutputTensorInfo().:ref:`set_layout <doxid-group__ov__layout__cpp__api_1ga18464fb8ed029acb5fdc2bb1737358d9>`("NCHW"); // model output is NCHW
	proc.output().postprocess().:ref:`convert_layout <doxid-classov_1_1preprocess_1_1_post_process_steps_1ad03132637307eeb01d734bd5175f2e4e>`("NHWC"); // User needs output as NHWC



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst_layout

		- New layout after conversion. If not specified - destination layout is obtained from appropriate tensor output properties.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_post_process_steps_1aaf7d00f913cda7fb08d7e2448b487b0d:
.. index:: pair: function; convert_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PostProcessSteps& convert_layout(const std::vector<uint64_t>& dims)

Add convert layout operation by direct specification of transposed dimensions.

Example: model produces output with shape [1, 3, 480, 640] and user's needs interleaved output image [1, 480, 640, 3]. Post-processing may look like this:

.. ref-code-block:: cpp

	 auto proc = PrePostProcessor(function);
	proc.output().postprocess().convert_layout({0, 2, 3, 1});
	function = proc.build();



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- Dimensions array specifying places for new axis. If not empty, array size (N) must match to input shape rank. Array values shall contain all values from 0 to N-1. If empty, no actual conversion will be added.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_post_process_steps_1addc7cfdb5b10c97dc1a6fa40d9d149c5:
.. index:: pair: function; custom

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PostProcessSteps& custom(const :ref:`CustomPostprocessOp<doxid-classov_1_1preprocess_1_1_post_process_steps_1a862ab1665043b63c361ee99dc3721973>`& postprocess_cb)

Add custom post-process operation. Client application can specify callback function for custom action.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- postprocess_cb

		- Client's custom postprocess operation.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner


