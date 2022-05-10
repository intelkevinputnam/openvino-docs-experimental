.. index:: pair: struct; ov::PropertyName
.. _doxid-structov_1_1_property_name:

struct ov::PropertyName
=======================



Overview
~~~~~~~~

This class is used to return property name and its mutability attribute. :ref:`More...<details-structov_1_1_property_name>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>
	
	struct PropertyName: public string
	{
		// construction
	
		:ref:`PropertyName<doxid-structov_1_1_property_name_1a30e3cb2d75135fc13a725913c6250232>`(
			const std::string& str,
			:ref:`PropertyMutability<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47>` mutability = :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`
			);

		// methods
	
		bool :ref:`is_mutable<doxid-structov_1_1_property_name_1a7c31d6356fad04394463ec5a3b9b4148>`() const;
	};
.. _details-structov_1_1_property_name:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is used to return property name and its mutability attribute.

Construction
------------

.. _doxid-structov_1_1_property_name_1a30e3cb2d75135fc13a725913c6250232:
.. index:: pair: function; PropertyName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PropertyName(
		const std::string& str,
		:ref:`PropertyMutability<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47>` mutability = :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`
		)

Constructs property name object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- str

		- property name

	*
		- mutability

		- property mutability

Methods
-------

.. _doxid-structov_1_1_property_name_1a7c31d6356fad04394463ec5a3b9b4148:
.. index:: pair: function; is_mutable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_mutable() const

check property mutability



.. rubric:: Returns:

true if property is mutable


