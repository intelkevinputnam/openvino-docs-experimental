.. index:: pair: class; ov::descriptor::Output
.. _doxid-classov_1_1descriptor_1_1_output:

class ov::descriptor::Output
============================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <output.hpp>
	
	class Output
	{
	public:
		// construction
	
		:target:`Output<doxid-classov_1_1descriptor_1_1_output_1acbbb03c2f95e9979898d4cd6ca87d93d>`();
		:ref:`Output<doxid-classov_1_1descriptor_1_1_output_1a609c9c631c8c66827f3044db921affeb>`(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index, const std::shared_ptr<:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`>& tensor);
		:target:`Output<doxid-classov_1_1descriptor_1_1_output_1a1174efdc64470c0c65261d9dc5368c0d>`(const Output&);
		:target:`Output<doxid-classov_1_1descriptor_1_1_output_1a9c7befae93593e75ec3f193f752037e6>`(Output&&);

		// methods
	
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_node<doxid-classov_1_1descriptor_1_1_output_1a392e827538f2915cd272f86719f95660>`() const;
		size_t :target:`get_index<doxid-classov_1_1descriptor_1_1_output_1a3c282c03ecc0339da5723002b86ba35f>`() const;
		:ref:`ov::Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`get_output<doxid-classov_1_1descriptor_1_1_output_1adff4afd8729a22bae92cfa0cdf24860e>`() const;
		std::shared_ptr<:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> :target:`get_tensor_ptr<doxid-classov_1_1descriptor_1_1_output_1a46095e63e8d10cdebc6529573ab58069>`() const;
		void :target:`set_tensor_ptr<doxid-classov_1_1descriptor_1_1_output_1a27526923ea6182dfb1f8d84be96bb646>`(const std::shared_ptr<:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`>& tensor);
		void :target:`add_input<doxid-classov_1_1descriptor_1_1_output_1aa067876f7bfb8c2ba58116f6239baf2f>`(:ref:`Input<doxid-classov_1_1descriptor_1_1_input>` \* input);
		void :target:`remove_input<doxid-classov_1_1descriptor_1_1_output_1a259b126612936c1e4246460d706a3c5b>`(:ref:`Input<doxid-classov_1_1descriptor_1_1_input>` \* input);
		const std::vector<:ref:`Input<doxid-classov_1_1descriptor_1_1_input>` \*>& :target:`get_inputs<doxid-classov_1_1descriptor_1_1_output_1af6bd6b9a888356c3c2d3f5dfcd5a77e2>`() const;
		:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :target:`get_tensor<doxid-classov_1_1descriptor_1_1_output_1aa690197ee3568637904175d8d3d02499>`() const;
		:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1descriptor_1_1_output_1a8dd979e8ae126aa2f999a270cb4d3912>`();
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1descriptor_1_1_output_1a5f4eb37d12002fd150495a8710a5cd2f>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1descriptor_1_1_output_1a4982ba689d90a816ea7252f33c389cb2>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classov_1_1descriptor_1_1_output_1acddaa8fda96e3779ee987835a4bbe0fd>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1descriptor_1_1_output_1a11b616a0660dedd61f7307a1b96d200f>`() const;
		Output& :target:`operator =<doxid-classov_1_1descriptor_1_1_output_1a5c6c156825f422c05781d5109a790cb4>` (const Output&);
	};
.. _details-classov_1_1descriptor_1_1_output:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Construction
------------

.. _doxid-classov_1_1descriptor_1_1_output_1a609c9c631c8c66827f3044db921affeb:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index, const std::shared_ptr<:ref:`Tensor<doxid-classov_1_1descriptor_1_1_tensor>`>& tensor)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- :ref:`Node <doxid-classov_1_1_node>` that owns this output.

	*
		- index

		- Position of the output tensor in all output tensors

	*
		- tensor

		- The tensor where the value will be written

Methods
-------

.. _doxid-classov_1_1descriptor_1_1_output_1a4982ba689d90a816ea7252f33c389cb2:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_shape() const



.. rubric:: Returns:

the shape of the output

.. _doxid-classov_1_1descriptor_1_1_output_1acddaa8fda96e3779ee987835a4bbe0fd:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const



.. rubric:: Returns:

the partial shape of the output

.. _doxid-classov_1_1descriptor_1_1_output_1a11b616a0660dedd61f7307a1b96d200f:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const



.. rubric:: Returns:

the element type of the output


