.. index:: pair: class; ngraph::pass::low_precision::CreateAttribute
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_create_attribute:

class ngraph::pass::low_precision::CreateAttribute
==================================================



Overview
~~~~~~~~

:ref:`CreateAttribute <doxid-classngraph_1_1pass_1_1low__precision_1_1_create_attribute>` transformation marks OperationType operations by AttributeType attribute. :ref:`More...<details-classngraph_1_1pass_1_1low__precision_1_1_create_attribute>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <create_attribute.hpp>
	
	template <
		typename AttributeType,
		typename OperationType = ngraph::pattern::op::Label
		>
	class CreateAttribute
	{
	public:
		// construction
	
		:target:`CreateAttribute<doxid-classngraph_1_1pass_1_1low__precision_1_1_create_attribute_1ab2c26e608b997214a103ebe74264274d>`(
			const :ref:`AttributeParameters<doxid-class_attribute_parameters>`& params = :ref:`AttributeParameters<doxid-class_attribute_parameters>`(),
			const :ref:`AttributeSource<doxid-create__attribute_8hpp_1a78c045d573f15c7ad7bfb0accb0c162e>` source = :ref:`AttributeSource::Node<doxid-create__attribute_8hpp_1a78c045d573f15c7ad7bfb0accb0c162ea6c3a6944a808a7c0bbb6788dbec54a9f>`
			);
	};
.. _details-classngraph_1_1pass_1_1low__precision_1_1_create_attribute:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`CreateAttribute <doxid-classngraph_1_1pass_1_1low__precision_1_1_create_attribute>` transformation marks OperationType operations by AttributeType attribute.

For more details about the transformation, refer to :ref:`CreateAttribute <doxid-openvino_docs__o_v__u_g_lpt__create_attribute>` page in the Inference Engine Developer Guide.


