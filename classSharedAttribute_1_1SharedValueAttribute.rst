.. index:: pair: class; SharedAttribute::SharedValueAttribute
.. _doxid-class_shared_attribute_1_1_shared_value_attribute:

class SharedAttribute::SharedValueAttribute
===========================================

.. toctree::
	:hidden:

	SharedValue <structSharedAttribute_1_1SharedValueAttribute_1_1SharedValue.rst>

:ref:`SharedValueAttribute <doxid-class_shared_attribute_1_1_shared_value_attribute>` type for shared value attributes. The attribute is used for attribute :ref:`SharedValue <doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value>` value backward propagation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <shared_value_attribute.hpp>
	
	class SharedValueAttribute: public std::enable_shared_from_this< SharedValueAttribute >
	{
	public:
		// structs
	
		struct :ref:`SharedValue<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value>`;

		// fields
	
		std::shared_ptr<:ref:`SharedValue<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value>`> :ref:`sharedValue<doxid-class_shared_attribute_1_1_shared_value_attribute_1ac3ad0b23aa29a08fca36a0607cac6c82>`;

		// construction
	
		:ref:`SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute_1aca8a265bb00ccd370e922027f540e35b>`();
		:ref:`SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute_1a398db5a6d98ab446a4b936fd66aa8982>`(const T& value);

		// methods
	
		std::string :ref:`get_string<doxid-class_shared_attribute_1_1_shared_value_attribute_1a20f79d7c5c6ddd88c63c9296cc853fed>`();
	};

