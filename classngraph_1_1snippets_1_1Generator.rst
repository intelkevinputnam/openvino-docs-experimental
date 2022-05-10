.. index:: pair: interface; ngraph::snippets::Generator
.. _doxid-classngraph_1_1snippets_1_1_generator:

interface ngraph::snippets::Generator
=====================================



Overview
~~~~~~~~

Target independent code generator interface. :ref:`More...<details-classngraph_1_1snippets_1_1_generator>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <generator.hpp>
	
	template Generator
	{
		// construction
	
		:ref:`Generator<doxid-classngraph_1_1snippets_1_1_generator_1a3a954b9078ce00b1b4b75b41113204e8>`(const std::shared_ptr<:ref:`TargetMachine<doxid-classngraph_1_1snippets_1_1_target_machine>`>& t);

		// methods
	
		:ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` :ref:`generate<doxid-classngraph_1_1snippets_1_1_generator_1ab1074eabb84a137b272641f467f348b6>`(
			std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m,
			const void \* compile_params = nullptr
			) const;
	};
.. _details-classngraph_1_1snippets_1_1_generator:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Target independent code generator interface.

Construction
------------

.. _doxid-classngraph_1_1snippets_1_1_generator_1a3a954b9078ce00b1b4b75b41113204e8:
.. index:: pair: function; Generator

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Generator(const std::shared_ptr<:ref:`TargetMachine<doxid-classngraph_1_1snippets_1_1_target_machine>`>& t)

Default constructor.

Methods
-------

.. _doxid-classngraph_1_1snippets_1_1_generator_1ab1074eabb84a137b272641f467f348b6:
.. index:: pair: function; generate

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` generate(
		std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m,
		const void \* compile_params = nullptr
		) const

virtual method any specific implementation should implement



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- m

		- model in canonical for for table-based code generation



.. rubric:: Returns:

pointer to generated code


