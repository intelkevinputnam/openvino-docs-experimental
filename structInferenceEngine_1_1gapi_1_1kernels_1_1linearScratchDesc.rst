.. index:: pair: struct; InferenceEngine::gapi::kernels::linearScratchDesc
.. _doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc:

struct InferenceEngine::gapi::kernels::linearScratchDesc
========================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename T, typename Mapper, int chanNum>
	struct linearScratchDesc
	{
		// typedefs
	
		typedef typename Mapper::alpha_type :target:`alpha_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a794b90dac042487a1e668446ec51b6de>`;
		typedef typename Mapper::index_type :target:`index_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a6fbb1cf7b43d7eb2d459cdeb3ae75f2c>`;

		// fields
	
		:ref:`alpha_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a794b90dac042487a1e668446ec51b6de>` \* :target:`alpha<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1ae6d9ab705a6c7d99fbae19b8bf392e03>`;
		:ref:`alpha_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a794b90dac042487a1e668446ec51b6de>` \* :target:`clone<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a1e8d860b2dbee7b86b753f0d1a5141b8>`;
		:ref:`index_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a6fbb1cf7b43d7eb2d459cdeb3ae75f2c>` \* :target:`mapsx<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1abcf3e9b02e1f6ebc55575846d5ad8deb>`;
		:ref:`alpha_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a794b90dac042487a1e668446ec51b6de>` \* :target:`beta<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a2c7b26651c4c1a0a00e158def240d8d3>`;
		:ref:`index_t<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a6fbb1cf7b43d7eb2d459cdeb3ae75f2c>` \* :target:`mapsy<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a3b066eef30ebd3dde6f386899bea1d14>`;
		T \* :target:`tmp<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a7cea9ba4c0347e8fd2ea13be7f9febd9>`;

		// construction
	
		:target:`linearScratchDesc<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1acaea2852ef34d0551e56e385298f3c0b>`(int, int, int outW, int outH, void \* data);

		// methods
	
		static int :target:`bufSize<doxid-struct_inference_engine_1_1gapi_1_1kernels_1_1linear_scratch_desc_1a680a3df802d7a5ad52c6b841d3062286>`(int inW, int, int outW, int outH, int lpi);
	};

