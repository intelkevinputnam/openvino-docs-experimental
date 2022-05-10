.. index:: pair: struct; ov::device::Properties
.. _doxid-structov_1_1device_1_1_properties:

struct ov::device::Properties
=============================



Overview
~~~~~~~~

Type for property to pass set of properties to specified device. :ref:`More...<details-structov_1_1device_1_1_properties>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>
	
	struct Properties
	{
		// methods
	
		std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`operator ()<doxid-structov_1_1device_1_1_properties_1a578868d9cb202ca5c75293d7d6ee3ca0>` (
			const std::string& device_name,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& config
			) const;
	
		template <typename... Properties>
		util::EnableIfAllStringAny<std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`>, Properties...> :ref:`operator ()<doxid-structov_1_1device_1_1_properties_1a83b0c09b5c62b327c4ea16273ef32aa9>` (
			const std::string& device_name,
			Properties&&... configs
			) const;
	};
.. _details-structov_1_1device_1_1_properties:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Type for property to pass set of properties to specified device.

Methods
-------

.. _doxid-structov_1_1device_1_1_properties_1a578868d9cb202ca5c75293d7d6ee3ca0:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> operator () (
		const std::string& device_name,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& config
		) const

Constructs property.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- device_name

		- device plugin alias

	*
		- config

		- set of property values with names



.. rubric:: Returns:

Pair of string key representation and type erased property value.

.. _doxid-structov_1_1device_1_1_properties_1a83b0c09b5c62b327c4ea16273ef32aa9:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Properties>
	util::EnableIfAllStringAny<std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`>, Properties...> operator () (
		const std::string& device_name,
		Properties&&... configs
		) const

Constructs property.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`Properties <doxid-structov_1_1device_1_1_properties>`

		- Should be the pack of ``std::pair<std::string, :ref:`ov::Any <doxid-classov_1_1_any>`>`` types

	*
		- device_name

		- device plugin alias

	*
		- configs

		- Optional pack of pairs: (config parameter name, config parameter value)



.. rubric:: Returns:

Pair of string key representation and type erased property value.


