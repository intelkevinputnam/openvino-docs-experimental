.. index:: pair: struct; ov::Property<T, PropertyMutability::RO>
.. _doxid-structov_1_1_property_3_01_t_00_01_property_mutability_1_1_r_o_01_4:

struct ov::Property<T, PropertyMutability::RO>
==============================================



Overview
~~~~~~~~

This class is used to bind read-only property name with value type. :ref:`More...<details-structov_1_1_property_3_01_t_00_01_property_mutability_1_1_r_o_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>
	
	template <typename T>
	struct Property<T, PropertyMutability::RO>: public util::BaseProperty< T, PropertyMutability::RO >
	{
	};
.. _details-structov_1_1_property_3_01_t_00_01_property_mutability_1_1_r_o_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is used to bind read-only property name with value type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type of value used to pass or get property


