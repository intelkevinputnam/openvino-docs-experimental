.. index:: pair: class; ov::descriptor::Tensor
.. _doxid-classov_1_1descriptor_1_1_tensor:

class ov::descriptor::Tensor
============================



Overview
~~~~~~~~

Compile-time descriptor of a first-class value that is a tensor. :ref:`More...<details-classov_1_1descriptor_1_1_tensor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <tensor.hpp>
	
	class Tensor
	{
	public:
		// construction
	
		:target:`Tensor<doxid-classov_1_1descriptor_1_1_tensor_1aa6bbd3d175bfa3887af8895cc8481ed6>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& pshape,
			const std::string& name
			);
	
		:target:`Tensor<doxid-classov_1_1descriptor_1_1_tensor_1a9a066d373fefc5f4eedd10f7db7b2ac7>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& pshape,
			:ref:`Node<doxid-classov_1_1_node>` \* node,
			size_t node_output_number
			);
	
		:target:`Tensor<doxid-classov_1_1descriptor_1_1_tensor_1a1a73a6e34c0733fa675f9832c2cb5831>`(const Tensor&);

		// methods
	
		Tensor& :target:`operator =<doxid-classov_1_1descriptor_1_1_tensor_1a5e0bbb9f09c90397c0a58b7343163b0a>` (const Tensor&);
		const std::string& :target:`get_name<doxid-classov_1_1descriptor_1_1_tensor_1a2ed6343e4a1e589898caa0c73d762b00>`() const;
		void :target:`set_name<doxid-classov_1_1descriptor_1_1_tensor_1aa7895f42f5e18651c714968aced9bed2>`(const std::string& name);
		std::string :target:`get_any_name<doxid-classov_1_1descriptor_1_1_tensor_1ac2129906992afe8707103dbe694476b4>`() const;
		const std::unordered_set<std::string>& :target:`get_names<doxid-classov_1_1descriptor_1_1_tensor_1a981d713aa2aa324da27000271ae3072d>`() const;
		void :target:`set_names<doxid-classov_1_1descriptor_1_1_tensor_1a5f21c3cb845cbee0b7350163644776a0>`(const std::unordered_set<std::string>& names);
		void :target:`add_names<doxid-classov_1_1descriptor_1_1_tensor_1a59684a610333e00b8c7bd53ea9972874>`(const std::unordered_set<std::string>& names);
	
		void :target:`set_tensor_type<doxid-classov_1_1descriptor_1_1_tensor_1abaaa483d3e3d24d2fa352a8de75aa388>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& element_type,
			const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& pshape
			);
	
		void :target:`set_element_type<doxid-classov_1_1descriptor_1_1_tensor_1ab272069fb2f14982b013ec0dbf6e8e48>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& elemenet_type);
		void :target:`set_partial_shape<doxid-classov_1_1descriptor_1_1_tensor_1a3de4d613fa4f2c10b283c7b7fbebce4e>`(const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& partial_shape);
		void :ref:`set_lower_value<doxid-classov_1_1descriptor_1_1_tensor_1ac9cc21f8acafd9eff484a4c76a58b208>`(const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& value);
		void :ref:`set_upper_value<doxid-classov_1_1descriptor_1_1_tensor_1ae33edc114cc1fa124c9032ab7486e108>`(const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& value);
		void :ref:`set_value_label<doxid-classov_1_1descriptor_1_1_tensor_1aa40a677a189e041c6ee66dba7a6e9171>`(const :ref:`TensorLabel<doxid-namespaceov_1aac5494a3f0f95faa7e12788ce1747240>`& value_label);
		void :ref:`invalidate_values<doxid-classov_1_1descriptor_1_1_tensor_1aa51a0e3d1c3d4654ea4318e4ed38ed68>`();
		const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& :target:`get_element_type<doxid-classov_1_1descriptor_1_1_tensor_1a71121f46b7fed6549e556ec554f9386a>`() const;
		const :ref:`Shape<doxid-classov_1_1_shape>`& :target:`get_shape<doxid-classov_1_1descriptor_1_1_tensor_1a8ee4c9b226caf7ccdfbd58bb13f619ea>`() const;
		const :ref:`PartialShape<doxid-classov_1_1_partial_shape>`& :target:`get_partial_shape<doxid-classov_1_1descriptor_1_1_tensor_1a40f1e82d3e52aabe6d96288271413e6b>`() const;
		:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` :ref:`get_lower_value<doxid-classov_1_1descriptor_1_1_tensor_1a637d7364cbcd7610799a591e4c6291a7>`() const;
		:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` :ref:`get_upper_value<doxid-classov_1_1descriptor_1_1_tensor_1aeabcde47e2249cf9b4f267053dc43388>`() const;
		:ref:`TensorLabel<doxid-namespaceov_1aac5494a3f0f95faa7e12788ce1747240>` :ref:`get_value_label<doxid-classov_1_1descriptor_1_1_tensor_1aae3246093011ebc64ca4c45361f80337>`() const;
		bool :ref:`has_and_set_bound<doxid-classov_1_1descriptor_1_1_tensor_1a41217a3ca661c101de448566b98f50b8>`() const;
		size_t :target:`size<doxid-classov_1_1descriptor_1_1_tensor_1ab49a212953ab3549294dfb8812e09c9c>`() const;
		:ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1descriptor_1_1_tensor_1a3cf60af9d58fddfdbc0e604bf7a896c9>`();
		const :ref:`RTMap<doxid-namespaceov_1aa2bb09ec4478a90caec0ecda2ec47f40>`& :target:`get_rt_info<doxid-classov_1_1descriptor_1_1_tensor_1a37422d56ecc295a3775c3cee4d2960fd>`() const;
	};
