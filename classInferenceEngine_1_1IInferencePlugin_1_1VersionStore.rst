.. index:: pair: class; InferenceEngine::IInferencePlugin::VersionStore
.. _doxid-class_inference_engine_1_1_i_inference_plugin_1_1_version_store:

class InferenceEngine::IInferencePlugin::VersionStore
=====================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class VersionStore: public :ref:`InferenceEngine::Version<doxid-struct_inference_engine_1_1_version>`
	{
	public:
		// construction
	
		:target:`VersionStore<doxid-class_inference_engine_1_1_i_inference_plugin_1_1_version_store_1a1dad3b55485e92debb9e91b8831899af>`();
		:target:`VersionStore<doxid-class_inference_engine_1_1_i_inference_plugin_1_1_version_store_1a443f2550a7d3b510f9213b2eb6e06b21>`(const :ref:`Version<doxid-struct_inference_engine_1_1_version>`& v);

		// methods
	
		VersionStore& :target:`operator =<doxid-class_inference_engine_1_1_i_inference_plugin_1_1_version_store_1ab853f95b8e52f26106f98df22f624a57>` (const VersionStore& v);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// structs
	
		struct :ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version>`;

		// fields
	
		:ref:`ApiVersion<doxid-struct_inference_engine_1_1_version_1_1_api_version>` :ref:`apiVersion<doxid-struct_inference_engine_1_1_version_1a67f6a06d9210b1b080e2547ef03f3859>`;
		const char \* :ref:`buildNumber<doxid-struct_inference_engine_1_1_version_1aa5f87bb79d0028b64bba724f67c02ec4>`;
		const char \* :ref:`description<doxid-struct_inference_engine_1_1_version_1acce46690f8fdd1b8ecf29c6915f8528b>`;


