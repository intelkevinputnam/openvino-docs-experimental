.. index:: pair: class; ngraph::runtime::Tensor
.. _doxid-classngraph_1_1runtime_1_1_tensor:

class ngraph::runtime::Tensor
=============================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <tensor.hpp>
	
	class Tensor
	{
	public:
		// methods
	
		Tensor& :target:`operator =<doxid-classngraph_1_1runtime_1_1_tensor_1a25c8a91a938c29b394eb24f6dc653ba2>` (const Tensor&);
		virtual const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classngraph_1_1runtime_1_1_tensor_1af3a5be2f9eda14fd567de39762d80ea3>`() const;
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classngraph_1_1runtime_1_1_tensor_1a1f1fa49dd7f517920fd249edda04fca4>`() const;
		virtual const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classngraph_1_1runtime_1_1_tensor_1a6ad0f55881641ee465c2773139faabae>`() const;
		virtual size_t :ref:`get_element_count<doxid-classngraph_1_1runtime_1_1_tensor_1a71f529fa5a4f95e7567cf1874e03f860>`() const;
		virtual size_t :ref:`get_size_in_bytes<doxid-classngraph_1_1runtime_1_1_tensor_1a65ff89c5d21f5f82d3de9fd4727b5873>`() const;
		const std::string& :ref:`get_name<doxid-classngraph_1_1runtime_1_1_tensor_1ac64f756bfa4dc604105e0813084d74e9>`() const;
		virtual void :ref:`write<doxid-classngraph_1_1runtime_1_1_tensor_1a6c61347d78e71fe0c6b95bff92f4d248>`(const void \* p, size_t n) = 0;
		virtual void :ref:`read<doxid-classngraph_1_1runtime_1_1_tensor_1a53bb688a972469338ab597b0eb29ef4f>`(void \* p, size_t n) const = 0;
	};

	// direct descendants

	class :ref:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor>`;
.. _details-classngraph_1_1runtime_1_1_tensor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classngraph_1_1runtime_1_1_tensor_1af3a5be2f9eda14fd567de39762d80ea3:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& get_shape() const

Get tensor shape.



.. rubric:: Returns:

const reference to a Shape

.. _doxid-classngraph_1_1runtime_1_1_tensor_1a1f1fa49dd7f517920fd249edda04fca4:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const

Get tensor partial shape.



.. rubric:: Returns:

const reference to a PartialShape

.. _doxid-classngraph_1_1runtime_1_1_tensor_1a6ad0f55881641ee465c2773139faabae:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const

Get tensor element type.



.. rubric:: Returns:

element::Type

.. _doxid-classngraph_1_1runtime_1_1_tensor_1a71f529fa5a4f95e7567cf1874e03f860:
.. index:: pair: function; get_element_count

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_element_count() const

Get number of elements in the tensor.



.. rubric:: Returns:

number of elements in the tensor

.. _doxid-classngraph_1_1runtime_1_1_tensor_1a65ff89c5d21f5f82d3de9fd4727b5873:
.. index:: pair: function; get_size_in_bytes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_size_in_bytes() const

Get the size in bytes of the tensor.



.. rubric:: Returns:

number of bytes in tensor's allocation

.. _doxid-classngraph_1_1runtime_1_1_tensor_1ac64f756bfa4dc604105e0813084d74e9:
.. index:: pair: function; get_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& get_name() const

Get tensor's unique name.



.. rubric:: Returns:

tensor's name

.. _doxid-classngraph_1_1runtime_1_1_tensor_1a6c61347d78e71fe0c6b95bff92f4d248:
.. index:: pair: function; write

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void write(const void \* p, size_t n) = 0

Write bytes directly into the tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- Pointer to source of data

	*
		- n

		- Number of bytes to write, must be integral number of elements.

.. _doxid-classngraph_1_1runtime_1_1_tensor_1a53bb688a972469338ab597b0eb29ef4f:
.. index:: pair: function; read

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void read(void \* p, size_t n) const = 0

Read bytes directly from the tensor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- p

		- Pointer to destination for data

	*
		- n

		- Number of bytes to read, must be integral number of elements.


