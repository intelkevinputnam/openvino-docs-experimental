.. index:: pair: class; ov::preprocess::PreProcessSteps
.. _doxid-classov_1_1preprocess_1_1_pre_process_steps:

class ov::preprocess::PreProcessSteps
=====================================



Overview
~~~~~~~~

Preprocessing steps. Each step typically intends adding of some operation to input parameter User application can specify sequence of preprocessing steps in a builder-like manner. :ref:`More...<details-classov_1_1preprocess_1_1_pre_process_steps>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <preprocess_steps.hpp>
	
	class PreProcessSteps
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>&node)> :ref:`CustomPreprocessOp<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab19b0d87acc85c3f206abdd5400630f9>`;

		// methods
	
		PreProcessSteps& :ref:`convert_element_type<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab9e7979668e7403a72b07786f76ec0e0>`(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type = {});
		PreProcessSteps& :ref:`convert_color<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a1cc7cc3fc7afb5992c1920c483ce3332>`(const :ref:`ov::preprocess::ColorFormat<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707>`& dst_format);
		PreProcessSteps& :ref:`scale<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ae32615f1a234e4c49c1eedf4cabf99ac>`(float value);
		PreProcessSteps& :ref:`scale<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a888da36423fd13f6a75d7392aacedf7e>`(const std::vector<float>& values);
		PreProcessSteps& :ref:`mean<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a73234aefee9b6f7c585ac7718c1e396e>`(float value);
		PreProcessSteps& :ref:`mean<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab1a355ed40353965c430bd4056d0bb5d>`(const std::vector<float>& values);
		PreProcessSteps& :ref:`custom<doxid-classov_1_1preprocess_1_1_pre_process_steps_1af09aed52169c79fcea85a10e8f91d43d>`(const :ref:`CustomPreprocessOp<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab19b0d87acc85c3f206abdd5400630f9>`& preprocess_cb);
	
		PreProcessSteps& :ref:`resize<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a910dfdc8dc19b1890b2e8f111162a8d6>`(
			:ref:`ResizeAlgorithm<doxid-namespaceov_1_1preprocess_1a8665e295e222dc2120be3550e04db8f3>` alg,
			size_t dst_height,
			size_t dst_width
			);
	
		PreProcessSteps& :ref:`resize<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ae93d9adfd98f8ca9085501bdeb7fb38a>`(:ref:`ResizeAlgorithm<doxid-namespaceov_1_1preprocess_1a8665e295e222dc2120be3550e04db8f3>` alg);
	
		PreProcessSteps& :ref:`crop<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a682a544fc403f6eab5abc5ca7829c81e>`(
			const std::vector<int>& begin,
			const std::vector<int>& end
			);
	
		PreProcessSteps& :ref:`convert_layout<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab5a0cd9d0090f82e0489171a057fcfd4>`(const :ref:`Layout<doxid-classov_1_1_layout>`& dst_layout = {});
		PreProcessSteps& :ref:`convert_layout<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a22c36646b4268b0a2d35e83e8f0592e8>`(const std::vector<uint64_t>& dims);
		PreProcessSteps& :ref:`reverse_channels<doxid-classov_1_1preprocess_1_1_pre_process_steps_1a42371adf9ce7fc080fb836b04a8b51c0>`();
	};
.. _details-classov_1_1preprocess_1_1_pre_process_steps:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Preprocessing steps. Each step typically intends adding of some operation to input parameter User application can specify sequence of preprocessing steps in a builder-like manner.

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	proc.input().preprocess()
	                       .mean(0.2:ref:`f <doxid-namespacengraph_1_1runtime_1_1reference_1a4582949bb0b6082a5159f90c43a71ca9>`)     // Subtract 0.2 from each element
	                       .scale(2.3:ref:`f <doxid-namespacengraph_1_1runtime_1_1reference_1a4582949bb0b6082a5159f90c43a71ca9>`));   // then divide each element to 2.3

Typedefs
--------

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab19b0d87acc85c3f206abdd5400630f9:
.. index:: pair: typedef; CustomPreprocessOp

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>&node)> CustomPreprocessOp

Signature for custom preprocessing operation. Custom preprocessing operation takes one input node and produces one output node. For more advanced cases, client's code can use transformation passes over :ref:`ov::Model <doxid-classov_1_1_model>` directly.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- :ref:`Input <doxid-classov_1_1_input>` node for custom preprocessing operation (output of previous preprocessing operation)



.. rubric:: Returns:

New node after applying custom preprocessing operation

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab9e7979668e7403a72b07786f76ec0e0:
.. index:: pair: function; convert_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& convert_element_type(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type = {})

Add convert element type preprocess operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Desired type of input.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a1cc7cc3fc7afb5992c1920c483ce3332:
.. index:: pair: function; convert_color

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& convert_color(const :ref:`ov::preprocess::ColorFormat<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707>`& dst_format)

Converts color format for user's input tensor. Requires source color format to be specified by :ref:`InputTensorInfo::set_color_format <doxid-classov_1_1preprocess_1_1_input_tensor_info_1a32df813b541b01ac7df6ae93d7f1f163>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst_format

		- Destination color format of input image



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1ae32615f1a234e4c49c1eedf4cabf99ac:
.. index:: pair: function; scale

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& scale(float value)

