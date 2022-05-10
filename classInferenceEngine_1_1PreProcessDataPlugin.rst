.. index:: pair: class; InferenceEngine::PreProcessDataPlugin
.. _doxid-class_inference_engine_1_1_pre_process_data_plugin:

class InferenceEngine::PreProcessDataPlugin
===========================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess_data.hpp>
	
	class PreProcessDataPlugin
	{
	public:
		// methods
	
		void :target:`setRoiBlob<doxid-class_inference_engine_1_1_pre_process_data_plugin_1a13fe2d4c08211b20b83970dbbe6c3d46>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& blob);
		:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :target:`getRoiBlob<doxid-class_inference_engine_1_1_pre_process_data_plugin_1a3e9c15e13d7d84ef5d427cbe6053b433>`() const;
	
		void :target:`execute<doxid-class_inference_engine_1_1_pre_process_data_plugin_1a7031da057e1c76e4f431d09a0e59a060>`(
			:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& preprocessedBlob,
			const :ref:`PreProcessInfo<doxid-class_inference_engine_1_1_pre_process_info>`& info,
			bool serial,
			int batchSize = -1
			);
	
		void :target:`isApplicable<doxid-class_inference_engine_1_1_pre_process_data_plugin_1a6e9fb6c046fad59da6da79538085f8e2>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& src, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& dst);
	};

