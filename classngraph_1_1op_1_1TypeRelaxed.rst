.. index:: pair: class; ngraph::op::TypeRelaxed
.. _doxid-classngraph_1_1op_1_1_type_relaxed:

class ngraph::op::TypeRelaxed
=============================



Overview
~~~~~~~~

Relaxes tensor element type requirements for BaseOp inputs and outputs This class template should be used with Node descendant class. :ref:`More...<details-classngraph_1_1op_1_1_type_relaxed>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <type_relaxed.hpp>
	
	template <typename BaseOp>
	class TypeRelaxed:
	    public BaseOp,
	    public :ref:`ngraph::op::TypeRelaxedBase<doxid-classngraph_1_1op_1_1_type_relaxed_base>`
	{
	public:
		// construction
	
		:target:`TypeRelaxed<doxid-classngraph_1_1op_1_1_type_relaxed_1ae380276784b703addb16298efc81a15b>`();
		:target:`TypeRelaxed<doxid-classngraph_1_1op_1_1_type_relaxed_1a3296db556ae736e092b808579236fc91>`(const BaseOp& base_op, :ref:`element::Type<doxid-classov_1_1element_1_1_type>` overridden_type);
	
		:target:`TypeRelaxed<doxid-classngraph_1_1op_1_1_type_relaxed_1affc3b9370703ab20c5cf4061a0d5eea1>`(
			const BaseOp& base_op,
			const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _input_data_types = {},
			const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _output_data_types = {}
			);
	
		template <typename... Args>
		:ref:`TypeRelaxed<doxid-classngraph_1_1op_1_1_type_relaxed_1a52d3bfb12e96ff8d3a38a33b0e8a5dee>`(
			const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _input_data_types,
			const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _output_data_types,
			Args&&... args
			);

		// methods
	
		void :target:`validate_and_infer_types<doxid-classngraph_1_1op_1_1_type_relaxed_1acffcd8797edc65e00a042c4ca4401319>`();
	
		:ref:`OPENVINO_SUPPRESS_DEPRECATED_START<doxid-openvino_2core_2deprecated_8hpp_1a80720d314461cf6f3098efd1719f54c5>` bool :target:`evaluate<doxid-classngraph_1_1op_1_1_type_relaxed_1a2f303c2b740dcb879d8390cdbc7eb855>`(
			const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& outputs,
			const :ref:`HostTensorVector<doxid-classngraph_1a4c69b1e96e984658be3a087d0610e67b>`& inputs
			) const;
	
		:ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`clone_with_new_inputs<doxid-classngraph_1_1op_1_1_type_relaxed_1a9415a16366b4c81c7bb301dd4ddb232b>`(const :ref:`OutputVector<doxid-classngraph_1a161d36c81df2d1949272f525a8d73605>`& new_args) const;
		bool :target:`visit_attributes<doxid-classngraph_1_1op_1_1_type_relaxed_1aa5158c96ffa8c99f41cc367289b9d596>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// structs
	
		struct :ref:`init_rt_result<doxid-structngraph_1_1op_1_1_type_relaxed_base_1_1init__rt__result>`;

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

.. _details-classngraph_1_1op_1_1_type_relaxed:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Relaxes tensor element type requirements for BaseOp inputs and outputs This class template should be used with Node descendant class. Defines a new operation by extending the original BaseOp operation with ability to accept inputs and provide outputs with element type that is unusual for BaseOp. For example, :ref:`TypeRelaxed\<opset1::Add> <doxid-classngraph_1_1op_1_1_type_relaxed_1ae380276784b703addb16298efc81a15b>` can accept mixed-precision inputs and provide another type of output. New types are provided as inputs attributes for :ref:`TypeRelaxed <doxid-classngraph_1_1op_1_1_type_relaxed>` template and fixed. There is no any deduction logic for types are provided as a part of this class and it should be implemented outside if required.

Construction
------------

.. _doxid-classngraph_1_1op_1_1_type_relaxed_1a52d3bfb12e96ff8d3a38a33b0e8a5dee:
.. index:: pair: function; TypeRelaxed

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Args>
	TypeRelaxed(
		const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _input_data_types,
		const :ref:`element::TypeVector<doxid-namespacengraph_1_1element_1a043e3b75d5062cd4deea2f2c00eb132c>`& _output_data_types,
		Args&&... args
		)

Creating a new :ref:`TypeRelaxed <doxid-classngraph_1_1op_1_1_type_relaxed>` operation by calling one of the original op ctors forwarding arguments directly.


