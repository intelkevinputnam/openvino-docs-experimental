.. index:: pair: class; ov::VariableState
.. _doxid-classov_1_1_variable_state:

class ov::VariableState
=======================



Overview
~~~~~~~~

:ref:`VariableState <doxid-classov_1_1_variable_state>` class. :ref:`More...<details-classov_1_1_variable_state>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable_state.hpp>
	
	class VariableState
	{
	public:
		// methods
	
		void :ref:`reset<doxid-classov_1_1_variable_state_1abee0db4d1ee84f2ee38f47a3e022ceb5>`();
		std::string :ref:`get_name<doxid-classov_1_1_variable_state_1abade5aae9a6a276d2831d6bd5faebcc4>`() const;
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`get_state<doxid-classov_1_1_variable_state_1a3a76af4210c36260fa2d1dba01e9ea43>`() const;
		void :ref:`set_state<doxid-classov_1_1_variable_state_1a631eadeb3b03121675486e2b0ba1aef4>`(const :ref:`Tensor<doxid-classov_1_1_tensor>`& state);
	};
.. _details-classov_1_1_variable_state:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`VariableState <doxid-classov_1_1_variable_state>` class.

Methods
-------

.. _doxid-classov_1_1_variable_state_1abee0db4d1ee84f2ee38f47a3e022ceb5:
.. index:: pair: function; reset

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reset()

Resets internal variable state for relevant infer request to a value specified as default for the corresponding ReadValue node.

.. _doxid-classov_1_1_variable_state_1abade5aae9a6a276d2831d6bd5faebcc4:
.. index:: pair: function; get_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string get_name() const

Gets the name of the current variable state. If length of an array is not enough, the name is truncated by len, null terminator is inserted as well. ``variable_id`` from the corresponding ``ReadValue`` is used as variable state name.



.. rubric:: Returns:

A string representing state name.

.. _doxid-classov_1_1_variable_state_1a3a76af4210c36260fa2d1dba01e9ea43:
.. index:: pair: function; get_state

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` get_state() const

Returns the value of the variable state.



.. rubric:: Returns:

A tensor representing a state.

.. _doxid-classov_1_1_variable_state_1a631eadeb3b03121675486e2b0ba1aef4:
.. index:: pair: function; set_state

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_state(const :ref:`Tensor<doxid-classov_1_1_tensor>`& state)

Sets the new state for the next inference.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- state

		- The current state to set.