.. _details-classov_1_1descriptor_1_1_tensor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Compile-time descriptor of a first-class value that is a tensor.

Methods
-------

.. _doxid-classov_1_1descriptor_1_1_tensor_1ac9cc21f8acafd9eff484a4c76a58b208:
.. index:: pair: function; set_lower_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_lower_value(const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& value)

sets lower bound value description

.. _doxid-classov_1_1descriptor_1_1_tensor_1ae33edc114cc1fa124c9032ab7486e108:
.. index:: pair: function; set_upper_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_upper_value(const :ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>`& value)

sets upper bound value description

.. _doxid-classov_1_1descriptor_1_1_tensor_1aa40a677a189e041c6ee66dba7a6e9171:
.. index:: pair: function; set_value_label

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_value_label(const :ref:`TensorLabel<doxid-namespaceov_1aac5494a3f0f95faa7e12788ce1747240>`& value_label)

sets value label description

.. _doxid-classov_1_1descriptor_1_1_tensor_1aa51a0e3d1c3d4654ea4318e4ed38ed68:
.. index:: pair: function; invalidate_values

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void invalidate_values()

unsets bound value descriptions

.. _doxid-classov_1_1descriptor_1_1_tensor_1a637d7364cbcd7610799a591e4c6291a7:
.. index:: pair: function; get_lower_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` get_lower_value() const

gets lower bound value description

.. _doxid-classov_1_1descriptor_1_1_tensor_1aeabcde47e2249cf9b4f267053dc43388:
.. index:: pair: function; get_upper_value

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ngraph::HostTensorPtr<doxid-classngraph_1addedbec9dcee7e1d2599da744bdfcecf>` get_upper_value() const

gets upper bound value description

.. _doxid-classov_1_1descriptor_1_1_tensor_1aae3246093011ebc64ca4c45361f80337:
.. index:: pair: function; get_value_label

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`TensorLabel<doxid-namespaceov_1aac5494a3f0f95faa7e12788ce1747240>` get_value_label() const

gets upper bound value description

.. _doxid-classov_1_1descriptor_1_1_tensor_1a41217a3ca661c101de448566b98f50b8:
.. index:: pair: function; has_and_set_bound

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has_and_set_bound() const

checks if lower and upper bound are set and point to the same HostTensor


