.. index:: pair: class; ov::op::util::ActivationFunction
.. _doxid-classov_1_1op_1_1util_1_1_activation_function:

class ov::op::util::ActivationFunction
======================================



Overview
~~~~~~~~

Class representing activation function used in RNN cells. :ref:`More...<details-classov_1_1op_1_1util_1_1_activation_function>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <activation_functions.hpp>
	
	class ActivationFunction
	{
	public:
		// construction
	
		:target:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function_1a3c5e51ba8a479b1071842a762b9fa456>`(:ref:`ActivationFunctionType<doxid-namespaceov_1_1op_1_1util_1a9f70582388f029216424805b5f53343a>` f, float alpha, float beta);
		:target:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function_1a27181e2eae616a3a04a879b8dfaf757d>`(:ref:`ActivationFunctionType<doxid-namespaceov_1_1op_1_1util_1a9f70582388f029216424805b5f53343a>` f, float alpha);
		:target:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function_1a20a7949799ebd0e754928fa75700523b>`(:ref:`ActivationFunctionType<doxid-namespaceov_1_1op_1_1util_1a9f70582388f029216424805b5f53343a>` f);
		:target:`ActivationFunction<doxid-classov_1_1op_1_1util_1_1_activation_function_1a670999cb91d3a78a3bcaeffee277e2b6>`();

		// methods
	
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`operator ()<doxid-classov_1_1op_1_1util_1_1_activation_function_1a60abd23e5ef9f10cb2dc4b34f75c00bc>` (const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& arg) const;
		void :target:`set_alpha<doxid-classov_1_1op_1_1util_1_1_activation_function_1a617b62a55d8af97ac6c7e08e825037bb>`(float alpha);
		void :target:`set_beta<doxid-classov_1_1op_1_1util_1_1_activation_function_1ae40c52219797393ae1ff741058dd4c84>`(float beta);
	};
.. _details-classov_1_1op_1_1util_1_1_activation_function:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class representing activation function used in RNN cells.

Methods
-------

.. _doxid-classov_1_1op_1_1util_1_1_activation_function_1a60abd23e5ef9f10cb2dc4b34f75c00bc:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> operator () (const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& arg) const

Calls stored activation function with provided node argument.


