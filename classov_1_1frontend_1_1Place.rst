.. index:: pair: class; ov::frontend::Place
.. _doxid-classov_1_1frontend_1_1_place:

class ov::frontend::Place
=========================



Overview
~~~~~~~~

An interface for identifying a place in a graph and iterate over it; can refer to an operation node, tensor, port etc. :ref:`More...<details-classov_1_1frontend_1_1_place>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <place.hpp>
	
	class Place
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Place> :target:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`;

		// methods
	
		virtual std::vector<std::string> :ref:`get_names<doxid-classov_1_1frontend_1_1_place_1af15de9d881e42a152c62d194ca903052>`() const;
		virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_consuming_operations<doxid-classov_1_1frontend_1_1_place_1a4882d1705baa6abbe8648b5a0f643f0f>`() const;
		virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_consuming_operations<doxid-classov_1_1frontend_1_1_place_1a4f9e373109a52f451af59b33ff16426f>`(int output_port_index) const;
		virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_consuming_operations<doxid-classov_1_1frontend_1_1_place_1ab975cf1c622637ab68d1d9c910921a69>`(const std::string& outputName) const;
	
		virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_consuming_operations<doxid-classov_1_1frontend_1_1_place_1a9f7d409d4817abcf41e361e3f2332a82>`(
			const std::string& outputName,
			int outputPortIndex
			) const;
	
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_target_tensor<doxid-classov_1_1frontend_1_1_place_1a53965514f5e7650f79e8c7c1c4bbbe3a>`() const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_target_tensor<doxid-classov_1_1frontend_1_1_place_1afd07eaee02b8ac473ee8d9d6ff02d48d>`(const std::string& outputName) const;
	
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_target_tensor<doxid-classov_1_1frontend_1_1_place_1adb14c36fdaf1e916442cae7db1998a3c>`(
			const std::string& outputName,
			int outputPortIndex
			) const;
	
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_target_tensor<doxid-classov_1_1frontend_1_1_place_1ade5dc4b04dfbae530097c14b9c30a2c5>`(int output_port_index) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_source_tensor<doxid-classov_1_1frontend_1_1_place_1adc63238f31c5a4e006a96d2f714c7c7a>`() const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_source_tensor<doxid-classov_1_1frontend_1_1_place_1acf16452630832ab855e0497aeeb6b343>`(int input_port_index) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_source_tensor<doxid-classov_1_1frontend_1_1_place_1a58420fc481af321e68d8b3c0fe1fd42d>`(const std::string& inputName) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_source_tensor<doxid-classov_1_1frontend_1_1_place_1a98ed2e8b474e9a622f136bfd6c27aeec>`(const std::string& inputName, int inputPortIndex) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_producing_operation<doxid-classov_1_1frontend_1_1_place_1a4991d99534564bac20e3db307c710f91>`() const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_producing_operation<doxid-classov_1_1frontend_1_1_place_1a94d58e21f89a4442e09c8c139c638f00>`(int input_port_index) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_producing_operation<doxid-classov_1_1frontend_1_1_place_1aacd4065ea2971b0d8078e3c602e3aa5b>`(const std::string& inputName) const;
	
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_producing_operation<doxid-classov_1_1frontend_1_1_place_1a3ed17f1255e048ac910a1ce889217990>`(
			const std::string& inputName,
			int inputPortIndex
			) const;
	
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_producing_port<doxid-classov_1_1frontend_1_1_place_1ac79f28f016b100ca2a0079349e751ff5>`() const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_input_port<doxid-classov_1_1frontend_1_1_place_1aed81a43b7a4f1db5ae9e42f5ce7c053e>`() const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_input_port<doxid-classov_1_1frontend_1_1_place_1a5ab961f8b319e21e596d957ee2ff6cb0>`(int input_port_index) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_input_port<doxid-classov_1_1frontend_1_1_place_1a913674bd24ba713113d91b16c45aa3ba>`(const std::string& input_name) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_input_port<doxid-classov_1_1frontend_1_1_place_1a1901f11ec350ff05e6e54d625ad48ad8>`(const std::string& input_name, int input_port_index) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_output_port<doxid-classov_1_1frontend_1_1_place_1a3cd154f9642c6aee6dd253a20a12007d>`() const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_output_port<doxid-classov_1_1frontend_1_1_place_1a435c107c39adbefb0c9fe79a54ac317d>`(int output_port_index) const;
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_output_port<doxid-classov_1_1frontend_1_1_place_1af769196021551e75af17c0eae8df5cca>`(const std::string& output_name) const;
	
		virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` :ref:`get_output_port<doxid-classov_1_1frontend_1_1_place_1a86b7306a6f620d4d5388f0f07b357504>`(
			const std::string& output_name,
			int output_port_index
			) const;
	
		virtual std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> :ref:`get_consuming_ports<doxid-classov_1_1frontend_1_1_place_1af7bb27d15bb36859435c225820088eb4>`() const;
		virtual bool :ref:`is_input<doxid-classov_1_1frontend_1_1_place_1a25b0b484093cdc13a007d36599768124>`() const;
		virtual bool :ref:`is_output<doxid-classov_1_1frontend_1_1_place_1a55838cb299a83a6c1275bb8a4d42ec5c>`() const;
		virtual bool :ref:`is_equal<doxid-classov_1_1frontend_1_1_place_1aecfaab756f47e369d89b33983c4c176b>`(const :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& another) const;
		virtual bool :ref:`is_equal_data<doxid-classov_1_1frontend_1_1_place_1aa4a4bc7f418906c41f66fd3d2774bc36>`(const :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& another) const;
	};
.. _details-classov_1_1frontend_1_1_place:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An interface for identifying a place in a graph and iterate over it; can refer to an operation node, tensor, port etc.

Each front end implementation provides specialization of this interface to represent a place in a model graph. Various methods in the front end classes accept and retrieve instances of :ref:`Place <doxid-classov_1_1frontend_1_1_place>` to point to particular node part which should be modified or satisfies some criteria. For example, this class is used to report model inputs and outputs, for searching operations and tensors by name, for setting shape etc.

:ref:`Place <doxid-classov_1_1frontend_1_1_place>` can refer to :ref:`Tensor <doxid-classov_1_1_tensor>`, :ref:`Input <doxid-classov_1_1_input>` Edge, :ref:`Input <doxid-classov_1_1_input>` Port, Operation, :ref:`Output <doxid-classov_1_1_output>` Port, :ref:`Output <doxid-classov_1_1_output>` Edge

.. code-block:: cpp

	     [Tensor A]
	         |
	         | [Input Edge]
	         |
	         V
	-------------------
	[  [Input Port 0] ]
	[                 ]
	[   Operation A   ]
	[                 ]
	[ [Output Port 0] ]
	-------------------
	         |
	         | [Output Edge]
	         |
	         V
	     [Tensor B]
	         |
	         | [Input Edge]
	         |
	         V
	-------------------
	[  [Input Port 0] ]
	[                 ]
	[   Operation B   ]
	[                 ]
	[ [Output Port 0] ]
	-------------------
	         |
	         | [Output Edge]
	         |
	         V
	     [Tensor C]

Methods
-------

.. _doxid-classov_1_1frontend_1_1_place_1af15de9d881e42a152c62d194ca903052:
.. index:: pair: function; get_names

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::string> get_names() const

All associated names (synonyms) that identify this place in the graph in a framework specific way.



.. rubric:: Returns:

A vector of strings each representing a name that identifies this place in the graph. Can be empty if there are no names associated with this place or name cannot be attached.

.. _doxid-classov_1_1frontend_1_1_place_1a4882d1705baa6abbe8648b5a0f643f0f:
.. index:: pair: function; get_consuming_operations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_consuming_operations() const

Returns references to all operation nodes that consume data from this place.

It can be called for any kind of graph place searching for the first consuming operations. It is optional if place has only one output port



.. rubric:: Returns:

A vector with all operation node references that consumes data from this place

.. _doxid-classov_1_1frontend_1_1_place_1a4f9e373109a52f451af59b33ff16426f:
.. index:: pair: function; get_consuming_operations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_consuming_operations(int output_port_index) const

Returns references to all operation nodes that consume data from this place for specified output port.

It can be called for any kind of graph place searching for the first consuming operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_port_index

		- If place is an operational node it specifies which output port should be considered.



.. rubric:: Returns:

A vector with all operation node references that consumes data from this place

.. _doxid-classov_1_1frontend_1_1_place_1ab975cf1c622637ab68d1d9c910921a69:
.. index:: pair: function; get_consuming_operations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_consuming_operations(const std::string& outputName) const

Returns references to all operation nodes that consume data from this place for specified output port.

It can be called for any kind of graph place searching for the first consuming operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outputName

		- If a given place is itself an operation node, this specifies name of output port group



.. rubric:: Returns:

A vector with all operation node references that consumes data from this place

.. _doxid-classov_1_1frontend_1_1_place_1a9f7d409d4817abcf41e361e3f2332a82:
.. index:: pair: function; get_consuming_operations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_consuming_operations(
		const std::string& outputName,
		int outputPortIndex
		) const

Returns references to all operation nodes that consume data from this place for specified output port.

It can be called for any kind of graph place searching for the first consuming operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outputName

		- If a given place is itself an operation node, this specifies name of output port group, each group can have multiple ports

	*
		- outputPortIndex

		- If place is an operational node it specifies which output port should be considered.



.. rubric:: Returns:

A vector with all operation node references that consumes data from this place

.. _doxid-classov_1_1frontend_1_1_place_1a53965514f5e7650f79e8c7c1c4bbbe3a:
.. index:: pair: function; get_target_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_target_tensor() const

Returns a tensor place that gets data from this place; applicable for operations, output ports and output edges which have only one output port.



.. rubric:: Returns:

A tensor place which hold the resulting value for this place

.. _doxid-classov_1_1frontend_1_1_place_1afd07eaee02b8ac473ee8d9d6ff02d48d:
.. index:: pair: function; get_target_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_target_tensor(const std::string& outputName) const

Returns a tensor place that gets data from this place; applicable for operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outputName

		- Name of output port group



.. rubric:: Returns:

A tensor place which hold the resulting value for this place

.. _doxid-classov_1_1frontend_1_1_place_1adb14c36fdaf1e916442cae7db1998a3c:
.. index:: pair: function; get_target_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_target_tensor(
		const std::string& outputName,
		int outputPortIndex
		) const

Returns a tensor place that gets data from this place; applicable for operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outputName

		- Name of output port group, each group can have multiple ports

	*
		- outputPortIndex

		- :ref:`Output <doxid-classov_1_1_output>` port index if the current place is an operation node and has multiple output ports



.. rubric:: Returns:

A tensor place which hold the resulting value for this place

.. _doxid-classov_1_1frontend_1_1_place_1ade5dc4b04dfbae530097c14b9c30a2c5:
.. index:: pair: function; get_target_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_target_tensor(int output_port_index) const

Returns a tensor place that gets data from this place; applicable for operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_port_index

		- :ref:`Output <doxid-classov_1_1_output>` port index if the current place is an operation node and has multiple output ports



.. rubric:: Returns:

A tensor place which hold the resulting value for this place

.. _doxid-classov_1_1frontend_1_1_place_1adc63238f31c5a4e006a96d2f714c7c7a:
.. index:: pair: function; get_source_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_source_tensor() const

Returns a tensor place that supplies data for this place; applicable for operations, input ports and input edges which have only one input port.



.. rubric:: Returns:

A tensor place which supplies data for this place

.. _doxid-classov_1_1frontend_1_1_place_1acf16452630832ab855e0497aeeb6b343:
.. index:: pair: function; get_source_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_source_tensor(int input_port_index) const

Returns a tensor place that supplies data for this place; applicable for operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_port_index

		- :ref:`Input <doxid-classov_1_1_input>` port index for operational nodes.



.. rubric:: Returns:

A tensor place which supplies data for this place

.. _doxid-classov_1_1frontend_1_1_place_1a58420fc481af321e68d8b3c0fe1fd42d:
.. index:: pair: function; get_source_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_source_tensor(const std::string& inputName) const

Returns a tensor place that supplies data for this place; applicable for operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputName

		- Name of input port group



.. rubric:: Returns:

A tensor place which supplies data for this place

.. _doxid-classov_1_1frontend_1_1_place_1a98ed2e8b474e9a622f136bfd6c27aeec:
.. index:: pair: function; get_source_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_source_tensor(const std::string& inputName, int inputPortIndex) const

Returns a tensor place that supplies data for this place; applicable for operations.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputName

		- If a given place is itself an operation node, this specifies name of output port group, each group can have multiple ports

	*
		- inputPortIndex

		- :ref:`Input <doxid-classov_1_1_input>` port index for operational nodes.



.. rubric:: Returns:

A tensor place which supplies data for this place

.. _doxid-classov_1_1frontend_1_1_place_1a4991d99534564bac20e3db307c710f91:
.. index:: pair: function; get_producing_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_producing_operation() const

Get an operation node place that immediately produces data for this place; applicable if place has only one input port.



.. rubric:: Returns:

An operation place that produces data for this place

.. _doxid-classov_1_1frontend_1_1_place_1a94d58e21f89a4442e09c8c139c638f00:
.. index:: pair: function; get_producing_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_producing_operation(int input_port_index) const

Get an operation node place that immediately produces data for this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_port_index

		- If a given place is itself an operation node, this specifies a port index



.. rubric:: Returns:

An operation place that produces data for this place

.. _doxid-classov_1_1frontend_1_1_place_1aacd4065ea2971b0d8078e3c602e3aa5b:
.. index:: pair: function; get_producing_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_producing_operation(const std::string& inputName) const

Get an operation node place that immediately produces data for this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputName

		- If a given place is itself an operation node, this specifies name of output port group



.. rubric:: Returns:

An operation place that produces data for this place

.. _doxid-classov_1_1frontend_1_1_place_1a3ed17f1255e048ac910a1ce889217990:
.. index:: pair: function; get_producing_operation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_producing_operation(
		const std::string& inputName,
		int inputPortIndex
		) const

Get an operation node place that immediately produces data for this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputName

		- If a given place is itself an operation node, this specifies name of output port group, each group can have multiple ports

	*
		- inputPortIndex

		- If a given place is itself an operation node, this specifies a port index



.. rubric:: Returns:

An operation place that produces data for this place

.. _doxid-classov_1_1frontend_1_1_place_1ac79f28f016b100ca2a0079349e751ff5:
.. index:: pair: function; get_producing_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_producing_port() const

Returns a port that produces data for this place.

.. _doxid-classov_1_1frontend_1_1_place_1aed81a43b7a4f1db5ae9e42f5ce7c053e:
.. index:: pair: function; get_input_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_input_port() const

For operation node returns reference to an input port; applicable if operation node has only one input port.



.. rubric:: Returns:

:ref:`Input <doxid-classov_1_1_input>` port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1a5ab961f8b319e21e596d957ee2ff6cb0:
.. index:: pair: function; get_input_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_input_port(int input_port_index) const

For operation node returns reference to an input port with specified index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_port_index

		- :ref:`Input <doxid-classov_1_1_input>` port index



.. rubric:: Returns:

Appropriate input port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1a913674bd24ba713113d91b16c45aa3ba:
.. index:: pair: function; get_input_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_input_port(const std::string& input_name) const

For operation node returns reference to an input port with specified name; applicable if port group has only one input port.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_name

		- Name of port group



.. rubric:: Returns:

Appropriate input port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1a1901f11ec350ff05e6e54d625ad48ad8:
.. index:: pair: function; get_input_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_input_port(const std::string& input_name, int input_port_index) const

For operation node returns reference to an input port with specified name and index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_name

		- Name of port group, each group can have multiple ports

	*
		- input_port_index

		- :ref:`Input <doxid-classov_1_1_input>` port index in a group



.. rubric:: Returns:

Appropriate input port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1a3cd154f9642c6aee6dd253a20a12007d:
.. index:: pair: function; get_output_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_output_port() const

For operation node returns reference to an output port; applicable for operations with only one output port.



.. rubric:: Returns:

Appropriate output port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1a435c107c39adbefb0c9fe79a54ac317d:
.. index:: pair: function; get_output_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_output_port(int output_port_index) const

For operation node returns reference to an output port with specified index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_port_index

		- :ref:`Output <doxid-classov_1_1_output>` port index



.. rubric:: Returns:

Appropriate output port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1af769196021551e75af17c0eae8df5cca:
.. index:: pair: function; get_output_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_output_port(const std::string& output_name) const

For operation node returns reference to an output port with specified name; applicable if port group has only one output port.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_name

		- Name of output port group



.. rubric:: Returns:

Appropriate output port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1a86b7306a6f620d4d5388f0f07b357504:
.. index:: pair: function; get_output_port

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>` get_output_port(
		const std::string& output_name,
		int output_port_index
		) const

