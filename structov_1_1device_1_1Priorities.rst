.. index:: pair: struct; ov::device::Priorities
.. _doxid-structov_1_1device_1_1_priorities:

struct ov::device::Priorities
=============================



Overview
~~~~~~~~

Type for device :ref:`Priorities <doxid-structov_1_1device_1_1_priorities>` config option, with comma-separated devices listed in the desired priority. :ref:`More...<details-structov_1_1device_1_1_priorities>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>
	
	struct Priorities: public :ref:`ov::Property<doxid-classov_1_1_property>`
	{
		// methods
	
		template <typename... Args>
		std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`operator ()<doxid-structov_1_1device_1_1_priorities_1a558fac8c911e573eb73debf29b27ef86>` (Args&&... args) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// structs
	
		template <typename V>
		struct :ref:`Forward<doxid-structov_1_1_property_1_1_forward>`;

		// methods
	
		template <typename... Args>
		std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> :ref:`operator ()<doxid-classov_1_1_property_1ab75500bcce40786e0ac2b29570180456>` (Args&&... args) const;

.. _details-structov_1_1device_1_1_priorities:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Type for device :ref:`Priorities <doxid-structov_1_1device_1_1_priorities>` config option, with comma-separated devices listed in the desired priority.

Methods
-------

.. _doxid-structov_1_1device_1_1_priorities_1a558fac8c911e573eb73debf29b27ef86:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Args>
	std::pair<std::string, :ref:`Any<doxid-classov_1_1_any>`> operator () (Args&&... args) const

Constructs device priorities.



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


