.. index:: pair: class; ov::op::util::VariableValue
.. _doxid-classov_1_1op_1_1util_1_1_variable_value:

class ov::op::util::VariableValue
=================================



Overview
~~~~~~~~

:ref:`VariableValue <doxid-classov_1_1op_1_1util_1_1_variable_value>` stores data and state (reset flag) for a :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`, and provides an interface for changing them. :ref:`More...<details-classov_1_1op_1_1util_1_1_variable_value>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable_value.hpp>
	
	class VariableValue
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<VariableValue> :target:`Ptr<doxid-classov_1_1op_1_1util_1_1_variable_value_1ac02453613047e3fc37b568870c7fb643>`;

		// construction
	
		:ref:`VariableValue<doxid-classov_1_1op_1_1util_1_1_variable_value_1af91f2a3761813ba466c8e07d47c61249>`();
		:ref:`VariableValue<doxid-classov_1_1op_1_1util_1_1_variable_value_1a4dba6f52968b5bc8e85bedf2d96aef5f>`(:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` value);
		:ref:`VariableValue<doxid-classov_1_1op_1_1util_1_1_variable_value_1ad1ba5ed5a6e1ca04c4bcc7111e7d93c0>`(:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` value, bool reset);

		// methods
	
		void :ref:`set_reset<doxid-classov_1_1op_1_1util_1_1_variable_value_1a3199b939ec047a9d78a7378cab448c82>`(bool reset);
		bool :ref:`get_reset<doxid-classov_1_1op_1_1util_1_1_variable_value_1aa712bfe37b0553573128c40c90ee14fd>`() const;
		const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& :ref:`get_value<doxid-classov_1_1op_1_1util_1_1_variable_value_1ad2d499c5cd4483bbc7b0531b0162918f>`() const;
		void :ref:`set_value<doxid-classov_1_1op_1_1util_1_1_variable_value_1a0c74e073b3d48b4adc328a035b8450e3>`(const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& value);
	};
.. _details-classov_1_1op_1_1util_1_1_variable_value:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`VariableValue <doxid-classov_1_1op_1_1util_1_1_variable_value>` stores data and state (reset flag) for a :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`, and provides an interface for changing them.

Construction
------------

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1af91f2a3761813ba466c8e07d47c61249:
.. index:: pair: function; VariableValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableValue()

Constructs an uninitialized :ref:`VariableValue <doxid-classov_1_1op_1_1util_1_1_variable_value>`.

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1a4dba6f52968b5bc8e85bedf2d96aef5f:
.. index:: pair: function; VariableValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableValue(:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` value)

Constructor for :ref:`VariableValue <doxid-classov_1_1op_1_1util_1_1_variable_value>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The data for :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1ad1ba5ed5a6e1ca04c4bcc7111e7d93c0:
.. index:: pair: function; VariableValue

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariableValue(:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` value, bool reset)

Constructor for :ref:`VariableValue <doxid-classov_1_1op_1_1util_1_1_variable_value>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- Data for :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.

	*
		- reset

		- The current state of the reset flag.

Methods
-------

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1a3199b939ec047a9d78a7378cab448c82:
.. index:: pair: function; set_reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_reset(bool reset)

Sets the reset flag to a new state.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- reset

		- The new state of the reset flag.

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1aa712bfe37b0553573128c40c90ee14fd:
.. index:: pair: function; get_reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_reset() const

Returns the current reset flag state.

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1ad2d499c5cd4483bbc7b0531b0162918f:
.. index:: pair: function; get_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& get_value() const

Returns the current stored data.

.. _doxid-classov_1_1op_1_1util_1_1_variable_value_1a0c74e073b3d48b4adc328a035b8450e3:
.. index:: pair: function; set_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_value(const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& value)

Sets new values for :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- New data for :ref:`Variable <doxid-classov_1_1op_1_1util_1_1_variable>`.


