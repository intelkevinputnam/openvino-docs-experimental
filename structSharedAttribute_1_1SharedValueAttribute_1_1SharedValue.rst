.. index:: pair: struct; SharedAttribute::SharedValueAttribute::SharedValue
.. _doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value:

struct SharedAttribute::SharedValueAttribute::SharedValue
=========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <shared_value_attribute.hpp>
	
	struct SharedValue: public std::enable_shared_from_this< SharedValue >
	{
		// fields
	
		T :ref:`value<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value_1abc98eb6b3b88cd998d258a634477f189>` = {};

		// construction
	
		:ref:`SharedValue<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value_1a6315b95368961133bcd465691e40e144>`();
		:ref:`SharedValue<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value_1a515e19cc45725d4594fc77d5ac19a8ea>`(const T& value);

		// methods
	
		void :ref:`addAttribute<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value_1a8fb72083f6ff5de9658484c870799caf>`(std::weak_ptr<:ref:`SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute>`> attribute);
		std::vector<std::weak_ptr<:ref:`SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute>`>>& :ref:`getAttributes<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value_1af0fb66b81d07dde5a203d73f6f54b538>`();
	};

