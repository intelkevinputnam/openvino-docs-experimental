.. index:: pair: class; ov::Output<const Node>
.. _doxid-classov_1_1_output_3_01const_01_node_01_4:

class ov::Output<const Node>
============================



Overview
~~~~~~~~

A handle for one of a node's outputs. :ref:`More...<details-classov_1_1_output_3_01const_01_node_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node_output.hpp>
	
	template <>
	class Output<const Node>
	{
	public:
		// construction
	
		:ref:`Output<doxid-classov_1_1_output_3_01const_01_node_01_4_1a1305722cabd05f013a2a98e4e490e2cd>`(const :ref:`Node<doxid-classov_1_1_node>` \* node, size_t index);
		:ref:`Output<doxid-classov_1_1_output_3_01const_01_node_01_4_1ae7eb1f6914fe43c44fd2228e33ebfa8b>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node, size_t index);
	
		template <typename T>
		:ref:`Output<doxid-classov_1_1_output_3_01const_01_node_01_4_1ad33c3656d84675c6214a358126288f48>`(const std::shared_ptr<const T>& node);
	
		:ref:`Output<doxid-classov_1_1_output_3_01const_01_node_01_4_1a7b6e24a2a10079aa95c5bc4414d39523>`();

		// methods
	
		void :target:`reset<doxid-classov_1_1_output_3_01const_01_node_01_4_1ade3aed245075fe75639415c1e3fd6786>`();
		const :ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_node<doxid-classov_1_1_output_3_01const_01_node_01_4_1a7bac4bd99c2c8df1635983ac6e38d59a>`() const;
		std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`> :ref:`get_node_shared_ptr<doxid-classov_1_1_output_3_01const_01_node_01_4_1aaeee5126c1ea4db526fabcb52a00d336>`() const;
		size_t :ref:`get_index<doxid-classov_1_1_output_3_01const_01_node_01_4_1ad6967d561df6a0d54209a774243737b0>`() const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_tensor<doxid-classov_1_1_output_3_01const_01_node_01_4_1a2cd76d76d5417e4d35565ce4d9853c78>`() const;
		std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> :ref:`get_tensor_ptr<doxid-classov_1_1_output_3_01const_01_node_01_4_1a5ee8a7df5553214f9d21209f9ad8463c>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1_output_3_01const_01_node_01_4_1a74541307e95551f5c37889954899fd1b>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1_output_3_01const_01_node_01_4_1ae9812be27add44ea48ba3053432e9ab2>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classov_1_1_output_3_01const_01_node_01_4_1af2f9926a7c868c0a68e3806548ea52a8>`() const;
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :ref:`get_rt_info<doxid-classov_1_1_output_3_01const_01_node_01_4_1ae44adf0149f36dea5b4c270ac2330aaf>`() const;
		const std::unordered_set<std::string>& :ref:`get_names<doxid-classov_1_1_output_3_01const_01_node_01_4_1a8e5b7de7bc0d8ebf1cb089b68f37a6b0>`() const;
		std::string :ref:`get_any_name<doxid-classov_1_1_output_3_01const_01_node_01_4_1ac0c2aa78bf780e66837f9a2ce60f8d14>`() const;
		std::set<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`get_target_inputs<doxid-classov_1_1_output_3_01const_01_node_01_4_1a2a94bb181f372ed686ac2e5c9bf2e621>`() const;
		bool :target:`operator ==<doxid-classov_1_1_output_3_01const_01_node_01_4_1a5369e99e6c49a28acbc6e86d5a204a8a>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator !=<doxid-classov_1_1_output_3_01const_01_node_01_4_1a4bf4bd7dee94bacdad79b8848d2b685c>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator <<doxid-classov_1_1_output_3_01const_01_node_01_4_1a17091559baf82003af59d8d878bef664>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator ><doxid-classov_1_1_output_3_01const_01_node_01_4_1ae01767508950f4ac4f26fdb7e3e3c6aa>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator <=<doxid-classov_1_1_output_3_01const_01_node_01_4_1ab0e4ae5a1019d90c126e8c7195695dcf>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator >=<doxid-classov_1_1_output_3_01const_01_node_01_4_1a59f048dff59c38f9c2901d5d2462e7a7>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
	};
.. _details-classov_1_1_output_3_01const_01_node_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A handle for one of a node's outputs.

Construction
------------

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a1305722cabd05f013a2a98e4e490e2cd:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output(const :ref:`Node<doxid-classov_1_1_node>` \* node, size_t index)

Constructs a :ref:`Output <doxid-classov_1_1_output>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- A pointer to the node for the output handle.

	*
		- index

		- The index of the output.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1ae7eb1f6914fe43c44fd2228e33ebfa8b:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node, size_t index)

