.. index:: pair: namespace; ov::frontend
.. _doxid-namespaceov_1_1frontend:

namespace ov::frontend
======================

.. toctree::
	:hidden:

	ExtensionHolder <structov_1_1frontend_1_1ExtensionHolder.rst>
	FrontEndPluginInfo <structov_1_1frontend_1_1FrontEndPluginInfo.rst>
	ConversionExtension <classov_1_1frontend_1_1ConversionExtension.rst>
	ConversionExtensionBase <classov_1_1frontend_1_1ConversionExtensionBase.rst>
	DecoderTransformationExtension <classov_1_1frontend_1_1DecoderTransformationExtension.rst>
	FWVisitor <classov_1_1frontend_1_1FWVisitor.rst>
	FrontEnd <classov_1_1frontend_1_1FrontEnd.rst>
	FrontEndManager <classov_1_1frontend_1_1FrontEndManager.rst>
	GeneralFailure <classov_1_1frontend_1_1GeneralFailure.rst>
	InitializationFailure <classov_1_1frontend_1_1InitializationFailure.rst>
	InputModel <classov_1_1frontend_1_1InputModel.rst>
	JsonConfigExtension <classov_1_1frontend_1_1JsonConfigExtension.rst>
	JsonTransformationExtension <classov_1_1frontend_1_1JsonTransformationExtension.rst>
	NodeContext <classov_1_1frontend_1_1NodeContext.rst>
	NotImplementedFailure <classov_1_1frontend_1_1NotImplementedFailure.rst>
	OpConversionFailure <classov_1_1frontend_1_1OpConversionFailure.rst>
	OpConversionFunction <classov_1_1frontend_1_1OpConversionFunction.rst>
	OpExtensionBase <classov_1_1frontend_1_1OpExtensionBase.rst>
	OpValidationFailure <classov_1_1frontend_1_1OpValidationFailure.rst>
	Place <classov_1_1frontend_1_1Place.rst>
	ProgressReporterExtension <classov_1_1frontend_1_1ProgressReporterExtension.rst>
	TelemetryExtension <classov_1_1frontend_1_1TelemetryExtension.rst>

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace frontend {

	// typedefs

	typedef :ref:`ov::frontend::OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base>`<:ref:`ov::frontend::ConversionExtension<doxid-classov_1_1frontend_1_1_conversion_extension>`, OVOpType> :target:`OpExtension<doxid-namespaceov_1_1frontend_1a45d917c50dc6fac04e27a273bcf02064>`;
	typedef std::function<:ref:`FrontEnd::Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>`()> :target:`FrontEndFactory<doxid-namespaceov_1_1frontend_1ac5dc4ee362133b5e540e65cb606567f0>`;
	typedef uint64_t :ref:`FrontEndVersion<doxid-namespaceov_1_1frontend_1acadb03c781dbcd071eb0fc58b5f94551>`;
	typedef std::function<:ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`(const :ref:`NodeContext<doxid-classov_1_1frontend_1_1_node_context>`&)> :target:`CreatorFunction<doxid-namespaceov_1_1frontend_1aa8aab3222c4b95dbd11746783646cb3c>`;
	typedef std::function<std::map<std::string, :ref:`OutputVector<doxid-namespaceov_1a0a3841455b82c164b1b04b61a9c7c560>`>(const :ref:`NodeContext<doxid-classov_1_1frontend_1_1_node_context>`&)> :target:`CreatorFunctionNamed<doxid-namespaceov_1_1frontend_1a9a8b976c6b2003da87f8d8dfedaa99f0>`;

	// structs

	struct :ref:`ExtensionHolder<doxid-structov_1_1frontend_1_1_extension_holder>`;
	struct :ref:`FrontEndPluginInfo<doxid-structov_1_1frontend_1_1_front_end_plugin_info>`;

	// classes

	class :ref:`ConversionExtension<doxid-classov_1_1frontend_1_1_conversion_extension>`;
	class :ref:`ConversionExtensionBase<doxid-classov_1_1frontend_1_1_conversion_extension_base>`;
	class :ref:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`;
	class :ref:`FWVisitor<doxid-classov_1_1frontend_1_1_f_w_visitor>`;
	class :ref:`FrontEnd<doxid-classov_1_1frontend_1_1_front_end>`;
	class :ref:`FrontEndManager<doxid-classov_1_1frontend_1_1_front_end_manager>`;
	class :ref:`GeneralFailure<doxid-classov_1_1frontend_1_1_general_failure>`;
	class :ref:`InitializationFailure<doxid-classov_1_1frontend_1_1_initialization_failure>`;
	class :ref:`InputModel<doxid-classov_1_1frontend_1_1_input_model>`;
	class :ref:`JsonConfigExtension<doxid-classov_1_1frontend_1_1_json_config_extension>`;
	class :ref:`JsonTransformationExtension<doxid-classov_1_1frontend_1_1_json_transformation_extension>`;
	class :ref:`NodeContext<doxid-classov_1_1frontend_1_1_node_context>`;
	class :ref:`NotImplementedFailure<doxid-classov_1_1frontend_1_1_not_implemented_failure>`;
	class :ref:`OpConversionFailure<doxid-classov_1_1frontend_1_1_op_conversion_failure>`;
	class :ref:`OpConversionFunction<doxid-classov_1_1frontend_1_1_op_conversion_function>`;
	template <typename BaseConversionType>
	class :ref:`OpExtensionBase<BaseConversionType, void><doxid-classov_1_1frontend_1_1_op_extension_base_3_01_base_conversion_type_00_01void_01_4>`;
	template <typename BaseConversionType, typename OVOpType = void>
	class :ref:`OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base>`;
	class :ref:`OpValidationFailure<doxid-classov_1_1frontend_1_1_op_validation_failure>`;
	class :ref:`Place<doxid-classov_1_1frontend_1_1_place>`;
	class :ref:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension>`;
	class :ref:`TelemetryExtension<doxid-classov_1_1frontend_1_1_telemetry_extension>`;

	// global functions

	const :ref:`ov::OpSet<doxid-classov_1_1_op_set>`& :ref:`get_opset_by_name<doxid-namespaceov_1_1frontend_1ac6789e8b813b81bd91003c4c847aebf3>`(const std::string& opset_name);

	} // namespace frontend
.. _details-namespaceov_1_1frontend:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Typedefs
--------

.. _doxid-namespaceov_1_1frontend_1acadb03c781dbcd071eb0fc58b5f94551:
.. index:: pair: typedef; FrontEndVersion

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef uint64_t FrontEndVersion

Each frontend plugin is responsible to export GetAPIVersion function returning version of frontend API used for this plugin If version is not matched with OV_FRONTEND_API_VERSION - plugin will not be loaded by :ref:`FrontEndManager <doxid-classov_1_1frontend_1_1_front_end_manager>`.

Global Functions
----------------

.. _doxid-namespaceov_1_1frontend_1ac6789e8b813b81bd91003c4c847aebf3:
.. index:: pair: function; get_opset_by_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`ov::OpSet<doxid-classov_1_1_op_set>`& get_opset_by_name(const std::string& opset_name)

The helper function to return an instance of :ref:`OpSet <doxid-classov_1_1_op_set>` class initialized with operations from provided opset by name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- opset_name

		- Opset name (opsetN) to initialize :ref:`OpSet <doxid-classov_1_1_op_set>` class.

