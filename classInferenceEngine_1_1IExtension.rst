.. index:: pair: class; InferenceEngine::IExtension
.. _doxid-class_inference_engine_1_1_i_extension:

class InferenceEngine::IExtension
=================================



Overview
~~~~~~~~

This class is the main extension interface. :ref:`More...<details-class_inference_engine_1_1_i_extension>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iextension.h>
	
	class IExtension: public std::enable_shared_from_this< IExtension >
	{
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

	protected:
	};

	// direct descendants

	class :ref:`Extension<doxid-class_inference_engine_1_1_extension>`;
.. _details-class_inference_engine_1_1_i_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class is the main extension interface.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_extension_1aa8a57e8761e4f30545c0a2d6c1224af2:
.. index:: pair: function; getOpSets

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, :ref:`ngraph::OpSet<doxid-classngraph_1_1_op_set>`> getOpSets()

Returns operation sets This method throws an exception if it was not implemented.



.. rubric:: Returns:

map of opset name to opset

.. _doxid-class_inference_engine_1_1_i_extension_1a9b017df21c79d4a4cbc4a6db62fb760e:
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

.. _doxid-class_inference_engine_1_1_i_extension_1a638fa9798b9c50af6a753f77f0a890a1:
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

.. _doxid-class_inference_engine_1_1_i_extension_1a1b679d6267b4fd85873d9f57080bfa48:
.. index:: pair: function; Unload

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Unload() = 0

Cleans resources up.

.. _doxid-class_inference_engine_1_1_i_extension_1afd076674a0ecf5703a6c8046abaef508:
.. index:: pair: function; GetVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void GetVersion(const :ref:`InferenceEngine::Version<doxid-struct_inference_engine_1_1_version>` \*& versionInfo) const = 0

Gets extension version information and stores in versionInfo.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- versionInfo

		- Pointer to version info, will be set by plugin

.. _doxid-class_inference_engine_1_1_i_extension_1a623bd95b9366ff8699e7b17dede5d5ad:
.. index:: pair: function; Release

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Release()

Implements deprecated API.