Constructs a :ref:`Output <doxid-classov_1_1_output>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- A ``shared_ptr`` to the node for the output handle.

	*
		- index

		- The index of the output.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1ad33c3656d84675c6214a358126288f48:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	Output(const std::shared_ptr<const T>& node)

Constructs a :ref:`Output <doxid-classov_1_1_output>`, referencing the zeroth output of the node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- A ``shared_ptr`` to the node for the output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a7b6e24a2a10079aa95c5bc4414d39523:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output()

A null output.

Methods
-------

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a7bac4bd99c2c8df1635983ac6e38d59a:
.. index:: pair: function; get_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Node<doxid-classov_1_1_node>` \* get_node() const



.. rubric:: Returns:

A pointer to the node referred to by this output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1aaeee5126c1ea4db526fabcb52a00d336:
.. index:: pair: function; get_node_shared_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`> get_node_shared_ptr() const



.. rubric:: Returns:

A ``shared_ptr`` to the node referred to by this output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1ad6967d561df6a0d54209a774243737b0:
.. index:: pair: function; get_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_index() const



.. rubric:: Returns:

The index of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a2cd76d76d5417e4d35565ce4d9853c78:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& get_tensor() const



.. rubric:: Returns:

A reference to the tensor descriptor for this output.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a5ee8a7df5553214f9d21209f9ad8463c:
.. index:: pair: function; get_tensor_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> get_tensor_ptr() const



.. rubric:: Returns:

A shared point to the tensor ptr for this output.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a74541307e95551f5c37889954899fd1b:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const



.. rubric:: Returns:

The element type of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1ae9812be27add44ea48ba3053432e9ab2:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_shape() const



.. rubric:: Returns:

The shape of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1af2f9926a7c868c0a68e3806548ea52a8:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const



.. rubric:: Returns:

The partial shape of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1ae44adf0149f36dea5b4c270ac2330aaf:
.. index:: pair: function; get_rt_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& get_rt_info() const



.. rubric:: Returns:

The constant reference to runtime info map

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a8e5b7de7bc0d8ebf1cb089b68f37a6b0:
.. index:: pair: function; get_names

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::unordered_set<std::string>& get_names() const



.. rubric:: Returns:

The tensor names associated with this output

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1ac0c2aa78bf780e66837f9a2ce60f8d14:
.. index:: pair: function; get_any_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string get_any_name() const



.. rubric:: Returns:

:ref:`Any <doxid-classov_1_1_any>` tensor name associated with this output

.. _doxid-classov_1_1_output_3_01const_01_node_01_4_1a2a94bb181f372ed686ac2e5c9bf2e621:
.. index:: pair: function; get_target_inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::set<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> get_target_inputs() const



.. rubric:: Returns:

A set containing handles for all inputs targeted by the output referenced by this output handle.


.. index:: pair: class; ov::Output<Node>
.. _doxid-classov_1_1_output_3_01_node_01_4:

class ov::Output<Node>
^^^^^^^^^^^^^^^^^^^^^^



Overview
~~~~~~~~

A handle for one of a node's outputs. :ref:`More...<details-classov_1_1_output_3_01_node_01_4>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node_output.hpp>
	
	template <>
	class Output<Node>
	{
	public:
		// construction
	
		:ref:`Output<doxid-classov_1_1_output_3_01_node_01_4_1a904213ae2fdb6b3d9ad552eba922c15a>`(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index);
		:ref:`Output<doxid-classov_1_1_output_3_01_node_01_4_1a1464bc5cba5f76fcfe772b24df9fbb41>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node, size_t index);
	
		template <typename T>
		:ref:`Output<doxid-classov_1_1_output_3_01_node_01_4_1a651c333cde68d2d5a420c3984263af03>`(const std::shared_ptr<T>& node);
	
		:ref:`Output<doxid-classov_1_1_output_3_01_node_01_4_1a366ad2eaa7930ca3d6037f6604955956>`();

		// methods
	
		void :target:`reset<doxid-classov_1_1_output_3_01_node_01_4_1af750c4ab1ad202e7fec31b65c920dad6>`();
		:ref:`Node<doxid-classov_1_1_node>` \* :ref:`get_node<doxid-classov_1_1_output_3_01_node_01_4_1a850674ffb3a8902361fdeb8b360c8e9f>`() const;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_node_shared_ptr<doxid-classov_1_1_output_3_01_node_01_4_1abc587b38fe0216deaa5c03e8c4d39233>`() const;
		size_t :ref:`get_index<doxid-classov_1_1_output_3_01_node_01_4_1a0e457c9b3627be6775476b1c5e81b99e>`() const;
		:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& :ref:`get_tensor<doxid-classov_1_1_output_3_01_node_01_4_1af6afc29262fc044066e6202f708ab52e>`() const;
		std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> :ref:`get_tensor_ptr<doxid-classov_1_1_output_3_01_node_01_4_1a1e839de694a9344c070d8cc066b8f83d>`() const;
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :ref:`get_element_type<doxid-classov_1_1_output_3_01_node_01_4_1aed07fdc2ce98a95d3b14292da1ce8d45>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :ref:`get_shape<doxid-classov_1_1_output_3_01_node_01_4_1ad28e6aa28c3d34142de20bb9fe16d5ea>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :ref:`get_partial_shape<doxid-classov_1_1_output_3_01_node_01_4_1adbcb8a607a4d31efe4f1ea04f16307db>`() const;
		:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :ref:`get_rt_info<doxid-classov_1_1_output_3_01_node_01_4_1a50460a6a648bd29899423d5bec56b70f>`();
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :ref:`get_rt_info<doxid-classov_1_1_output_3_01_node_01_4_1a8c1f891156481c953a8aa62e06cccebb>`() const;
		const std::unordered_set<std::string>& :ref:`get_names<doxid-classov_1_1_output_3_01_node_01_4_1a439ce0103c52c953a2c568f9450f4ebc>`() const;
		std::string :ref:`get_any_name<doxid-classov_1_1_output_3_01_node_01_4_1ad564b2270333b7389075e0ca0794a2a9>`() const;
		void :ref:`set_names<doxid-classov_1_1_output_3_01_node_01_4_1a399fb6bd2693085ff4f700e6584dc981>`(const std::unordered_set<std::string>& names);
		void :ref:`add_names<doxid-classov_1_1_output_3_01_node_01_4_1a2a96e4d4e9a2de8716755835acd09e1c>`(const std::unordered_set<std::string>& names);
		std::set<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :ref:`get_target_inputs<doxid-classov_1_1_output_3_01_node_01_4_1a6597e846409eccafb728e15fe4557568>`() const;
		void :ref:`remove_target_input<doxid-classov_1_1_output_3_01_node_01_4_1a99173df52059fdd8b5815662709d12ca>`(const :ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>& target_input) const;
		void :ref:`replace<doxid-classov_1_1_output_3_01_node_01_4_1a6ea8bcfbc89a0ab58889be0306eab79b>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& replacement);
		bool :target:`operator ==<doxid-classov_1_1_output_3_01_node_01_4_1ae9fe5d9f5873765ea794434b4b9ffcaf>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator !=<doxid-classov_1_1_output_3_01_node_01_4_1ab5a6e1baacfa0f95a1306e40ae72fc81>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator <<doxid-classov_1_1_output_3_01_node_01_4_1a9649da9fcc18a289548e4ba4e72196db>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator ><doxid-classov_1_1_output_3_01_node_01_4_1afdf1aa208dcfbf92d42f1556efee3ca6>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator <=<doxid-classov_1_1_output_3_01_node_01_4_1a363415d45fd8b86c6855577663910180>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
		bool :target:`operator >=<doxid-classov_1_1_output_3_01_node_01_4_1a8355ebafad51580dd2d9850bbbcacda8>` (const :ref:`Output<doxid-classov_1_1_output>`& other) const;
	};
