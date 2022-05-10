.. index:: pair: class; ngraph::FusedNames
.. _doxid-classngraph_1_1_fused_names:

class ngraph::FusedNames
========================



Overview
~~~~~~~~

FusedName class represents runtime info attribute that stores all operation names that was fully or partially fused into node. :ref:`More...<details-classngraph_1_1_fused_names>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <fused_names_attribute.hpp>
	
	class FusedNames: public :ref:`ov::RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`
	{
	public:
		// construction
	
		:ref:`FusedNames<doxid-classngraph_1_1_fused_names_1aa5d9fe0096b0de6339148d461a2e2301>`();
		:ref:`FusedNames<doxid-classngraph_1_1_fused_names_1af2bc9e0d648815658b38e25d5af9405d>`(const std::string& name);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1_fused_names_1a21bc8299044377cc574446b1a2282401>`("fused_names", "0");
		void :ref:`fuseWith<doxid-classngraph_1_1_fused_names_1ad1043441cccbacb7dada6d4ea16a3474>`(const FusedNames& names);
		std::string :ref:`getNames<doxid-classngraph_1_1_fused_names_1a5912785e83394b2af77fa2a19eac2258>`() const;
		std::vector<std::string> :ref:`getVectorNames<doxid-classngraph_1_1_fused_names_1a53e8488736fae0f71ab3e500ef39433f>`() const;
		:ref:`ov::Any<doxid-classov_1_1_any>` :target:`merge<doxid-classngraph_1_1_fused_names_1af26a792742f37d5f252236fabc0845cd>`(const :ref:`ngraph::NodeVector<doxid-classngraph_1a7b4a05064df831b05909c6535f6874c5>`& nodes) const;
		:ref:`ov::Any<doxid-classov_1_1_any>` :target:`init<doxid-classngraph_1_1_fused_names_1a267da987ff0c28af5ff0f1bbcb4e97a3>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node) const;
		bool :target:`visit_attributes<doxid-classngraph_1_1_fused_names_1ab2301cc88eede0dcd875132807e9e40e>`(AttributeVisitor& visitor);
		virtual std::string :target:`to_string<doxid-classngraph_1_1_fused_names_1a07a426819375a794f9aab84765949c42>`() const;
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

.. _details-classngraph_1_1_fused_names:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

FusedName class represents runtime info attribute that stores all operation names that was fully or partially fused into node.

Construction
------------

.. _doxid-classngraph_1_1_fused_names_1aa5d9fe0096b0de6339148d461a2e2301:
.. index:: pair: function; FusedNames

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FusedNames()

A default constructor

.. _doxid-classngraph_1_1_fused_names_1af2bc9e0d648815658b38e25d5af9405d:
.. index:: pair: function; FusedNames

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FusedNames(const std::string& name)

Constructs a new object consisting of a single name \*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- The name

Methods
-------

.. _doxid-classngraph_1_1_fused_names_1ad1043441cccbacb7dada6d4ea16a3474:
.. index:: pair: function; fuseWith

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void fuseWith(const FusedNames& names)

Unites current set of already fused names with another :ref:`FusedNames <doxid-classngraph_1_1_fused_names>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- names

		- Another object to fuse with

.. _doxid-classngraph_1_1_fused_names_1a5912785e83394b2af77fa2a19eac2258:
.. index:: pair: function; getNames

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getNames() const

return string with operation names separated by coma in alphabetical order

.. _doxid-classngraph_1_1_fused_names_1a53e8488736fae0f71ab3e500ef39433f:
.. index:: pair: function; getVectorNames

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> getVectorNames() const

return vector of fused names sorted in alphabetical order



.. rubric:: Returns:

vector if strings


