.. index:: pair: class; ov::preprocess::InputInfo
.. _doxid-classov_1_1preprocess_1_1_input_info:

class ov::preprocess::InputInfo
===============================



Overview
~~~~~~~~

Class holding preprocessing information for one input From preprocessing pipeline perspective, each input can be represented as: :ref:`More...<details-classov_1_1preprocess_1_1_input_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <input_info.hpp>
	
	class InputInfo
	{
	public:
		// construction
	
		:ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info_1a10c4f04f7c95e215ecacadfeb377a14c>`(InputInfo&& other);

		// methods
	
		InputInfo& :ref:`operator =<doxid-classov_1_1preprocess_1_1_input_info_1a512090237901db9d5ac40c98e921485e>` (InputInfo&& other);
		:ref:`InputTensorInfo<doxid-classov_1_1preprocess_1_1_input_tensor_info>`& :ref:`tensor<doxid-classov_1_1preprocess_1_1_input_info_1ac7dbfe9df70c8961d9c58af5745dc4f6>`();
		:ref:`PreProcessSteps<doxid-classov_1_1preprocess_1_1_pre_process_steps>`& :ref:`preprocess<doxid-classov_1_1preprocess_1_1_input_info_1a8d8f9165adf4f4c6249a7c52af8a5eff>`();
		:ref:`InputModelInfo<doxid-classov_1_1preprocess_1_1_input_model_info>`& :ref:`model<doxid-classov_1_1preprocess_1_1_input_info_1af0210a5809c4721a07d006611b3dab98>`();
	};
.. _details-classov_1_1preprocess_1_1_input_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class holding preprocessing information for one input From preprocessing pipeline perspective, each input can be represented as:

* User's input parameter info (:ref:`InputInfo::tensor <doxid-classov_1_1preprocess_1_1_input_info_1ac7dbfe9df70c8961d9c58af5745dc4f6>`)

* Preprocessing steps applied to user's input (:ref:`InputInfo::preprocess <doxid-classov_1_1preprocess_1_1_input_info_1a8d8f9165adf4f4c6249a7c52af8a5eff>`)

* :ref:`Model <doxid-classov_1_1_model>` 's input info, which is a final input's info after preprocessing (:ref:`InputInfo::model <doxid-classov_1_1preprocess_1_1_input_info_1af0210a5809c4721a07d006611b3dab98>`)

Construction
------------

.. _doxid-classov_1_1preprocess_1_1_input_info_1a10c4f04f7c95e215ecacadfeb377a14c:
.. index:: pair: function; InputInfo

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputInfo(InputInfo&& other)

Move constructor.

Methods
-------

.. _doxid-classov_1_1preprocess_1_1_input_info_1a512090237901db9d5ac40c98e921485e:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InputInfo& operator = (InputInfo&& other)

Move assignment operator.

.. _doxid-classov_1_1preprocess_1_1_input_info_1ac7dbfe9df70c8961d9c58af5745dc4f6:
.. index:: pair: function; tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InputTensorInfo<doxid-classov_1_1preprocess_1_1_input_tensor_info>`& tensor()

Get current input tensor information with ability to change specific data.



.. rubric:: Returns:

Reference to current input tensor structure

.. _doxid-classov_1_1preprocess_1_1_input_info_1a8d8f9165adf4f4c6249a7c52af8a5eff:
.. index:: pair: function; preprocess

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PreProcessSteps<doxid-classov_1_1preprocess_1_1_pre_process_steps>`& preprocess()

Get current input preprocess information with ability to add more preprocessing steps.



.. rubric:: Returns:

Reference to current preprocess steps structure

.. _doxid-classov_1_1preprocess_1_1_input_info_1af0210a5809c4721a07d006611b3dab98:
.. index:: pair: function; model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`InputModelInfo<doxid-classov_1_1preprocess_1_1_input_model_info>`& model()

Get current input model information with ability to change original model's input data.



.. rubric:: Returns:

Reference to current model's input information structure


