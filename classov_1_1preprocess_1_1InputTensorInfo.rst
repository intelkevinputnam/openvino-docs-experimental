.. index:: pair: class; ov::preprocess::InputTensorInfo
.. _doxid-classov_1_1preprocess_1_1_input_tensor_info:

class ov::preprocess::InputTensorInfo
=====================================



Overview
~~~~~~~~

Information about user's input tensor. By default, it will be initialized to same data (type/shape/etc) as model's input parameter. User application can override particular parameters (like 'element_type') according to application's data and specify appropriate conversions in pre-processing steps. :ref:`More...<details-classov_1_1preprocess_1_1_input_tensor_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <input_tensor_info.hpp>
	
	class InputTensorInfo
	{
	public:
		// methods
	
		InputTensorInfo& :ref:`set_element_type<doxid-classov_1_1preprocess_1_1_input_tensor_info_1a320c54e50d794da07852ccecf9468e2a>`(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type);
		InputTensorInfo& :ref:`set_layout<doxid-classov_1_1preprocess_1_1_input_tensor_info_1af10932e00c45bb0ef09b2f856fab5268>`(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout);
		InputTensorInfo& :ref:`set_spatial_dynamic_shape<doxid-classov_1_1preprocess_1_1_input_tensor_info_1a924a6b32f6ed1427a16f2ab2d47892f9>`();
		InputTensorInfo& :ref:`set_spatial_static_shape<doxid-classov_1_1preprocess_1_1_input_tensor_info_1a03db58db580f2974469a01da5b03f511>`(size_t height, size_t width);
	
		InputTensorInfo& :ref:`set_color_format<doxid-classov_1_1preprocess_1_1_input_tensor_info_1a32df813b541b01ac7df6ae93d7f1f163>`(
			const :ref:`ov::preprocess::ColorFormat<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707>`& format,
			const std::vector<std::string>& sub_names = {}
			);
	
		InputTensorInfo& :ref:`set_memory_type<doxid-classov_1_1preprocess_1_1_input_tensor_info_1ae170f7c198591f9de58279692012a065>`(const std::string& memory_type);
		InputTensorInfo& :ref:`set_shape<doxid-classov_1_1preprocess_1_1_input_tensor_info_1aea4706c76671f054a4f87cec441b7a2f>`(const :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& shape);
		InputTensorInfo& :ref:`set_from<doxid-classov_1_1preprocess_1_1_input_tensor_info_1a4c64b5adcd93e6fcb450a9b8399d0f79>`(const :ref:`ov::Tensor<doxid-classov_1_1_tensor>`& runtime_tensor);
	};
.. _details-classov_1_1preprocess_1_1_input_tensor_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Information about user's input tensor. By default, it will be initialized to same data (type/shape/etc) as model's input parameter. User application can override particular parameters (like 'element_type') according to application's data and specify appropriate conversions in pre-processing steps.

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	proc.input().tensor().set_element_type(:ref:`ov::element::u8 <doxid-group__ov__element__cpp__api_1gaaf60c536d3e295285f6a899eb3d29e2f>`);

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1a320c54e50d794da07852ccecf9468e2a:
.. index:: pair: function; set_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_element_type(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type)

Set element type for user's input tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Element type for user's input tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1af10932e00c45bb0ef09b2f856fab5268:
.. index:: pair: function; set_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_layout(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout)

Set layout for user's input tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layout

		- :ref:`Layout <doxid-classov_1_1_layout>` for user's input tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1a924a6b32f6ed1427a16f2ab2d47892f9:
.. index:: pair: function; set_spatial_dynamic_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_spatial_dynamic_shape()

By default, input image shape is inherited from model input shape. This method specifies that user's input image has dynamic spatial dimensions (width & height). This can be useful for adding resize preprocessing from any input image to model's expected dimensions.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1a03db58db580f2974469a01da5b03f511:
.. index:: pair: function; set_spatial_static_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_spatial_static_shape(size_t height, size_t width)

By default, input image shape is inherited from model input shape. Use this method to specify different width and height of user's input image. In case if input image size is not known, use ``set_spatial_dynamic_shape`` method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- height

		- Set fixed user's input image height.

	*
		- width

		- Set fixed user's input image width.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1a32df813b541b01ac7df6ae93d7f1f163:
.. index:: pair: function; set_color_format

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_color_format(
		const :ref:`ov::preprocess::ColorFormat<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707>`& format,
		const std::vector<std::string>& sub_names = {}
		)

Set color format for user's input tensor.

In general way, some formats support multi-plane input, e.g. NV12 image can be represented as 2 separate tensors (planes): Y plane and UV plane. set_color_format API also allows to set sub_names for such parameters for convenient usage of plane parameters. During build stage, new parameters for each plane will be inserted to the place of original parameter. This means that all parameters located after will shift their positions accordingly (e.g. {param1, param2} will become {param1/Y, param1/UV, param2})



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- format

		- Color format of input image.

	*
		- sub_names

		- Optional list of sub-names assigned for each plane (e.g. {"Y", "UV"}). If specified, number of sub-names shall match with number of planes. If not specified, friendly name and tensor name for plane parameters will be empty. It is not allowed to specify sub-names for single-plane inputs.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1ae170f7c198591f9de58279692012a065:
.. index:: pair: function; set_memory_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_memory_type(const std::string& memory_type)

Set memory type runtime information for user's input tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- memory_type

		- Memory type. Refer to specific plugin's documentation for exact string format



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1aea4706c76671f054a4f87cec441b7a2f:
.. index:: pair: function; set_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_shape(const :ref:`ov::PartialShape<doxid-classov_1_1_partial_shape>`& shape)

By default, input shape is inherited from model's input shape. Use this method to specify different input data shape. If it is needed to change only input height & width of input image, consider define layout and use set_spatial_static_shape or 'set_spatial_dynamic_shape' instead. This method allows defining any custom input shape and can be useful for custom preprocessing operations.

Methods 'set_spatial_dynamic_shape', 'set_spatial_static_shape' are also intended to modify input shape, using those methods together will throw :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>` exception



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- shape

		- New shape for input tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_input_tensor_info_1a4c64b5adcd93e6fcb450a9b8399d0f79:
.. index:: pair: function; set_from

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputTensorInfo& set_from(const :ref:`ov::Tensor<doxid-classov_1_1_tensor>`& runtime_tensor)

Helper function to reuse element type and shape from user's created tensor. Use this only in case if input tensor is already known and available before. Overwrites previously set element type & shape via ``set_element_type`` and ``set_shape``. :ref:`Tensor <doxid-classov_1_1_tensor>` 's memory type is not reused, so if ``runtime_tensor`` represents remote tensor with particular memory type - you should still specify appropriate memory type manually using ``set_memory_type``

As for ``:ref:`InputTensorInfo::set_shape <doxid-classov_1_1preprocess_1_1_input_tensor_info_1aea4706c76671f054a4f87cec441b7a2f>```, this method shall not be used together with methods 'set_spatial_dynamic_shape' and 'set_spatial_static_shape', otherwise :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>` exception will be thrown



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- runtime_tensor

		- User's created tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.