Add scale preprocess operation Divide each element of input by specified value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- Scaling value.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a888da36423fd13f6a75d7392aacedf7e:
.. index:: pair: function; scale

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& scale(const std::vector<float>& values)

Add scale preprocess operation by specified array of scale values for each channel.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- values

		- Scaling values. :ref:`Layout <doxid-classov_1_1_layout>` runtime info with channels dimension must be specified for input tensor



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a73234aefee9b6f7c585ac7718c1e396e:
.. index:: pair: function; mean

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& mean(float value)

Add mean preprocess operation Subtract specified value from each element of input.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- Value to subtract from each element.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab1a355ed40353965c430bd4056d0bb5d:
.. index:: pair: function; mean

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& mean(const std::vector<float>& values)

Add mean preprocess operation by specified array of mean values for each channel.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- values

		- Mean values. :ref:`Layout <doxid-classov_1_1_layout>` runtime info with channels dimension must be specified for input tensor



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1af09aed52169c79fcea85a10e8f91d43d:
.. index:: pair: function; custom

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& custom(const :ref:`CustomPreprocessOp<doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab19b0d87acc85c3f206abdd5400630f9>`& preprocess_cb)

Add custom preprocess operation Client application can specify callback function for custom action.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- preprocess_cb

		- Client's custom preprocess operation.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a910dfdc8dc19b1890b2e8f111162a8d6:
.. index:: pair: function; resize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& resize(
		:ref:`ResizeAlgorithm<doxid-namespaceov_1_1preprocess_1a8665e295e222dc2120be3550e04db8f3>` alg,
		size_t dst_height,
		size_t dst_width
		)

Add resize operation to known dimensions - Lvalue version.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- alg

		- Resize algorithm.

	*
		- dst_height

		- Desired height of resized image.

	*
		- dst_width

		- Desired width of resized image.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1ae93d9adfd98f8ca9085501bdeb7fb38a:
.. index:: pair: function; resize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& resize(:ref:`ResizeAlgorithm<doxid-namespaceov_1_1preprocess_1a8665e295e222dc2120be3550e04db8f3>` alg)

Add resize operation to model's dimensions.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- alg

		- Resize algorithm.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a682a544fc403f6eab5abc5ca7829c81e:
.. index:: pair: function; crop

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& crop(
		const std::vector<int>& begin,
		const std::vector<int>& end
		)

Crop input tensor between begin and end coordinates. Under the hood, inserts ``opset8::Slice`` operation to execution graph. It is recommended to use to together with ``:ref:`ov::preprocess::InputTensorInfo::set_shape <doxid-classov_1_1preprocess_1_1_input_tensor_info_1aea4706c76671f054a4f87cec441b7a2f>``` to set original input shape before cropping.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- begin

		- Begin indexes for input tensor cropping. Negative values represent counting elements from the end of input tensor

	*
		- end

		- End indexes for input tensor cropping. End indexes are exclusive, which means values including end edge are not included in the output slice. Negative values represent counting elements from the end of input tensor



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab5a0cd9d0090f82e0489171a057fcfd4:
.. index:: pair: function; convert_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& convert_layout(const :ref:`Layout<doxid-classov_1_1_layout>`& dst_layout = {})

Add 'convert layout' operation to specified layout.

Adds appropriate 'transpose' operation between user layout and target layout. Current implementation requires source and destination layout to have same number of dimensions

Example: when user data has 'NHWC' layout (example is RGB image, [1, 224, 224, 3]) but model expects planar input image ('NCHW', [1, 3, 224, 224]). Preprocessing may look like this:

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(:ref:`model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>`);
	proc.input().tensor().set_layout("NHWC"); // User data is NHWC
	proc.input().preprocess().convert_layout("NCHW")) // model expects input as NCHW



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dst_layout

		- New layout after conversion. If not specified - destination layout is obtained from appropriate model input properties.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a22c36646b4268b0a2d35e83e8f0592e8:
.. index:: pair: function; convert_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& convert_layout(const std::vector<uint64_t>& dims)

Add convert layout operation by direct specification of transposed dimensions.

Example: when user data has input RGB image {1x480x640x3} but model expects planar input image ('NCHW', [1, 3, 480, 640]). Preprocessing may look like this:

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	proc.input().preprocess().convert_layout({0, 3, 1, 2});



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- dims

		- Dimensions array specifying places for new axis. If not empty, array size (N) must match to input shape rank. Array values shall contain all values from 0 to N-1. If empty, no actual conversion will be added.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_pre_process_steps_1a42371adf9ce7fc080fb836b04a8b51c0:
.. index:: pair: function; reverse_channels

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PreProcessSteps& reverse_channels()

Reverse channels operation.

Adds appropriate operation which reverses channels layout. Operation requires layout having 'C' dimension Operation convert_color (RGB<->BGR) does reversing of channels also, but only for NHWC layout

Example: when user data has 'NCHW' layout (example is [1, 3, 224, 224] RGB order) but model expects BGR planes order. Preprocessing may look like this:

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	proc.input().tensor().set_layout("NCHW"); // User data is NCHW
	proc.input().preprocess().reverse_channels();



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.


