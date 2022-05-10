.. index:: pair: class; ov::OldApiMapOrder
.. _doxid-classov_1_1_old_api_map_order:

class ov::OldApiMapOrder
========================



Overview
~~~~~~~~

:ref:`OldApiMapOrder <doxid-classov_1_1_old_api_map_order>` class represents runtime info attribute that stores order of the transpose that is required for obtaining IR in old API. :ref:`More...<details-classov_1_1_old_api_map_order>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <old_api_map_order_attribute.hpp>
	
	class OldApiMapOrder: public :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`
	{
	public:
		// fields
	
		std::vector<uint64_t> :target:`value<doxid-classov_1_1_old_api_map_order_1a1da170cc39c2904881f89a48a2bf303f>`;

		// construction
	
		:ref:`OldApiMapOrder<doxid-classov_1_1_old_api_map_order_1a80a3da1c2665ef3e39037ee44b6c333e>`();
		:ref:`OldApiMapOrder<doxid-classov_1_1_old_api_map_order_1a741964829bf1728ef20135c62c477a49>`(const std::vector<uint64_t>& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_old_api_map_order_1a1df4bdda990d2b2f686054f0b9086604>`("old_api_map_order", "0");
		virtual bool :target:`is_copyable<doxid-classov_1_1_old_api_map_order_1a7b09c05c7d5ab5147feea31984e2ecd6>`() const;
		virtual bool :target:`visit_attributes<doxid-classov_1_1_old_api_map_order_1a5f7fef48a5f90eba174262bca39d5fb6>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Ptr<doxid-classov_1_1_runtime_attribute_1a0ac56ae81bace38d80c2c57e6695cf8f>`;
		typedef std::tuple<:::ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :ref:`Base<doxid-classov_1_1_runtime_attribute_1aa8d1a337411d2728e4d8beb58eeb7ccc>`;

		// methods
	
		static :ref:`_OPENVINO_HIDDEN_METHOD<doxid-core_2include_2openvino_2core_2visibility_8hpp_1a751977ff5ff49e1bfd5b4efc0b994f27>` const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info_static<doxid-classov_1_1_runtime_attribute_1a57fac9ef5e4f13144d53102212bed8c6>`();
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_runtime_attribute_1a1c452854e1d01d1852cca180327c6882>`() const;
		virtual bool :ref:`is_copyable<doxid-classov_1_1_runtime_attribute_1a0813e513d24e9fc5c7a010732c179eb5>`() const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`init<doxid-classov_1_1_runtime_attribute_1a85cfa598b9589c581cb1cdababf36cd6>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`merge<doxid-classov_1_1_runtime_attribute_1abbc804f43f52cd6ed54fab2b6c7b573b>`(const :ref:`ov::NodeVector<doxid-namespaceov_1a750141ccb27d75af03e91a5295645c7f>`& nodes) const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :ref:`merge<doxid-classov_1_1_runtime_attribute_1a034010091b62f617c14e4576fcf56cb2>`(const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& outputs) const;
		virtual std::string :ref:`to_string<doxid-classov_1_1_runtime_attribute_1aaf017b973a9eb4ef7e5d8466cf385ee4>`() const;
		virtual bool :ref:`visit_attributes<doxid-classov_1_1_runtime_attribute_1abacd4929156e317cdb0c74d9cc714025>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		bool :ref:`visit_attributes<doxid-classov_1_1_runtime_attribute_1ad41560d786103ecad79977ce84e68912>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor) const;

.. _details-classov_1_1_old_api_map_order:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`OldApiMapOrder <doxid-classov_1_1_old_api_map_order>` class represents runtime info attribute that stores order of the transpose that is required for obtaining IR in old API.

:ref:`OldApiMapOrder <doxid-classov_1_1_old_api_map_order>` stores the following information. Parameter: Order of the transpose which should be applied to Parameter with old API layout to obtain Parameter with new API layout.

Result: Order of the transpose which should be applied to Result with new API layout to obtain Result with old API layout.

Construction
------------

.. _doxid-classov_1_1_old_api_map_order_1a80a3da1c2665ef3e39037ee44b6c333e:
.. index:: pair: function; OldApiMapOrder

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OldApiMapOrder()

A default constructor

.. _doxid-classov_1_1_old_api_map_order_1a741964829bf1728ef20135c62c477a49:
.. index:: pair: function; OldApiMapOrder

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OldApiMapOrder(const std::vector<uint64_t>& value)

Constructs a new :ref:`OldApiMapOrder <doxid-classov_1_1_old_api_map_order>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The object that stores values of :ref:`OldApiMapOrder <doxid-classov_1_1_old_api_map_order>`.


