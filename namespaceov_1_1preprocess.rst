.. index:: pair: namespace; ov::preprocess
.. _doxid-namespaceov_1_1preprocess:

namespace ov::preprocess
========================

.. toctree::
	:hidden:

	ColorFormat <enumov_1_1preprocess_1_1ColorFormat.rst>
	ResizeAlgorithm <enumov_1_1preprocess_1_1ResizeAlgorithm.rst>
	InputInfo <classov_1_1preprocess_1_1InputInfo.rst>
	InputModelInfo <classov_1_1preprocess_1_1InputModelInfo.rst>
	InputTensorInfo <classov_1_1preprocess_1_1InputTensorInfo.rst>
	OutputInfo <classov_1_1preprocess_1_1OutputInfo.rst>
	OutputModelInfo <classov_1_1preprocess_1_1OutputModelInfo.rst>
	OutputTensorInfo <classov_1_1preprocess_1_1OutputTensorInfo.rst>
	PostProcessSteps <classov_1_1preprocess_1_1PostProcessSteps.rst>
	PreProcessSteps <classov_1_1preprocess_1_1PreProcessSteps.rst>
	TensorInfoMemoryType <classov_1_1preprocess_1_1TensorInfoMemoryType.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace preprocess {

	// enums

	enum :ref:`ColorFormat<doxid-namespaceov_1_1preprocess_1ab027f26e58038e454e1b50a5243f1707>`;
	enum :ref:`ResizeAlgorithm<doxid-namespaceov_1_1preprocess_1a8665e295e222dc2120be3550e04db8f3>`;

	// classes

	class :ref:`InputInfo<doxid-classov_1_1preprocess_1_1_input_info>`;
	class :ref:`InputModelInfo<doxid-classov_1_1preprocess_1_1_input_model_info>`;
	class :ref:`InputTensorInfo<doxid-classov_1_1preprocess_1_1_input_tensor_info>`;
	class :ref:`OutputInfo<doxid-classov_1_1preprocess_1_1_output_info>`;
	class :ref:`OutputModelInfo<doxid-classov_1_1preprocess_1_1_output_model_info>`;
	class :ref:`OutputTensorInfo<doxid-classov_1_1preprocess_1_1_output_tensor_info>`;
	class :ref:`PostProcessSteps<doxid-classov_1_1preprocess_1_1_post_process_steps>`;
	class :ref:`PrePostProcessor<doxid-classov_1_1preprocess_1_1_pre_post_processor>`;
	class :ref:`PreProcessSteps<doxid-classov_1_1preprocess_1_1_pre_process_steps>`;
	class :ref:`TensorInfoMemoryType<doxid-classov_1_1preprocess_1_1_tensor_info_memory_type>`;

	// global functions

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& :ref:`operator <<<doxid-namespaceov_1_1preprocess_1a77b9c0eb634c3acb9ea54a7143960a2a>` (
		std::ostream& str,
		const :ref:`PrePostProcessor<doxid-classov_1_1preprocess_1_1_pre_post_processor>`& prePostProcessor
		);

	} // namespace preprocess
.. _details-namespaceov_1_1preprocess:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespaceov_1_1preprocess_1a77b9c0eb634c3acb9ea54a7143960a2a:
.. index:: pair: function; operator<<

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::ostream& operator << (
		std::ostream& str,
		const :ref:`PrePostProcessor<doxid-classov_1_1preprocess_1_1_pre_post_processor>`& prePostProcessor
		)

Inserts a human-readable representation of a PrePostProcessors into an output stream. The output to the stream is in "informal" notation and can be used for debugging purposes.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- str

		- The output stream targeted for insertion.

	*
		- prePostProcessor

		- The shape to be inserted into output stream.



.. rubric:: Returns:

A reference to same output stream after insertion.

