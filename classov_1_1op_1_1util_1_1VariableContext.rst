.. index:: pair: class; ov::op::util::VariableContext
.. _doxid-classov_1_1op_1_1util_1_1_variable_context:

class ov::op::util::VariableContext
===================================



Overview
~~~~~~~~

:ref:`VariableContext <doxid-classov_1_1op_1_1util_1_1_variable_context>` stores and manages a evaluation context for Variables. :ref:`More...<details-classov_1_1op_1_1util_1_1_variable_context>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable_context.hpp>
	
	class VariableContext
	{
	public:
		// construction
	
		:ref:`VariableContext<doxid-classov_1_1op_1_1util_1_1_variable_context_1a68062b5395eb7500a695f3972210c670>`();
		:ref:`VariableContext<doxid-classov_1_1op_1_1util_1_1_variable_context_1aed4fae0f0874d32be3e5d6b718ee8a3d>`(const :ref:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`& variable_values);

		// methods
	
		void :ref:`reset_variable_context<doxid-classov_1_1op_1_1util_1_1_variable_context_1abc5504690228bf9078846eb7d9377147>`() const;
		void :ref:`set_variable_values<doxid-classov_1_1op_1_1util_1_1_variable_context_1abb3a4c89811d4e457436b3cb07533948>`(const :ref:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`& variable_values);
	
		void :ref:`set_variable_value<doxid-classov_1_1op_1_1util_1_1_variable_context_1a4410c51290a3c67cdcd49e9ea2c7c575>`(
			const :ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable,
			const :ref:`VariableValue::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_value_1ac02453613047e3fc37b568870c7fb643>`& variable_value
			);
	
		void :ref:`remove_variable_value<doxid-classov_1_1op_1_1util_1_1_variable_context_1ac4cb03be01e90e12ab81a7420dc79242>`(const :ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable);
		const :ref:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`& :ref:`get_variable_values<doxid-classov_1_1op_1_1util_1_1_variable_context_1aab32e5e38ebe401b3cda7010973f6190>`() const;
		:ref:`VariableValue::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_value_1ac02453613047e3fc37b568870c7fb643>` :ref:`get_variable_value<doxid-classov_1_1op_1_1util_1_1_variable_context_1af4fb5f52f274929b2b96be4aa6e47db1>`(const :ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable) const;
	};
.. _details-classov_1_1op_1_1util_1_1_variable_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`VariableContext <doxid-classov_1_1op_1_1util_1_1_variable_context>` stores and manages a evaluation context for Variables.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1a68062b5395eb7500a695f3972210c670:
.. index:: pair: function; VariableContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableContext()

Constructs an uninitialized :ref:`VariableContext <doxid-classov_1_1op_1_1util_1_1_variable_context>`.

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1aed4fae0f0874d32be3e5d6b718ee8a3d:
.. index:: pair: function; VariableContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableContext(const :ref:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`& variable_values)

Constructor for :ref:`VariableContext <doxid-classov_1_1op_1_1util_1_1_variable_context>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable_values

		- The values associated with a particular Variables.

Methods
-------

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1abc5504690228bf9078846eb7d9377147:
.. index:: pair: function; reset_variable_context

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reset_variable_context() const

Sets the reset flags for all stored Variables to true.

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1abb3a4c89811d4e457436b3cb07533948:
.. index:: pair: function; set_variable_values

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_variable_values(const :ref:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`& variable_values)

Sets the new values for Variables.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable_values

		- The new values associated with a particular :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1a4410c51290a3c67cdcd49e9ea2c7c575:
.. index:: pair: function; set_variable_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_variable_value(
		const :ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable,
		const :ref:`VariableValue::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_value_1ac02453613047e3fc37b568870c7fb643>`& variable_value
		)

Changes/sets the values for :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable

		- New or stored :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.

	*
		- variable_value

		- The values associated with the variable.

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1ac4cb03be01e90e12ab81a7420dc79242:
.. index:: pair: function; remove_variable_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_variable_value(const :ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable)

Removes context for a particular :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable

		- The variable for which the context will be cleared.

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1aab32e5e38ebe401b3cda7010973f6190:
.. index:: pair: function; get_variable_values

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`VariableMap<doxid-namespaceov_1_1op_1_1util_1af459b4ae159647388079bd645f96324d>`& get_variable_values() const

Returns the current values for Variables.

.. _doxid-classov_1_1op_1_1util_1_1_variable_context_1af4fb5f52f274929b2b96be4aa6e47db1:
.. index:: pair: function; get_variable_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`VariableValue::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_value_1ac02453613047e3fc37b568870c7fb643>` get_variable_value(const :ref:`Variable::Ptr<doxid-classov_1_1op_1_1util_1_1_variable_1ace82a8f044f3aacd282630aca8bff198>`& variable) const

Returns the value for specified :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.


