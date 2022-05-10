.. index:: pair: namespace; InferenceEngine::gapi
.. _doxid-namespace_inference_engine_1_1gapi:

namespace InferenceEngine::gapi
===============================

.. toctree::
	:hidden:

	kernels <namespaceInferenceEngine_1_1gapi_1_1kernels.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace gapi {

	// namespaces

	namespace :ref:`InferenceEngine::gapi::kernels<doxid-namespace_inference_engine_1_1gapi_1_1kernels>`;
		namespace :ref:`InferenceEngine::gapi::kernels::areaDownscale32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_downscale32f>`;
		namespace :ref:`InferenceEngine::gapi::kernels::areaDownscale8u<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_downscale8u>`;
		namespace :ref:`InferenceEngine::gapi::kernels::areaUpscale<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_upscale>`;
		namespace :ref:`InferenceEngine::gapi::kernels::areaUpscale32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1area_upscale32f>`;
		namespace :ref:`InferenceEngine::gapi::kernels::avx<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx>`;
		namespace :ref:`InferenceEngine::gapi::kernels::avx512<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1avx512>`;
		namespace :ref:`InferenceEngine::gapi::kernels::linear<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1linear>`;
		namespace :ref:`InferenceEngine::gapi::kernels::linear32f<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1linear32f>`;
		namespace :ref:`InferenceEngine::gapi::kernels::neon<doxid-namespace_inference_engine_1_1gapi_1_1kernels_1_1neon>`;

	// typedefs

	typedef cv::gapi::own::Size :target:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`;
	typedef std::tuple<cv::GMat, cv::GMat> :target:`GMat2<doxid-namespace_inference_engine_1_1gapi_1a8ffde0e347b5aaba1aa145788906e3a2>`;
	typedef std::tuple<cv::GMat, cv::GMat, cv::GMat> :target:`GMat3<doxid-namespace_inference_engine_1_1gapi_1a8073b6a65a3e1f73c148fe8a6033e5bb>`;
	typedef std::tuple<cv::GMat, cv::GMat, cv::GMat, cv::GMat> :target:`GMat4<doxid-namespace_inference_engine_1_1gapi_1ab005904b1493309cbc8a708406b89017>`;

	// global functions

	cv::gapi::GKernelPackage :target:`preprocKernels<doxid-namespace_inference_engine_1_1gapi_1a6b44ed6c2d53ae6385e3aec508231137>`();

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aa790e0daed7c378173a497fee4adbbbf>`(
		ChanToPlane,
		<cv::GMat(cv::GMat, int)>,
		"com.intel.ie.chan_to_plane"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aec01a0c870f54e5df17b39541e58be30>`(
		ScalePlane,
		<cv::GMat(cv::GMat, int, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_plane"
		);

	:target:`G_TYPED_KERNEL_M<doxid-namespace_inference_engine_1_1gapi_1a35fd3f4b5e8696bfc08d7ad973e441d4>`(
		ScalePlanes,
		<:ref:`GMat3<doxid-namespace_inference_engine_1_1gapi_1a8073b6a65a3e1f73c148fe8a6033e5bb>`(cv::GMat, int, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_planes"
		);

	:target:`G_TYPED_KERNEL_M<doxid-namespace_inference_engine_1_1gapi_1a41a0d2be82a8be8d0b5d7eee7aa4b69b>`(
		ScalePlanes4,
		<:ref:`GMat4<doxid-namespace_inference_engine_1_1gapi_1ab005904b1493309cbc8a708406b89017>`(cv::GMat, int, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_planes4"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aff517b8f8317a337bef72d24fbab0d27>`(
		ScalePlane8u,
		<cv::GMat(cv::GMat, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_plane_8u"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a9e94a2b75a98b2f36230ac7d9b92b8cd>`(
		ScalePlane32f,
		<cv::GMat(cv::GMat, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_plane_32f"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a1ca996e9fe9fcfd7472c4b8bf833a0b6>`(
		UpscalePlaneArea8u,
		<cv::GMat(cv::GMat, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.upscale_plane_area_8u"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1ad9120c410a9bb0cb89522a5c45a00e62>`(
		UpscalePlaneArea32f,
		<cv::GMat(cv::GMat, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.upscale_plane_area_32f"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a5ffa1151bc8401253a3a183105762e54>`(
		ScalePlaneArea8u,
		<cv::GMat(cv::GMat, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_plane_area_8u"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aa46edd37cb25f9198aef78342ed6bef6>`(
		ScalePlaneArea32f,
		<cv::GMat(cv::GMat, :ref:`Size<doxid-namespace_inference_engine_1_1gapi_1abfae352fcf3162d0b3a795593049bd5b>`, int)>,
		"com.intel.ie.scale_plane_area_32f"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aaf24cd25f01179e21114bb658358d661>`(Merge2, <cv::GMat(cv::GMat, cv::GMat)>, "com.intel.ie.merge2");

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1af11a6a101efb5d0b1c429df14a576e3f>`(
		Merge3,
		<cv::GMat(cv::GMat, cv::GMat, cv::GMat)>,
		"com.intel.ie.merge3"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a9e753e652e0031e69e112fc06b89904f>`(
		Merge4,
		<cv::GMat(cv::GMat, cv::GMat, cv::GMat, cv::GMat)>,
		"com.intel.ie.merge4"
		);

	:target:`G_TYPED_KERNEL_M<doxid-namespace_inference_engine_1_1gapi_1a5d5171a9bc12b2a70d13ca317e11a512>`(Split2, <:ref:`GMat2<doxid-namespace_inference_engine_1_1gapi_1a8ffde0e347b5aaba1aa145788906e3a2>`(cv::GMat)>, "com.intel.ie.split2");
	:target:`G_TYPED_KERNEL_M<doxid-namespace_inference_engine_1_1gapi_1a6a6f308ddeed3525790d53121200697a>`(Split3, <:ref:`GMat3<doxid-namespace_inference_engine_1_1gapi_1a8073b6a65a3e1f73c148fe8a6033e5bb>`(cv::GMat)>, "com.intel.ie.split3");
	:target:`G_TYPED_KERNEL_M<doxid-namespace_inference_engine_1_1gapi_1a4c86e79e57bc214fc503447c64c02558>`(Split4, <:ref:`GMat4<doxid-namespace_inference_engine_1_1gapi_1ab005904b1493309cbc8a708406b89017>`(cv::GMat)>, "com.intel.ie.split4");

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aa6986972e5d0611df5d08124960e53d0>`(
		NV12toRGB,
		<cv::GMat(cv::GMat, cv::GMat)>,
		"com.intel.ie.nv12torgb"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a373b2720aefb5ea41331908320e02f1e>`(
		I420toRGB,
		<cv::GMat(cv::GMat, cv::GMat, cv::GMat)>,
		"com.intel.ie.i420torgb"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a872f944ad782b43aa0e156c25ea5264a>`(
		ConvertDepth,
		<cv::GMat(cv::GMat, int depth)>,
		"com.intel.ie.ConvertDepth"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1aa479f49cacba8dda5c82de4c0c7b18cf>`(
		GSubC,
		<cv::GMat(cv::GMat, cv::GScalar, int)>,
		"com.intel.ie.math.subC"
		);

	:target:`G_TYPED_KERNEL<doxid-namespace_inference_engine_1_1gapi_1a603d7b635abf7d4261c353f9b68d518d>`(
		GDivC,
		<cv::GMat(cv::GMat, cv::GScalar, double, int)>,
		"com.intel.ie.math.divC"
		);

	} // namespace gapi
