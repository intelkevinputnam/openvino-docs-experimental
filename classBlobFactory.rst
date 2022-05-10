.. index:: pair: class; BlobFactory
.. _doxid-class_blob_factory:

class BlobFactory
=================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <InferenceEngine::Precision::ePrecision precision>
	class BlobFactory
	{
	public:
		// typedefs
	
		typedef typename :ref:`InferenceEngine::PrecisionTrait<doxid-struct_inference_engine_1_1_precision_trait>`<precision>::value_type :target:`BlobType<doxid-class_blob_factory_1a6d1197868ec3470dcca8491d6de7325d>`;

		// methods
	
		static :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :target:`make<doxid-class_blob_factory_1aa9b427847c5a1b0a28024a6fe4f9fec0>`(const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc);
	
		static :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :target:`make<doxid-class_blob_factory_1aa9bbdb2d73f0135ce8c8ac00d0bec3c6>`(
			const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
			void \* ptr
			);
	
		static :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :target:`make<doxid-class_blob_factory_1ad173ac6e850377c78d407fc4f9132606>`(
			const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
			void \* ptr,
			const std::size_t size
			);
	
		static :ref:`InferenceEngine::Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>` :target:`make<doxid-class_blob_factory_1a0b4bb8a19ecc57251b5f6ea2bb62f7b2>`(
			const :ref:`InferenceEngine::TensorDesc<doxid-class_inference_engine_1_1_tensor_desc>`& desc,
			const std::shared_ptr<:ref:`InferenceEngine::IAllocator<doxid-class_inference_engine_1_1_i_allocator>`>& alloc
			);
	};

