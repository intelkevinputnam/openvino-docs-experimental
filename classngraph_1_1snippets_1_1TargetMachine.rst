.. index:: pair: interface; ngraph::snippets::TargetMachine
.. _doxid-classngraph_1_1snippets_1_1_target_machine:

interface ngraph::snippets::TargetMachine
=========================================



Overview
~~~~~~~~

Base class Target machine representation. Target derives from this class to provide generator information about supported emittors. :ref:`More...<details-classngraph_1_1snippets_1_1_target_machine>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <generator.hpp>
	
	template TargetMachine
	{
		// methods
	
		virtual bool :ref:`is_supported<doxid-classngraph_1_1snippets_1_1_target_machine_1a9483ad2a5db444185d603237bad1d235>`() const = 0;
		virtual :ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` :ref:`get_snippet<doxid-classngraph_1_1snippets_1_1_target_machine_1a222066dbd662435972850f739f7ea385>`() const = 0;
		virtual size_t :ref:`get_lanes<doxid-classngraph_1_1snippets_1_1_target_machine_1abf9a391d2f3aa6f1fed48ae0af33b688>`() const = 0;
		std::function<std::shared_ptr<:ref:`Emitter<doxid-classngraph_1_1snippets_1_1_emitter>`>std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>)> :ref:`get<doxid-classngraph_1_1snippets_1_1_target_machine_1a738dd573cddd713f4b8b245d598072e0>`(const :ref:`ngraph::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` type) const;
		bool :ref:`has<doxid-classngraph_1_1snippets_1_1_target_machine_1a6e0d14fd84742d193b46b72d618b593f>`(const :ref:`ngraph::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` type) const;
	};
.. _details-classngraph_1_1snippets_1_1_target_machine:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Base class Target machine representation. Target derives from this class to provide generator information about supported emittors.

Methods
-------

.. _doxid-classngraph_1_1snippets_1_1_target_machine_1a9483ad2a5db444185d603237bad1d235:
.. index:: pair: function; is_supported

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_supported() const = 0

checks if target is natively supported



.. rubric:: Returns:

true, if supported

.. _doxid-classngraph_1_1snippets_1_1_target_machine_1a222066dbd662435972850f739f7ea385:
.. index:: pair: function; get_snippet

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`code<doxid-namespacengraph_1_1snippets_1ac4f44bdec6f42fb835362020d78b6aab>` get_snippet() const = 0

finalizes code generation



.. rubric:: Returns:

generated kernel binary

.. _doxid-classngraph_1_1snippets_1_1_target_machine_1abf9a391d2f3aa6f1fed48ae0af33b688:
.. index:: pair: function; get_lanes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_lanes() const = 0

gets number of lanes supported by target's vector ISA



.. rubric:: Returns:

number of lanes

.. _doxid-classngraph_1_1snippets_1_1_target_machine_1a738dd573cddd713f4b8b245d598072e0:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::function<std::shared_ptr<:ref:`Emitter<doxid-classngraph_1_1snippets_1_1_emitter>`>std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>)> get(const :ref:`ngraph::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` type) const

called by generator to all the emittor for a target machine



.. rubric:: Returns:

a map by node's type info with callbacks to create an instance of emmitter for corresponding operation type

.. _doxid-classngraph_1_1snippets_1_1_target_machine_1a6e0d14fd84742d193b46b72d618b593f:
.. index:: pair: function; has

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has(const :ref:`ngraph::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` type) const

checks if emitter for a specific operation is supported



.. rubric:: Returns:

true, if supported


