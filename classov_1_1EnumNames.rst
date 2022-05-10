.. index:: pair: class; ov::EnumNames
.. _doxid-classov_1_1_enum_names:

class ov::EnumNames
===================



Overview
~~~~~~~~

Uses a pairings defined by EnumTypes::get() to convert between strings and enum values. :ref:`More...<details-classov_1_1_enum_names>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <enum_names.hpp>
	
	template <typename EnumType>
	class EnumNames
	{
	public:
		// methods
	
		static EnumType :ref:`as_enum<doxid-classov_1_1_enum_names_1a6a7b5955bb7653a8e6aae078d98dddee>`(const std::string& name);
		static const std::string& :ref:`as_string<doxid-classov_1_1_enum_names_1a2bd546012ae3994fb23a8fcbb2101225>`(EnumType e);
	};
.. _details-classov_1_1_enum_names:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Uses a pairings defined by EnumTypes::get() to convert between strings and enum values.

Methods
-------

.. _doxid-classov_1_1_enum_names_1a6a7b5955bb7653a8e6aae078d98dddee:
.. index:: pair: function; as_enum

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static EnumType as_enum(const std::string& name)

Converts strings to enum values.

.. _doxid-classov_1_1_enum_names_1a2bd546012ae3994fb23a8fcbb2101225:
.. index:: pair: function; as_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static const std::string& as_string(EnumType e)

Converts enum values to strings.


