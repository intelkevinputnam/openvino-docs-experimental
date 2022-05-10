.. index:: pair: class; InferenceEngine::RemoteContext
.. _doxid-class_inference_engine_1_1_remote_context:

class InferenceEngine::RemoteContext
====================================



Overview
~~~~~~~~

This class represents an Inference Engine abstraction for remote (non-CPU) accelerator device-specific execution context. Such context represents a scope on the device within which executable networks and remote memory blobs can exist, function and exchange data. :ref:`More...<details-class_inference_engine_1_1_remote_context>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_remote_context.hpp>
	
	class RemoteContext: public std::enable_shared_from_this< RemoteContext >
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<RemoteContext> :ref:`Ptr<doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93>`;
		typedef std::shared_ptr<const RemoteContext> :ref:`CPtr<doxid-class_inference_engine_1_1_remote_context_1a67424c5e4360db20e621ced6fbd406be>`;

		// methods
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		bool :ref:`is<doxid-class_inference_engine_1_1_remote_context_1acf2f061a42ddb6678ef6e04df868a9b8>`();
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		bool :ref:`is<doxid-class_inference_engine_1_1_remote_context_1a7101e3faa737b9fa6c4d69e5d89358ef>`() const;
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		T \* :ref:`as<doxid-class_inference_engine_1_1_remote_context_1a9b0aa51076f3293c14c8967fa390098f>`();
	
		template <
			typename T,
			typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
			typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
			>
		const T \* :ref:`as<doxid-class_inference_engine_1_1_remote_context_1ad46a1b2173cc5806c907976c79f76e71>`() const;
	
		virtual std::string :ref:`getDeviceName<doxid-class_inference_engine_1_1_remote_context_1a5d3cd0e80b7b5442082e8bc51e42e1c3>`() const = 0;
	
		virtual :ref:`RemoteBlob::Ptr<doxid-class_inference_engine_1_1_remote_blob_1a495fd7cc9fbb55b2e0b6bc8b8790197b>` :ref:`CreateBlob<doxid-class_inference_engine_1_1_remote_context_1afe1313eb1a0d6f06fbb4a99889956145>`(
			const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc,
			const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params = {}
			) = 0;
	
		virtual :ref:`MemoryBlob::Ptr<doxid-class_inference_engine_1_1_memory_blob_1a294bf7449b6181f29ac05636a5968e1d>` :ref:`CreateHostBlob<doxid-class_inference_engine_1_1_remote_context_1a1c4a610a7e4ec6c9e66a338e858635da>`(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc);
		virtual :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>` :ref:`getParams<doxid-class_inference_engine_1_1_remote_context_1a2c6be24d0fbf02fcd3028b81945e8c90>`() const = 0;
	};

	// direct descendants

	class :ref:`ClContext<doxid-class_inference_engine_1_1gpu_1_1_cl_context>`;
.. _details-class_inference_engine_1_1_remote_context:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an Inference Engine abstraction for remote (non-CPU) accelerator device-specific execution context. Such context represents a scope on the device within which executable networks and remote memory blobs can exist, function and exchange data.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_remote_context_1adc79805c11b6939c51a794b90b8bfa93:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<RemoteContext> Ptr

A smart pointer to the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object.

.. _doxid-class_inference_engine_1_1_remote_context_1a67424c5e4360db20e621ced6fbd406be:
.. index:: pair: typedef; CPtr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<const RemoteContext> CPtr

A smart pointer to the const :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object.

Methods
-------

.. _doxid-class_inference_engine_1_1_remote_context_1acf2f061a42ddb6678ef6e04df868a9b8:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
		>
	bool is()

Checks if the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object can be cast to the type T\*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to be checked. Must represent a class derived from the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>`



.. rubric:: Returns:

true if this object can be dynamically cast to the type T\*. Otherwise, false

.. _doxid-class_inference_engine_1_1_remote_context_1a7101e3faa737b9fa6c4d69e5d89358ef:
.. index:: pair: function; is

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
		>
	bool is() const

Checks if the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object can be cast to the type const T\*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to be checked. Must represent a class derived from the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>`



.. rubric:: Returns:

true if this object can be dynamically cast to the type const T\*. Otherwise, false

.. _doxid-class_inference_engine_1_1_remote_context_1a9b0aa51076f3293c14c8967fa390098f:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
		>
	T \* as()

Casts this :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object to the type T\*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to cast to. Must represent a class derived from the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>`



.. rubric:: Returns:

Raw pointer to the object of the type T or nullptr on error

.. _doxid-class_inference_engine_1_1_remote_context_1ad46a1b2173cc5806c907976c79f76e71:
.. index:: pair: function; as

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename T,
		typename std::enable_if<!std::is_pointer<T>::value&&!std::is_reference<T>::value, int>::type = 0,
		typename std::enable_if<std::is_base_of<RemoteContext, T>::value, int>::type = 0
		>
	const T \* as() const

Casts this :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>` object to the type const T\*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- Type to cast to. Must represent a class derived from the :ref:`RemoteContext <doxid-class_inference_engine_1_1_remote_context>`



.. rubric:: Returns:

Raw pointer to the object of the type const T or nullptr on error

.. _doxid-class_inference_engine_1_1_remote_context_1a5d3cd0e80b7b5442082e8bc51e42e1c3:
.. index:: pair: function; getDeviceName

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getDeviceName() const = 0

Returns name of the device on which underlying object is allocated. Abstract method.



.. rubric:: Returns:

A device name string in the same format as that in plugin metric.

.. _doxid-class_inference_engine_1_1_remote_context_1afe1313eb1a0d6f06fbb4a99889956145:
.. index:: pair: function; CreateBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`RemoteBlob::Ptr<doxid-class_inference_engine_1_1_remote_blob_1a495fd7cc9fbb55b2e0b6bc8b8790197b>` CreateBlob(
		const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc,
		const :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>`& params = {}
		) = 0

Allocates memory blob in device memory or wraps user-supplied memory handle using the specified tensor description and low-level device-specific parameters. Returns a pointer to the object which implements :ref:`RemoteBlob <doxid-class_inference_engine_1_1_remote_blob>` interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Defines the layout and dims of the blob

	*
		- params

		- Map of the low-level blob object parameters. Abstract method.



.. rubric:: Returns:

A pointer to plugin object that implements :ref:`RemoteBlob <doxid-class_inference_engine_1_1_remote_blob>` interface.

.. _doxid-class_inference_engine_1_1_remote_context_1a1c4a610a7e4ec6c9e66a338e858635da:
.. index:: pair: function; CreateHostBlob

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`MemoryBlob::Ptr<doxid-class_inference_engine_1_1_memory_blob_1a294bf7449b6181f29ac05636a5968e1d>` CreateHostBlob(const :ref:`TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& tensorDesc)

Allocates host accessible memory blob friendly for the device in current context Returns a pointer to the object which implements :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensorDesc

		- Defines the layout and dims of the blob



.. rubric:: Returns:

A pointer to host accessible :ref:`MemoryBlob <doxid-class_inference_engine_1_1_memory_blob>` object

.. _doxid-class_inference_engine_1_1_remote_context_1a2c6be24d0fbf02fcd3028b81945e8c90:
.. index:: pair: function; getParams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ParamMap<doxid-namespace_inference_engine_1ab952963217c4a8b098fd90ba51708a9f>` getParams() const = 0

Returns a map of device-specific parameters required for low-level operations with underlying object. Parameters include device/context handles, access flags, etc. Contents of the map returned depend on remote execution context that is currently set on the device (working scenario). Abstract method.



.. rubric:: Returns:

A map of name/parameter elements.


