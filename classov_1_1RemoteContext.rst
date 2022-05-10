.. index:: pair: class; ov::RemoteContext
.. _doxid-classov_1_1_remote_context:

class ov::RemoteContext
=======================



Overview
~~~~~~~~

This class represents an abstraction

for remote (non-CPU) accelerator device-specific inference context. Such context represents a scope on the device within which compiled models and remote memory tensors can exist, function, and exchange data. :ref:`More...<details-classov_1_1_remote_context>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <remote_context.hpp>
	
	class RemoteContext
	{
	public:
		// construction
	
		:ref:`RemoteContext<doxid-classov_1_1_remote_context_1a7caa251a29106487817bf94f5682a97a>`();
		:ref:`RemoteContext<doxid-classov_1_1_remote_context_1a687dbc5e8954534ce1081c9aa1863811>`(const RemoteContext& other);
		:ref:`RemoteContext<doxid-classov_1_1_remote_context_1a4a6d25798ce1d235561078119ef761a7>`(RemoteContext&& other);

		// methods
	
		RemoteContext& :ref:`operator =<doxid-classov_1_1_remote_context_1a21458de48b8c09459af904e52211a821>` (const RemoteContext& other);
		RemoteContext& :ref:`operator =<doxid-classov_1_1_remote_context_1a7c57cd1cee1195ce0d0bd316db992d08>` (RemoteContext&& other);
	
		template <typename T>
		bool :ref:`is<doxid-classov_1_1_remote_context_1ad266845dbe86f7a187b659a9a1980198>`() const;
	
		template <typename T>
		const T :ref:`as<doxid-classov_1_1_remote_context_1a54021126344109640e35a18842d22654>`() const;
	
		:ref:`RemoteTensor<doxid-classov_1_1_remote_tensor>` :ref:`create_tensor<doxid-classov_1_1_remote_context_1ac1735cf031cfde65e2ced782b21cc256>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& params = {}
			);
	
		:ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>` :ref:`get_params<doxid-classov_1_1_remote_context_1a45f1cad216e6d44b811b89b78fe4e638>`() const;
		:ref:`Tensor<doxid-classov_1_1_tensor>` :ref:`create_host_tensor<doxid-classov_1_1_remote_context_1a5cfbba2a531a15c4f778a7a72092f848>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
	
		static void :ref:`type_check<doxid-classov_1_1_remote_context_1a1ce9cb6cb79a4fcfc21f03a8ed7cd257>`(
			const RemoteContext& remote_context,
			const std::map<std::string, std::vector<std::string>>& type_info = {}
			);
	};

	// direct descendants

	class :ref:`ClContext<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>`;
.. _details-classov_1_1_remote_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an abstraction

for remote (non-CPU) accelerator device-specific inference context. Such context represents a scope on the device within which compiled models and remote memory tensors can exist, function, and exchange data.

Construction
------------

.. _doxid-classov_1_1_remote_context_1a7caa251a29106487817bf94f5682a97a:
.. index:: pair: function; RemoteContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RemoteContext()

Default constructor.

.. _doxid-classov_1_1_remote_context_1a687dbc5e8954534ce1081c9aa1863811:
.. index:: pair: function; RemoteContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RemoteContext(const RemoteContext& other)

Default copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object.

.. _doxid-classov_1_1_remote_context_1a4a6d25798ce1d235561078119ef761a7:
.. index:: pair: function; RemoteContext

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RemoteContext(RemoteContext&& other)

Default move constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object.

Methods
-------

.. _doxid-classov_1_1_remote_context_1a21458de48b8c09459af904e52211a821:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RemoteContext& operator = (const RemoteContext& other)

Default copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object.



.. rubric:: Returns:

Reference to the current object.

.. _doxid-classov_1_1_remote_context_1a7c57cd1cee1195ce0d0bd316db992d08:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RemoteContext& operator = (RemoteContext&& other)

Default move assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- Another :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object.



.. rubric:: Returns:

Reference to the current object.

.. _doxid-classov_1_1_remote_context_1ad266845dbe86f7a187b659a9a1980198:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	bool is() const

Checks if the :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object can be cast to the type T.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to be checked. Must represent a class derived from :ref:`RemoteContext <doxid-classov_1_1_remote_context>`.



.. rubric:: Returns:

True if this object can be dynamically cast to the type T\*; false, otherwise.

.. _doxid-classov_1_1_remote_context_1a54021126344109640e35a18842d22654:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	const T as() const

Casts this :ref:`RemoteContext <doxid-classov_1_1_remote_context>` object to the type T.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to cast to. Must represent a class derived from :ref:`RemoteContext <doxid-classov_1_1_remote_context>`.



.. rubric:: Returns:

T Object.

.. _doxid-classov_1_1_remote_context_1ac1735cf031cfde65e2ced782b21cc256:
.. index:: pair: function; create_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RemoteTensor<doxid-classov_1_1_remote_tensor>` create_tensor(
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& type,
		const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
		const :ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>`& params = {}
		)

Allocates memory tensor in device memory or wraps user-supplied memory handle using the specified tensor description and low-level device-specific parameters. Returns a pointer to the object that implements the :ref:`RemoteTensor <doxid-classov_1_1_remote_tensor>` interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- Defines the element type of the tensor.

	*
		- shape

		- Defines the shape of the tensor.

	*
		- params

		- Map of the low-level tensor object parameters.



.. rubric:: Returns:

Pointer to a plugin object that implements the :ref:`RemoteTensor <doxid-classov_1_1_remote_tensor>` interface.

.. _doxid-classov_1_1_remote_context_1a45f1cad216e6d44b811b89b78fe4e638:
.. index:: pair: function; get_params

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>` get_params() const

Returns a map of device-specific parameters required for low-level operations with the underlying object. Parameters include device/context handles, access flags, etc. Content of the returned map depends on a remote execution context that is currently set on the device (working scenario). Abstract method.



.. rubric:: Returns:

A map of name/parameter elements.

.. _doxid-classov_1_1_remote_context_1a5cfbba2a531a15c4f778a7a72092f848:
.. index:: pair: function; create_host_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Tensor<doxid-classov_1_1_tensor>` create_host_tensor(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

This method is used to create a host tensor object friendly for the device in current context. For example, GPU context may allocate USM host memory (if corresponding extension is available), which could be more efficient than regular host memory.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- type

		- :ref:`Tensor <doxid-classov_1_1_tensor>` element type.

	*
		- shape

		- :ref:`Tensor <doxid-classov_1_1_tensor>` shape.



.. rubric:: Returns:

A tensor instance with device friendly memory.

.. _doxid-classov_1_1_remote_context_1a1ce9cb6cb79a4fcfc21f03a8ed7cd257:
.. index:: pair: function; type_check

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void type_check(
		const RemoteContext& remote_context,
		const std::map<std::string, std::vector<std::string>>& type_info = {}
		)

Internal method: checks remote type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- remote_context

		- Remote context which type is checked.

	*
		- type_info

		- Map with remote object runtime info.

	*
		- :ref:`Exception <doxid-classov_1_1_exception>`

		- if type check with the specified parameters failed.


