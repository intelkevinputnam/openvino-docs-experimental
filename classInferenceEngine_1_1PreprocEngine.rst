.. index:: pair: class; InferenceEngine::PreprocEngine
.. _doxid-class_inference_engine_1_1_preproc_engine:

class InferenceEngine::PreprocEngine
====================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_preprocess_gapi.hpp>
	
	class PreprocEngine
	{
	public:
		// methods
	
		void :target:`preprocessWithGAPI<doxid-class_inference_engine_1_1_preproc_engine_1a4e665603aaff037721f034926b5578ca>`(
			const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& inBlob,
			:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& outBlob,
			const :ref:`ResizeAlgorithm<doxid-namespace_inference_engine_1a805a09efb0e7b327ffa078f8d02222e9>`& algorithm,
			:ref:`ColorFormat<doxid-namespace_inference_engine_1a5ee5ca7708cc67a9a0becc2593d0558a>` in_fmt,
			bool omp_serial,
			int batch_size = -1
			);
	
		static void :target:`checkApplicabilityGAPI<doxid-class_inference_engine_1_1_preproc_engine_1a1f0e74bd2d5ba54e54e5946012f15eff>`(const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& src, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& dst);
		static int :target:`getCorrectBatchSize<doxid-class_inference_engine_1_1_preproc_engine_1a327e55777bd97ca70e9423f98aa5f9a8>`(int batch_size, const :ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`& roiBlob);
	};

