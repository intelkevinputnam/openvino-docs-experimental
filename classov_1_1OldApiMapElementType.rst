.. index:: pair: class; ov::OldApiMapElementType
.. _doxid-classov_1_1_old_api_map_element_type:

class ov::OldApiMapElementType
==============================



Overview
~~~~~~~~

:ref:`OldApiMapElementType <doxid-classov_1_1_old_api_map_element_type>` class represents runtime info attribute that stores legacy type that is required for obtaining IR in old API. :ref:`More...<details-classov_1_1_old_api_map_element_type>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <old_api_map_element_type_attribute.hpp>
	
	class OldApiMapElementType: public :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`
	{
	public:
		// fields
	
		:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` :target:`value<doxid-classov_1_1_old_api_map_element_type_1a820bc90a596ff502fd7e280e80fbad60>`;

		// construction
	
		:ref:`OldApiMapElementType<doxid-classov_1_1_old_api_map_element_type_1a29785d805159cbbaaed35237dd932dba>`();
		:ref:`OldApiMapElementType<doxid-classov_1_1_old_api_map_element_type_1aaa53fec31d797ba122dc0fa2a2265621>`(const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`& value);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1_old_api_map_element_type_1a1c41fc58861aa0b8b8cd6257c5861396>`("old_api_map_element_type", "0");
		virtual bool :target:`is_copyable<doxid-classov_1_1_old_api_map_element_type_1abf4db76bcb4ed8a6ef86130220bb4b0d>`() const;
		virtual bool :target:`visit_attributes<doxid-classov_1_1_old_api_map_element_type_1a1bc99f87ba3c2b7ac1c178d97d9ef636>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
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

.. _details-classov_1_1_old_api_map_element_type:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`OldApiMapElementType <doxid-classov_1_1_old_api_map_element_type>` class represents runtime info attribute that stores legacy type that is required for obtaining IR in old API.

Construction
------------

.. _doxid-classov_1_1_old_api_map_element_type_1a29785d805159cbbaaed35237dd932dba:
.. index:: pair: function; OldApiMapElementType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OldApiMapElementType()

A default constructor

.. _doxid-classov_1_1_old_api_map_element_type_1aaa53fec31d797ba122dc0fa2a2265621:
.. index:: pair: function; OldApiMapElementType

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OldApiMapElementType(const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`& value)

Constructs a new :ref:`OldApiMapElementType <doxid-classov_1_1_old_api_map_element_type>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- The object that stores values of :ref:`OldApiMapElementType <doxid-classov_1_1_old_api_map_element_type>`.


