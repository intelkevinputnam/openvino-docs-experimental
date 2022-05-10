.. index:: pair: class; InferenceEngine::ThreadSafeQueueWithSize
.. _doxid-class_inference_engine_1_1_thread_safe_queue_with_size:

class InferenceEngine::ThreadSafeQueueWithSize
==============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_thread_safe_containers.hpp>
	
	template <typename T>
	class ThreadSafeQueueWithSize
	{
	public:
		// methods
	
		void :target:`push<doxid-class_inference_engine_1_1_thread_safe_queue_with_size_1ae3953d7653ba263db52b5070471db797>`(T value);
		bool :target:`try_pop<doxid-class_inference_engine_1_1_thread_safe_queue_with_size_1adcc1d809a026896ddddf793aca4d7503>`(T& value);
		size_t :target:`size<doxid-class_inference_engine_1_1_thread_safe_queue_with_size_1af58c493b4033db64bbd06dc3e34b8297>`();
	};

