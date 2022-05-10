.. index:: pair: class; ngraph::op::TypeRelaxedBase
.. _doxid-classngraph_1_1op_1_1_type_relaxed_base:

class ngraph::op::TypeRelaxedBase
=================================

.. toctree::
	:hidden:

	init_rt_result <structngraph_1_1op_1_1TypeRelaxedBase_1_1init_rt_result.rst>

Overview
~~~~~~~~

A base class for templated :ref:`TypeRelaxed <doxid-classngraph_1_1op_1_1_type_relaxed>` that maintains overridden input types and output types for an operation. :ref:`More...<details-classngraph_1_1op_1_1_type_relaxed_base>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <type_relaxed.hpp>
	
	class TypeRelaxedBase
	{
	public:
		// structs
	
		struct :ref:`init_rt_result<doxid-structngraph_1_1op_1_1_type_relaxed_base_1_1init__rt__result>`;

		// construction
	
		:target:`TypeRelaxedBase<doxid-classngraph_1_1op_1_1_type_relaxed_base_1a2e55af691df5dcbe867b9c066f411b7b>`(
			const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _input_data_types = {},
			const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _output_data_types = {}
			);

		// methods
	
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_overridden_output_type<doxid-classngraph_1_1op_1_1_type_relaxed_base_1a275253061c20bbf42014d8be16a8ec89>`(size_t outputIndex = 0) const;
	
		void :ref:`set_overridden_output_type<doxid-classngraph_1_1op_1_1_type_relaxed_base_1ad8174e14b026b9fc8a931aa19d8696b1>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			size_t outputIndex = 0
			);
	
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_origin_input_type<doxid-classngraph_1_1op_1_1_type_relaxed_base_1aa039f5bdb5a9b01839a6cfced5f82a82>`(size_t inputIndex = 0) const;
	
		void :ref:`set_origin_input_type<doxid-classngraph_1_1op_1_1_type_relaxed_base_1a5e4adfa461ad669b451c769ccdf5d7ed>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			size_t inputIndex = 0
			);
	};

	// direct descendants

	template <typename BaseOp>
	class :ref:`TypeRelaxed<doxid-classngraph_1_1op_1_1_type_relaxed>`;
.. _details-classngraph_1_1op_1_1_type_relaxed_base:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A base class for templated :ref:`TypeRelaxed <doxid-classngraph_1_1op_1_1_type_relaxed>` that maintains overridden input types and output types for an operation.

Methods
-------

.. _doxid-classngraph_1_1op_1_1_type_relaxed_base_1a275253061c20bbf42014d8be16a8ec89:
.. index:: pair: function; get_overridden_output_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_overridden_output_type(size_t outputIndex = 0) const

This method may look similar to :ref:`Node::get_output_element_type <doxid-classov_1_1_node_1af54b4c4728f6fe535e00979c04181926>`, but it is not the same thing, because get_output_element_type returns the result of type inference, so it is completely deduced from an operation inputs and attributes, and get_overridden_output_type returns value of the attribute that is used to deduce output type. In some cases they don't match: get_overridden_output_type may return element::undefined for some index i, and get_output_element_type will return some real type for the same index i.



.. rubric:: Returns:

Data type that will be set for output with a given index outputIndex. If output with a specified index outputIndex hasn't been set before, element::undefined will returned. Undefined means no type override happens for a given outputIndex and it will deduced as original operation defineds in its infer function.

.. _doxid-classngraph_1_1op_1_1_type_relaxed_base_1ad8174e14b026b9fc8a931aa19d8696b1:
.. index:: pair: function; set_overridden_output_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_overridden_output_type(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
		size_t outputIndex = 0
		)

Set data type that overrides the original data type for output port with outputIndex index In case if outputIndex is out of range of known outputs (and this class cannot detect the real number of outputs for original operation), the number of overridden outputs is changed according to a given outputIndex value.

.. _doxid-classngraph_1_1op_1_1_type_relaxed_base_1aa039f5bdb5a9b01839a6cfced5f82a82:
.. index:: pair: function; get_origin_input_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_origin_input_type(size_t inputIndex = 0) const



.. rubric:: Returns:

Data type that will be set for input when original shape/type inference function is called. If index inputIndex hasn't been set before, element::undefined will returned. Undefined means that the type from input tensor descriptor is used for a given index.

.. _doxid-classngraph_1_1op_1_1_type_relaxed_base_1a5e4adfa461ad669b451c769ccdf5d7ed:
.. index:: pair: function; set_origin_input_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_origin_input_type(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
		size_t inputIndex = 0
		)

Set data type that overrides the original data type for input port with inputIndex index. In case if inputIndex is out of range of known inputs (and this class cannot detect the real number of inputs for original operation), the number of overridden inputs is changed according to a given inputIndex value. All new entries except one added at inputIndex position are undefined.


