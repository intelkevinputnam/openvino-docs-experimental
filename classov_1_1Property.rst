.. index:: pair: class; ov::Property
.. _doxid-classov_1_1_property:

class ov::Property
==================

.. toctree::
	:hidden:

	Forward <structov_1_1Property_1_1Forward.rst>

Overview
~~~~~~~~

This class is used to bind property name with value type. :ref:`More...<details-classov_1_1_property>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>
	
	template <typename T, PropertyMutability mutability_ = PropertyMutability::RW>
	class Property: public util::BaseProperty< T, PropertyMutability::RW >
	{
	public:
		// structs
	
		template <typename V>
		struct :ref:`Forward<doxid-structov_1_1_property_1_1_forward>`;

		// methods
	
		template <typename... Args>
		std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`operator ()<doxid-classov_1_1_property_1ab75500bcce40786e0ac2b29570180456>` (Args&&... args) const;
	};

	// direct descendants

	struct :ref:`Priorities<doxid-structov_1_1device_1_1_priorities>`;
.. _details-classov_1_1_property:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is used to bind property name with value type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- type of value used to set or get property

Methods
-------

.. _doxid-classov_1_1_property_1ab75500bcce40786e0ac2b29570180456:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Args>
	std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> operator () (Args&&... args) const

Constructs property.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Args

		- property constructor arguments types

	*
		- args

		- property constructor arguments



.. rubric:: Returns:

Pair of name and type erased value.