.. _details-classov_1_1_output_3_01_node_01_4:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A handle for one of a node's outputs.

Construction
------------

.. _doxid-classov_1_1_output_3_01_node_01_4_1a904213ae2fdb6b3d9ad552eba922c15a:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index)

Constructs a :ref:`Output <doxid-classov_1_1_output>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- A pointer to the node for the output handle.

	*
		- index

		- The index of the output.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a1464bc5cba5f76fcfe772b24df9fbb41:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node, size_t index)

Constructs a :ref:`Output <doxid-classov_1_1_output>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- A ``shared_ptr`` to the node for the output handle.

	*
		- index

		- The index of the output.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a651c333cde68d2d5a420c3984263af03:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	Output(const std::shared_ptr<T>& node)

Constructs a :ref:`Output <doxid-classov_1_1_output>`, referencing the zeroth output of the node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- A ``shared_ptr`` to the node for the output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a366ad2eaa7930ca3d6037f6604955956:
.. index:: pair: function; Output

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Output()

A null output.

Methods
-------

.. _doxid-classov_1_1_output_3_01_node_01_4_1a850674ffb3a8902361fdeb8b360c8e9f:
.. index:: pair: function; get_node

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Node<doxid-classov_1_1_node>` \* get_node() const



.. rubric:: Returns:

A pointer to the node referred to by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1abc587b38fe0216deaa5c03e8c4d39233:
.. index:: pair: function; get_node_shared_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> get_node_shared_ptr() const



.. rubric:: Returns:

A ``shared_ptr`` to the node referred to by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a0e457c9b3627be6775476b1c5e81b99e:
.. index:: pair: function; get_index

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_index() const



.. rubric:: Returns:

The index of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1af6afc29262fc044066e6202f708ab52e:
.. index:: pair: function; get_tensor

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`& get_tensor() const



