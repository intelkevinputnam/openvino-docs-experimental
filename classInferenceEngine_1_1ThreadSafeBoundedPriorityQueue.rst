.. index:: pair: class; InferenceEngine::ThreadSafeBoundedPriorityQueue
.. _doxid-class_inference_engine_1_1_thread_safe_bounded_priority_queue:

class InferenceEngine::ThreadSafeBoundedPriorityQueue
=====================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_thread_safe_containers.hpp>
	
	template <typename T>
	class ThreadSafeBoundedPriorityQueue
	{
	public:
		// methods
	
		bool :target:`try_push<doxid-class_inference_engine_1_1_thread_safe_bounded_priority_queue_1abecaf97643ed82bd4186e0ce90456743>`(T&& value);
		bool :target:`try_pop<doxid-class_inference_engine_1_1_thread_safe_bounded_priority_queue_1ae24f7e458eb6f123a121ceb8ecdd1c67>`(T& value);
		void :target:`set_capacity<doxid-class_inference_engine_1_1_thread_safe_bounded_priority_queue_1abf0a33255a6fff570103f844ac22d463>`(std::size_t newCapacity);
	};

