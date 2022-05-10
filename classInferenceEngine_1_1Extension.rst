.. index:: pair: class; InferenceEngine::Extension
.. _doxid-class_inference_engine_1_1_extension:

class InferenceEngine::Extension
================================



Overview
~~~~~~~~

This class is a C++ helper to work with objects created using extensions. :ref:`More...<details-class_inference_engine_1_1_extension>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_extension.h>
	
	class Extension: public :ref:`InferenceEngine::IExtension<doxid-class_inference_engine_1_1_i_extension>`
	{
	public:
		// construction
	
		:ref:`Extension<doxid-class_inference_engine_1_1_extension_1a04595462ee0b12ec2f2101e5ab602bac>`(const std::string& name);

		// methods
	
		virtual void :ref:`GetVersion<doxid-class_inference_engine_1_1_extension_1a0bbf32861d5399660ee426dbcf77f1c5>`(const :ref:`InferenceEngine::Version<doxid-struct_inference_engine_1_1_version>` \*& versionInfo) const;
		virtual void :ref:`Unload<doxid-class_inference_engine_1_1_extension_1a196c01759d2d939baa15b227c25aa469>`();
		virtual std::map<std::string, :ref:`ngraph::OpSet<doxid-classngraph_1_1_op_set>`> :ref:`getOpSets<doxid-class_inference_engine_1_1_extension_1a581c9d724a75a30e6be6018ed81afbce>`();
		virtual std::vector<std::string> :ref:`getImplTypes<doxid-class_inference_engine_1_1_extension_1abfed209a40e95f5e07d922e38a957c1c>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	
		virtual :ref:`ILayerImpl::Ptr<doxid-class_inference_engine_1_1_i_layer_impl_1a83cfc1d50968aa3dbdd05fac0a55c28d>` :ref:`getImplementation<doxid-class_inference_engine_1_1_extension_1a5db8ee89f21919cef7dbd28866f2e9cf>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
			const std::string& implType
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual std::map<std::string, :ref:`ngraph::OpSet<doxid-classngraph_1_1_op_set>`> :ref:`getOpSets<doxid-class_inference_engine_1_1_i_extension_1aa8a57e8761e4f30545c0a2d6c1224af2>`();
		virtual std::vector<std::string> :ref:`getImplTypes<doxid-class_inference_engine_1_1_i_extension_1a9b017df21c79d4a4cbc4a6db62fb760e>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	
		virtual :ref:`ILayerImpl::Ptr<doxid-class_inference_engine_1_1_i_layer_impl_1a83cfc1d50968aa3dbdd05fac0a55c28d>` :ref:`getImplementation<doxid-class_inference_engine_1_1_i_extension_1a638fa9798b9c50af6a753f77f0a890a1>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
			const std::string& implType
			);
	
		virtual void :ref:`Unload<doxid-class_inference_engine_1_1_i_extension_1a1b679d6267b4fd85873d9f57080bfa48>`() = 0;
		virtual void :ref:`GetVersion<doxid-class_inference_engine_1_1_i_extension_1afd076674a0ecf5703a6c8046abaef508>`(const :ref:`InferenceEngine::Version<doxid-struct_inference_engine_1_1_version>` \*& versionInfo) const = 0;
		virtual void :ref:`Release<doxid-class_inference_engine_1_1_i_extension_1a623bd95b9366ff8699e7b17dede5d5ad>`();

.. _details-class_inference_engine_1_1_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is a C++ helper to work with objects created using extensions.

Construction
------------

.. _doxid-class_inference_engine_1_1_extension_1a04595462ee0b12ec2f2101e5ab602bac:
.. index:: pair: function; Extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Extension(const std::string& name)

Loads extension from a shared library.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Full or relative path to extension library

Methods
-------

.. _doxid-class_inference_engine_1_1_extension_1a0bbf32861d5399660ee426dbcf77f1c5:
.. index:: pair: function; GetVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void GetVersion(const :ref:`InferenceEngine::Version<doxid-struct_inference_engine_1_1_version>` \*& versionInfo) const

Gets the extension version information.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- versionInfo

		- A pointer to version info, set by the plugin

.. _doxid-class_inference_engine_1_1_extension_1a196c01759d2d939baa15b227c25aa469:
.. index:: pair: function; Unload

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Unload()

Cleans the resources up.

.. _doxid-class_inference_engine_1_1_extension_1a581c9d724a75a30e6be6018ed81afbce:
.. index:: pair: function; getOpSets

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, :ref:`ngraph::OpSet<doxid-classngraph_1_1_op_set>`> getOpSets()

Returns operation sets This method throws an exception if it was not implemented.



.. rubric:: Returns:

map of opset name to opset

.. _doxid-class_inference_engine_1_1_extension_1abfed209a40e95f5e07d922e38a957c1c:
.. index:: pair: function; getImplTypes

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::string> getImplTypes(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node)

Returns vector of implementation types.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- shared pointer to nGraph op



.. rubric:: Returns:

vector of strings

.. _doxid-class_inference_engine_1_1_extension_1a5db8ee89f21919cef7dbd28866f2e9cf:
.. index:: pair: function; getImplementation

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ILayerImpl::Ptr<doxid-class_inference_engine_1_1_i_layer_impl_1a83cfc1d50968aa3dbdd05fac0a55c28d>` getImplementation(
		const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
		const std::string& implType
		)

Returns implementation for specific nGraph op.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- shared pointer to nGraph op

	*
		- implType

		- implementation type



.. rubric:: Returns:

shared pointer to implementation


