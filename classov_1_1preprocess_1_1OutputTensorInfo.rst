.. index:: pair: class; ov::preprocess::OutputTensorInfo
.. _doxid-classov_1_1preprocess_1_1_output_tensor_info:

class ov::preprocess::OutputTensorInfo
======================================



Overview
~~~~~~~~

Information about user's desired output tensor. By default, it will be initialized to same data (type/shape/etc) as model's output parameter. User application can override particular parameters (like 'element_type') according to application's data and specify appropriate conversions in post-processing steps. :ref:`More...<details-classov_1_1preprocess_1_1_output_tensor_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <output_tensor_info.hpp>
	
	class OutputTensorInfo
	{
	public:
		// methods
	
		OutputTensorInfo& :ref:`set_element_type<doxid-classov_1_1preprocess_1_1_output_tensor_info_1a9c2a13f397541993747a5bce4165d17e>`(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type);
		OutputTensorInfo& :ref:`set_layout<doxid-classov_1_1preprocess_1_1_output_tensor_info_1a948528d67d6e174190a53864b24472c6>`(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout);
	};
.. _details-classov_1_1preprocess_1_1_output_tensor_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Information about user's desired output tensor. By default, it will be initialized to same data (type/shape/etc) as model's output parameter. User application can override particular parameters (like 'element_type') according to application's data and specify appropriate conversions in post-processing steps.

.. ref-code-block:: cpp

	auto proc = PrePostProcessor(function);
	auto& output = proc.output();
	output.postprocess().<:ref:`add <doxid-namespacengraph_1_1runtime_1_1reference_1a12956a756feab4106f4f12a6a372db41>` steps + conversion to user's output element type>;
	output.tensor().set_element_type(ov::element::u8);
	function = proc.build();

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_output_tensor_info_1a9c2a13f397541993747a5bce4165d17e:
.. index:: pair: function; set_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OutputTensorInfo& set_element_type(const :ref:`ov::element::Type<doxid-classov_1_1element_1_1_type>`& type)

Set element type for user's desired output tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Element type for user's output tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner.

.. _doxid-classov_1_1preprocess_1_1_output_tensor_info_1a948528d67d6e174190a53864b24472c6:
.. index:: pair: function; set_layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OutputTensorInfo& set_layout(const :ref:`ov::Layout<doxid-classov_1_1_layout>`& layout)

Set layout for user's output tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layout

		- :ref:`Layout <doxid-classov_1_1_layout>` for user's output tensor.



.. rubric:: Returns:

Reference to 'this' to allow chaining with other calls in a builder-like manner


