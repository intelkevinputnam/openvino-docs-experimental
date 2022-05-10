.. index:: pair: class; ov::op::util::VariableExtension
.. _doxid-classov_1_1op_1_1util_1_1_variable_extension:

class ov::op::util::VariableExtension
=====================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <variable_extension.hpp>
	
	class VariableExtension
	{
	public:
		// methods
	
		virtual std::shared_ptr<:ref:`Variable<doxid-classov_1_1op_1_1util_1_1_variable>`> :ref:`get_variable<doxid-classov_1_1op_1_1util_1_1_variable_extension_1afb31eee58abe64d67a23da38e637a40c>`() const;
		virtual void :ref:`set_variable<doxid-classov_1_1op_1_1util_1_1_variable_extension_1ae1b303e2ba2cc97d91e9f0948c14aaf9>`(const std::shared_ptr<:ref:`Variable<doxid-classov_1_1op_1_1util_1_1_variable>`>& variable);
		virtual void :ref:`set_variable_id<doxid-classov_1_1op_1_1util_1_1_variable_extension_1a8a0ce485b3557c04c6b9bbfd6b25869e>`(const std::string& variable_id);
		virtual std::string :ref:`get_variable_id<doxid-classov_1_1op_1_1util_1_1_variable_extension_1a29af3ea10980289b15b9bdfb705023b5>`() const = 0;

	protected:
	};

	// direct descendants

	class :ref:`AssignBase<doxid-classov_1_1op_1_1util_1_1_assign_base>`;
	class :ref:`ReadValueBase<doxid-classov_1_1op_1_1util_1_1_read_value_base>`;
.. _details-classov_1_1op_1_1util_1_1_variable_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1op_1_1util_1_1_variable_extension_1afb31eee58abe64d67a23da38e637a40c:
.. index:: pair: function; get_variable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`Variable<doxid-classov_1_1op_1_1util_1_1_variable>`> get_variable() const

Returns variable connected to this node.

.. _doxid-classov_1_1op_1_1util_1_1_variable_extension_1ae1b303e2ba2cc97d91e9f0948c14aaf9:
.. index:: pair: function; set_variable

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_variable(const std::shared_ptr<:ref:`Variable<doxid-classov_1_1op_1_1util_1_1_variable>`>& variable)

Sets a new variable to be connected to this node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable

		- New variable to be connected to this node.

.. _doxid-classov_1_1op_1_1util_1_1_variable_extension_1a8a0ce485b3557c04c6b9bbfd6b25869e:
.. index:: pair: function; set_variable_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_variable_id(const std::string& variable_id)

Sets the identifier to a variable.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- variable_id

		- New identifier of the variable.

.. _doxid-classov_1_1op_1_1util_1_1_variable_extension_1a29af3ea10980289b15b9bdfb705023b5:
.. index:: pair: function; get_variable_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string get_variable_id() const = 0

Returns the identifier of corresponding variable.