.. rubric:: Returns:

A reference to the tensor descriptor for this output.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a1e839de694a9344c070d8cc066b8f83d:
.. index:: pair: function; get_tensor_ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`descriptor::Tensor<doxid-classov_1_1descriptor_1_1_tensor>`> get_tensor_ptr() const



.. rubric:: Returns:

A shared point to the tensor ptr for this output.

.. _doxid-classov_1_1_output_3_01_node_01_4_1aed07fdc2ce98a95d3b14292da1ce8d45:
.. index:: pair: function; get_element_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& get_element_type() const



.. rubric:: Returns:

The element type of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1ad28e6aa28c3d34142de20bb9fe16d5ea:
.. index:: pair: function; get_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Shape<doxid-classov_1_1_shape>`& get_shape() const



.. rubric:: Returns:

The shape of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1adbcb8a607a4d31efe4f1ea04f16307db:
.. index:: pair: function; get_partial_shape

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& get_partial_shape() const



.. rubric:: Returns:

The partial shape of the output referred to by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a50460a6a648bd29899423d5bec56b70f:
.. index:: pair: function; get_rt_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& get_rt_info()



.. rubric:: Returns:

The reference to runtime info map

.. _doxid-classov_1_1_output_3_01_node_01_4_1a8c1f891156481c953a8aa62e06cccebb:
.. index:: pair: function; get_rt_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& get_rt_info() const



.. rubric:: Returns:

The constant reference to runtime info map

.. _doxid-classov_1_1_output_3_01_node_01_4_1a439ce0103c52c953a2c568f9450f4ebc:
.. index:: pair: function; get_names

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::unordered_set<std::string>& get_names() const



.. rubric:: Returns:

The tensor names associated with this output

.. _doxid-classov_1_1_output_3_01_node_01_4_1ad564b2270333b7389075e0ca0794a2a9:
.. index:: pair: function; get_any_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string get_any_name() const



.. rubric:: Returns:

:ref:`Any <doxid-classov_1_1_any>` tensor names associated with this output

.. _doxid-classov_1_1_output_3_01_node_01_4_1a399fb6bd2693085ff4f700e6584dc981:
.. index:: pair: function; set_names

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_names(const std::unordered_set<std::string>& names)



.. rubric:: Returns:

Set tensor names associated with this output

.. _doxid-classov_1_1_output_3_01_node_01_4_1a2a96e4d4e9a2de8716755835acd09e1c:
.. index:: pair: function; add_names

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_names(const std::unordered_set<std::string>& names)



.. rubric:: Returns:

Add tensor names associated with this output

.. _doxid-classov_1_1_output_3_01_node_01_4_1a6597e846409eccafb728e15fe4557568:
.. index:: pair: function; get_target_inputs

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::set<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> get_target_inputs() const



.. rubric:: Returns:

A set containing handles for all inputs targeted by the output referenced by this output handle.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a99173df52059fdd8b5815662709d12ca:
.. index:: pair: function; remove_target_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove_target_input(const :ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>& target_input) const

Removes a target input from the output referenced by this output handle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- target_input

		- The target input to remove.

.. _doxid-classov_1_1_output_3_01_node_01_4_1a6ea8bcfbc89a0ab58889be0306eab79b:
.. index:: pair: function; replace

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void replace(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& replacement)

Replace all users of this value with replacement.


.. index:: pair: class; ov::Output
.. _doxid-classov_1_1_output:

class ov::Output
^^^^^^^^^^^^^^^^






