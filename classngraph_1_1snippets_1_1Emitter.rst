.. index:: pair: interface; ngraph::snippets::Emitter
.. _doxid-classngraph_1_1snippets_1_1_emitter:

interface ngraph::snippets::Emitter
===================================



Overview
~~~~~~~~

Base class for all target specific code emitters used by generator. :ref:`More...<details-classngraph_1_1snippets_1_1_emitter>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <emitter.hpp>
	
	template Emitter
	{
		// construction
	
		:ref:`Emitter<doxid-classngraph_1_1snippets_1_1_emitter_1ab202eee5db9d751b52bd9fd405178d4f>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& n);
		:target:`Emitter<doxid-classngraph_1_1snippets_1_1_emitter_1a1c96f16027d7eabaf84e500479819e59>`(std::vector<std::pair<std::shared_ptr<Emitter>, :ref:`RegInfo<doxid-namespacengraph_1_1snippets_1a3d2700d6955f8b1f9e2fffa540cd5556>`>>& region);

		// methods
	
		virtual void :ref:`emit_code<doxid-classngraph_1_1snippets_1_1_emitter_1af9b5c7145cebff6a84961e168818d034>`(
			const std::vector<size_t>& in,
			const std::vector<size_t>& out,
			const std::vector<size_t>& pool = {},
			const std::vector<size_t>& gpr = {}
			) const = 0;
	
		virtual void :ref:`emit_data<doxid-classngraph_1_1snippets_1_1_emitter_1a527554674f3f3cb59f33f440f68e2ec9>`() const;
	};
.. _details-classngraph_1_1snippets_1_1_emitter:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Base class for all target specific code emitters used by generator.

Construction
------------

.. _doxid-classngraph_1_1snippets_1_1_emitter_1ab202eee5db9d751b52bd9fd405178d4f:
.. index:: pair: function; Emitter

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Emitter(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& n)

Default constructor.

Methods
-------

.. _doxid-classngraph_1_1snippets_1_1_emitter_1af9b5c7145cebff6a84961e168818d034:
.. index:: pair: function; emit_code

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void emit_code(
		const std::vector<size_t>& in,
		const std::vector<size_t>& out,
		const std::vector<size_t>& pool = {},
		const std::vector<size_t>& gpr = {}
		) const = 0

called by generator to generate code to produce target code for a specific operation



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- in

		- vector of vector argument registers

	*
		- out

		- vector of vector resulting registers

	*
		- pool

		- optional vector of free vector registers which might be used inside method

	*
		- gpr

		- vector of free generam puproce registers which might be used inside method



.. rubric:: Returns:

void

.. _doxid-classngraph_1_1snippets_1_1_emitter_1a527554674f3f3cb59f33f440f68e2ec9:
.. index:: pair: function; emit_data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void emit_data() const

called by generator to generate data section, if needed for a specific operation



.. rubric:: Returns:

void


