.. index:: pair: class; ov::OpExtension
.. _doxid-classov_1_1_op_extension:

class ov::OpExtension
=====================



Overview
~~~~~~~~

The default implementation of OpenVINO operation extensions. :ref:`More...<details-classov_1_1_op_extension>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <op_extension.hpp>
	
	template <class T>
	class OpExtension: public :ref:`ov::BaseOpExtension<doxid-classov_1_1_base_op_extension>`
	{
	public:
		// methods
	
		virtual const :ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_op_extension_1aaf384c172124c7ad4524b9102832e1b9>`() const;
	
		virtual :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :ref:`create<doxid-classov_1_1_op_extension_1ad46ab05266665c316bfe928254c64ff9>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs,
			:ref:`ov::AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor
			) const;
	
		virtual std::vector<:ref:`ov::Extension::Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`> :ref:`get_attached_extensions<doxid-classov_1_1_op_extension_1a0bbb313601ee50298d099760a4a002e0>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;
		typedef std::shared_ptr<:ref:`BaseOpExtension<doxid-classov_1_1_base_op_extension>`> :ref:`Ptr<doxid-classov_1_1_base_op_extension_1a65ffb8a33d7773e3474e716b965f51b4>`;

		// methods
	
		virtual const :ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :ref:`get_type_info<doxid-classov_1_1_base_op_extension_1aaa88ab372ae10181c8bae19d560a60ca>`() const = 0;
	
		virtual :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` :ref:`create<doxid-classov_1_1_base_op_extension_1aee9da36ffe82a00fa423b26cb042f20f>`(
			const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs,
			:ref:`ov::AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor
			) const = 0;
	
		virtual std::vector<:ref:`ov::Extension::Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`> :ref:`get_attached_extensions<doxid-classov_1_1_base_op_extension_1a818f0d03d775555c8bfa2075c849efd9>`() const = 0;

.. _details-classov_1_1_op_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

The default implementation of OpenVINO operation extensions.

Methods
-------

.. _doxid-classov_1_1_op_extension_1aaf384c172124c7ad4524b9102832e1b9:
.. index:: pair: function; get_type_info

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const :ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& get_type_info() const

Returns the type info of operation.



.. rubric:: Returns:

:ref:`ov::DiscreteTypeInfo <doxid-structov_1_1_discrete_type_info>`

.. _doxid-classov_1_1_op_extension_1ad46ab05266665c316bfe928254c64ff9:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>` create(
		const :ref:`ov::OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`& inputs,
		:ref:`ov::AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor
		) const

Method creates an OpenVINO operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- vector of input ports

	*
		- visitor

		- attribute visitor which allows to read necessaty arguments



.. rubric:: Returns:

vector of output ports

.. _doxid-classov_1_1_op_extension_1a0bbb313601ee50298d099760a4a002e0:
.. index:: pair: function; get_attached_extensions

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`ov::Extension::Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`> get_attached_extensions() const

Returns extensions that should be registered together with this extension class object.

Attached extensions may include frontend extensions that OpenVINO op to framework ops or necessary transformations that should be applied to the network which consist of target op.



.. rubric:: Returns:


