.. index:: pair: class; ngraph::runtime::HostTensor
.. _doxid-classngraph_1_1runtime_1_1_host_tensor:

class ngraph::runtime::HostTensor
=================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <host_tensor.hpp>
	
	class HostTensor: public :ref:`ngraph::runtime::Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`
	{
	public:
		// construction
	
		:target:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor_1a00930af7373eb8de466be29ba0818f83>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			const :ref:`Shape<doxid-classov_1_1_shape>`& shape,
			void \* memory_pointer
			);
	
		:target:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor_1a8fd09e5a39f7eacd126bbc5dfcaa2b1a>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type, const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
		:target:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor_1ae112516ecc083139f576106de6714bea>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type, const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& partial_shape);
		:target:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor_1a9558622a2633ab6717ab794a15a0510b>`();
		:target:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor_1a1a390224405f0e3ca4f0cc32fa916fd1>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`ov::Node<doxid-classov_1_1_node>`>&);
		:target:`HostTensor<doxid-classngraph_1_1runtime_1_1_host_tensor_1ae0cd683247ddeac691d3bf2625e3e7e7>`(const std::shared_ptr<:ref:`op::v0::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`>& constant);

		// methods
	
		void :target:`initialize<doxid-classngraph_1_1runtime_1_1_host_tensor_1a116815bac9067301c81ea8603de5696b>`(const std::shared_ptr<:ref:`op::v0::Constant<doxid-classov_1_1op_1_1v0_1_1_constant>`>& constant);
		void \* :target:`get_data_ptr<doxid-classngraph_1_1runtime_1_1_host_tensor_1af5549bde0557fd07a6ecae0bb106a0bd>`();
		const void \* :target:`get_data_ptr<doxid-classngraph_1_1runtime_1_1_host_tensor_1a8da23c2134408c7bb0b271d69a74d7f6>`() const;
	
		template <typename T>
		T \* :target:`get_data_ptr<doxid-classngraph_1_1runtime_1_1_host_tensor_1ad2b62d5db1f81851054a448de0c9801b>`();
	
		template <typename T>
		const T \* :target:`get_data_ptr<doxid-classngraph_1_1runtime_1_1_host_tensor_1a164783a86bc6dc005466f161d60a9406>`() const;
	
		template <element::Type_t ET>
		:ref:`element_type_traits<doxid-structov_1_1element__type__traits>`<ET>::value_type \* :target:`get_data_ptr<doxid-classngraph_1_1runtime_1_1_host_tensor_1aea7d844e1727bddc1598d50d34e26e1d>`();
	
		template <element::Type_t ET>
		const :ref:`element_type_traits<doxid-structov_1_1element__type__traits>`<ET>::value_type \* :target:`get_data_ptr<doxid-classngraph_1_1runtime_1_1_host_tensor_1ab6a72e97f5b39ff36943452a7ca628df>`() const;
	
		virtual void :ref:`write<doxid-classngraph_1_1runtime_1_1_host_tensor_1a2736b4e0d47ba22c059283924dcd7610>`(const void \* p, size_t n);
		virtual void :ref:`read<doxid-classngraph_1_1runtime_1_1_host_tensor_1a2c0d121e808b80f34b6e5315b68237f8>`(void \* p, size_t n) const;
		bool :target:`get_is_allocated<doxid-classngraph_1_1runtime_1_1_host_tensor_1acf7a6eb9460f2d07856bfbe767edc355>`() const;
		void :ref:`set_element_type<doxid-classngraph_1_1runtime_1_1_host_tensor_1a348eeada5caaaf45c16e25a3161402a5>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type);
		void :ref:`set_shape<doxid-classngraph_1_1runtime_1_1_host_tensor_1a10d681b4885a21269e7f00346d33010c>`(const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
		void :ref:`set_unary<doxid-classngraph_1_1runtime_1_1_host_tensor_1a5d1f868239574f816df35b14fd49f54f>`(const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg);
	
		void :ref:`set_broadcast<doxid-classngraph_1_1runtime_1_1_host_tensor_1ad281b4bbdb537daa4cc873c7b0611775>`(
			const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob,
			const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg0,
			const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg1
			);
	
		void :ref:`set_broadcast<doxid-classngraph_1_1runtime_1_1_host_tensor_1aedc326d663a8f8cfe7d2777c0e75f351>`(
			const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob,
			const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg0,
			const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg1,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		:ref:`Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`& :ref:`operator =<doxid-classngraph_1_1runtime_1_1_tensor_1a25c8a91a938c29b394eb24f6dc653ba2>` (const :ref:`Tensor<doxid-classngraph_1_1runtime_1_1_tensor>`&);
		virtual const :ref:`ngraph::Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classngraph_1_1runtime_1_1_tensor_1af3a5be2f9eda14fd567de39762d80ea3>`() const;
		const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classngraph_1_1runtime_1_1_tensor_1a1f1fa49dd7f517920fd249edda04fca4>`() const;
		virtual const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classngraph_1_1runtime_1_1_tensor_1a6ad0f55881641ee465c2773139faabae>`() const;
		virtual size_t :ref:`get_element_count<doxid-classngraph_1_1runtime_1_1_tensor_1a71f529fa5a4f95e7567cf1874e03f860>`() const;
		virtual size_t :ref:`get_size_in_bytes<doxid-classngraph_1_1runtime_1_1_tensor_1a65ff89c5d21f5f82d3de9fd4727b5873>`() const;
		const std::string& :ref:`get_name<doxid-classngraph_1_1runtime_1_1_tensor_1ac64f756bfa4dc604105e0813084d74e9>`() const;
		virtual void :ref:`write<doxid-classngraph_1_1runtime_1_1_tensor_1a6c61347d78e71fe0c6b95bff92f4d248>`(const void \* p, size_t n) = 0;
		virtual void :ref:`read<doxid-classngraph_1_1runtime_1_1_tensor_1a53bb688a972469338ab597b0eb29ef4f>`(void \* p, size_t n) const = 0;

.. _details-classngraph_1_1runtime_1_1_host_tensor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1a2736b4e0d47ba22c059283924dcd7610:
.. index:: pair: function; write

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void write(const void \* p, size_t n)

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

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1a2c0d121e808b80f34b6e5315b68237f8:
.. index:: pair: function; read

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void read(void \* p, size_t n) const

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

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1a348eeada5caaaf45c16e25a3161402a5:
.. index:: pair: function; set_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_element_type(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type)

Set the element type. Must be compatible with the current element type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- element_type

		- The element type

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1a10d681b4885a21269e7f00346d33010c:
.. index:: pair: function; set_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_shape(const :ref:`Shape<doxid-classov_1_1_shape>`& shape)

Set the actual shape of the tensor compatibly with the partial shape.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- shape

		- The shape being set

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1a5d1f868239574f816df35b14fd49f54f:
.. index:: pair: function; set_unary

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_unary(const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg)

Set the shape of a node from an input.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- arg

		- The input argument

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1ad281b4bbdb537daa4cc873c7b0611775:
.. index:: pair: function; set_broadcast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_broadcast(
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob,
		const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg0,
		const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg1
		)

Set the shape of the tensor using broadcast rules.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- autob

		- The broadcast mode

	*
		- arg0

		- The first argument

	*
		- arg1

		- The second argument

.. _doxid-classngraph_1_1runtime_1_1_host_tensor_1aedc326d663a8f8cfe7d2777c0e75f351:
.. index:: pair: function; set_broadcast

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_broadcast(
		const :ref:`op::AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec>`& autob,
		const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg0,
		const :ref:`HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& arg1,
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type
		)

Set the shape of the tensor using broadcast rules.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- autob

		- The broadcast mode

	*
		- arg0

		- The first argument

	*
		- arg1

		- The second argument

	*
		- element_type

		- The output element type


