.. index:: pair: interface; ngraph::snippets::Schedule
.. _doxid-classngraph_1_1snippets_1_1_schedule:

interface ngraph::snippets::Schedule
====================================



Overview
~~~~~~~~

Return scheduling information and pointer to generated kernel code. :ref:`More...<details-classngraph_1_1snippets_1_1_schedule>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <generator.hpp>
	
	template Schedule
	{
		// fields
	
		:ref:`Shape<doxid-classov_1_1_shape>` :target:`work_size<doxid-classngraph_1_1snippets_1_1_schedule_1a144b0132c92716d2efc9dc0d21a169f6>` {};
		bool :target:`is_flat<doxid-classngraph_1_1snippets_1_1_schedule_1abb2005b0660716f584f5503c9472d57c>` {false};
		:ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` :target:`ptr<doxid-classngraph_1_1snippets_1_1_schedule_1aeeb1787d03fa357594235eac4dc1a0d8>` {nullptr};

		// construction
	
		:ref:`Schedule<doxid-classngraph_1_1snippets_1_1_schedule_1a5b3c1d82e3ab9cbed291d02e7edf8d97>`();
		:ref:`Schedule<doxid-classngraph_1_1snippets_1_1_schedule_1ac3e6499d4c67ba7d2995b970065c3522>`(const :ref:`Shape<doxid-classov_1_1_shape>`& ws, bool f, :ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` p);

		// methods
	
		template <typename K>
		K :ref:`get_callable<doxid-classngraph_1_1snippets_1_1_schedule_1a778c3d8586ac85e833c2627a1b1e3e9b>`() const;
	};
.. _details-classngraph_1_1snippets_1_1_schedule:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Return scheduling information and pointer to generated kernel code.

Construction
------------

.. _doxid-classngraph_1_1snippets_1_1_schedule_1a5b3c1d82e3ab9cbed291d02e7edf8d97:
.. index:: pair: function; Schedule

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Schedule()

Default constructor.

.. _doxid-classngraph_1_1snippets_1_1_schedule_1ac3e6499d4c67ba7d2995b970065c3522:
.. index:: pair: function; Schedule

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Schedule(const :ref:`Shape<doxid-classov_1_1_shape>`& ws, bool f, :ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` p)

Default to create schedule out of specific parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ws

		- work size for kernel execution

	*
		- f

		- can this kernel be linearided to 1D range

	*
		- p

		- pointer to generated code

Methods
-------

.. _doxid-classngraph_1_1snippets_1_1_schedule_1a778c3d8586ac85e833c2627a1b1e3e9b:
.. index:: pair: function; get_callable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename K>
	K get_callable() const

Returns callable instanse of code pointer.