For operation node returns reference to an output port with specified name and index.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- output_name

		- Name of output port group, each group can have multiple ports

	*
		- output_port_index

		- :ref:`Output <doxid-classov_1_1_output>` port index



.. rubric:: Returns:

Appropriate output port place or nullptr if not exists

.. _doxid-classov_1_1frontend_1_1_place_1af7bb27d15bb36859435c225820088eb4:
.. index:: pair: function; get_consuming_ports

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`Place::Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`> get_consuming_ports() const

Returns all input ports that consume data flows through this place.

.. _doxid-classov_1_1frontend_1_1_place_1a25b0b484093cdc13a007d36599768124:
.. index:: pair: function; is_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_input() const

Returns true if this place is input for a model.

.. _doxid-classov_1_1frontend_1_1_place_1a55838cb299a83a6c1275bb8a4d42ec5c:
.. index:: pair: function; is_output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_output() const

Returns true if this place is output for a model.

.. _doxid-classov_1_1frontend_1_1_place_1aecfaab756f47e369d89b33983c4c176b:
.. index:: pair: function; is_equal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_equal(const :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& another) const

Returns true if another place is the same as this place.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- another

		- Another place object

.. _doxid-classov_1_1frontend_1_1_place_1aa4a4bc7f418906c41f66fd3d2774bc36:
.. index:: pair: function; is_equal_data

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_equal_data(const :ref:`Ptr<doxid-classov_1_1frontend_1_1_place_1ae93b8f34d75d2208e1894601ca8fa86c>`& another) const

Returns true if another place points to the same data.

The same data means all places on path: output port -> output edge -> tensor -> input edge -> input port.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- another

		- Another place object


