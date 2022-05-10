.. index:: pair: class; ov::frontend::NodeContext
.. _doxid-classov_1_1frontend_1_1_node_context:

class ov::frontend::NodeContext
===============================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node_context.hpp>
	
	class NodeContext
	{
	public:
		// construction
	
		:target:`NodeContext<doxid-classov_1_1frontend_1_1_node_context_1a7c0e010c876dde798be5b932405df509>`(const std::string& op_type);

		// methods
	
		virtual size_t :ref:`get_input_size<doxid-classov_1_1frontend_1_1_node_context_1a7e8506b39e7692f90792a06ebebe8b3f>`() const;
		virtual size_t :ref:`get_input_size<doxid-classov_1_1frontend_1_1_node_context_1a536b381b846e2cfbe0af12b1999a99ab>`(const std::string& port_name) const;
		virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input<doxid-classov_1_1frontend_1_1_node_context_1aefd6066f0f721dee2e1cb68a41f8adfa>`(int idx) const;
		virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input<doxid-classov_1_1frontend_1_1_node_context_1a0a011d47b501132b0dc6f340c7b814aa>`(const std::string& name, int idx) const;
		virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_input<doxid-classov_1_1frontend_1_1_node_context_1aaa43d8f6917ae002a631e35a8e5eec72>`(const std::string& name) const;
		virtual const std::string& :target:`get_op_type<doxid-classov_1_1frontend_1_1_node_context_1a003b705dce8961eee0b7f5237fd2c2d4>`() const;
	
		template <class T>
		T :ref:`get_attribute<doxid-classov_1_1frontend_1_1_node_context_1addd9e05f2766e29c43594c84592ecc1b>`(const std::string& name) const;
	
		template <class T>
		T :ref:`get_attribute<doxid-classov_1_1frontend_1_1_node_context_1ad415eab29cac84e3f39cfce12688a319>`(const std::string& name, const T& def) const;
	
		bool :ref:`has_attribute<doxid-classov_1_1frontend_1_1_node_context_1ae428bf822068ad24dee7748862aa354a>`(const std::string& name) const;
		virtual :ref:`ov::Any<doxid-classov_1_1_any>` :ref:`get_attribute_as_any<doxid-classov_1_1frontend_1_1_node_context_1ae0826b4f1f4f43600798c3acc7b6edc1>`(const std::string& name) const = 0;
	};
.. _details-classov_1_1frontend_1_1_node_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1frontend_1_1_node_context_1a7e8506b39e7692f90792a06ebebe8b3f:
.. index:: pair: function; get_input_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_input_size() const

Returns a number of inputs.

.. _doxid-classov_1_1frontend_1_1_node_context_1a536b381b846e2cfbe0af12b1999a99ab:
.. index:: pair: function; get_input_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_input_size(const std::string& port_name) const

Returns a number of inputs.

.. _doxid-classov_1_1frontend_1_1_node_context_1aefd6066f0f721dee2e1cb68a41f8adfa:
.. index:: pair: function; get_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_input(int idx) const

Returns exactly one input with a given idx; throws if there is no inputs or there are more than one input.

.. _doxid-classov_1_1frontend_1_1_node_context_1a0a011d47b501132b0dc6f340c7b814aa:
.. index:: pair: function; get_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_input(const std::string& name, int idx) const

Returns exactly one input with a given name and idx; throws if there is no inputs or there are more than one input.

.. _doxid-classov_1_1frontend_1_1_node_context_1aaa43d8f6917ae002a631e35a8e5eec72:
.. index:: pair: function; get_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> get_input(const std::string& name) const

Returns exactly one input with a given name; throws if there is no inputs or there are more than one input.

.. _doxid-classov_1_1frontend_1_1_node_context_1addd9e05f2766e29c43594c84592ecc1b:
.. index:: pair: function; get_attribute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	T get_attribute(const std::string& name) const

Returns node attribute by name.

.. _doxid-classov_1_1frontend_1_1_node_context_1ad415eab29cac84e3f39cfce12688a319:
.. index:: pair: function; get_attribute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class T>
	T get_attribute(const std::string& name, const T& def) const

Returns node attribute by name. Returns 'def' value if attribute does not exist.

.. _doxid-classov_1_1frontend_1_1_node_context_1ae428bf822068ad24dee7748862aa354a:
.. index:: pair: function; has_attribute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has_attribute(const std::string& name) const

Check if an attribute of a given name exist.

.. _doxid-classov_1_1frontend_1_1_node_context_1ae0826b4f1f4f43600798c3acc7b6edc1:
.. index:: pair: function; get_attribute_as_any

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ov::Any<doxid-classov_1_1_any>` get_attribute_as_any(const std::string& name) const = 0

Returns node attribute by name as :ref:`ov::Any <doxid-classov_1_1_any>`.


