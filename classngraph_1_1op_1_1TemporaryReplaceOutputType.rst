.. index:: pair: class; ngraph::op::TemporaryReplaceOutputType
.. _doxid-classngraph_1_1op_1_1_temporary_replace_output_type:

class ngraph::op::TemporaryReplaceOutputType
============================================



Overview
~~~~~~~~

Set another type for a specified output for the period of time when an instance of the class exists. :ref:`More...<details-classngraph_1_1op_1_1_temporary_replace_output_type>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <type_relaxed.hpp>
	
	class TemporaryReplaceOutputType
	{
	public:
		// construction
	
		:ref:`TemporaryReplaceOutputType<doxid-classngraph_1_1op_1_1_temporary_replace_output_type_1afda84d2bd58e10814eb9b76a331ec179>`(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> output, :ref:`element::Type<doxid-classov_1_1element_1_1_type>` tmp_type);

		// methods
	
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get<doxid-classngraph_1_1op_1_1_temporary_replace_output_type_1a7ca86d1f311628efc3fb249ff6a143da>`() const;
	};
.. _details-classngraph_1_1op_1_1_temporary_replace_output_type:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set another type for a specified output for the period of time when an instance of the class exists. When the execution leaves the scope where an onject of :ref:`TemporaryReplaceOutputType <doxid-classngraph_1_1op_1_1_temporary_replace_output_type>` is defined, the type of the output is set to its original value. Used when initialized TypeRelaxed<BaseOp> operation in case when inputs have types that are not compatible with BaseOp infer function. In this case before :ref:`TypeRelaxed <doxid-classngraph_1_1op_1_1_type_relaxed>` is constructed the BaseOp contructor requires modified data types. So it should be

Construction
------------

.. _doxid-classngraph_1_1op_1_1_temporary_replace_output_type_1afda84d2bd58e10814eb9b76a331ec179:
.. index:: pair: function; TemporaryReplaceOutputType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TemporaryReplaceOutputType(:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> output, :ref:`element::Type<doxid-classov_1_1element_1_1_type>` tmp_type)

Replace element type for a given output port by tmp_type.

Methods
-------

.. _doxid-classngraph_1_1op_1_1_temporary_replace_output_type_1a7ca86d1f311628efc3fb249ff6a143da:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get() const

Return the output port that was used in the constructor.


