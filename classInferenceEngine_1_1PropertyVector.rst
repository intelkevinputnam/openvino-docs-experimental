.. index:: pair: class; InferenceEngine::PropertyVector
.. _doxid-class_inference_engine_1_1_property_vector:

class InferenceEngine::PropertyVector
=====================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers_property.hpp>
	
	template <class T, int N = MAX_DIMS_NUMBER>
	class PropertyVector
	{
	public:
		// construction
	
		:target:`PropertyVector<doxid-class_inference_engine_1_1_property_vector_1aa9348ebbad0f960b7beb2de634d59472>`();
		:target:`PropertyVector<doxid-class_inference_engine_1_1_property_vector_1a44e160f0ba44f87a4a34ad6d55093cfb>`(size_t len, T val);
		:target:`PropertyVector<doxid-class_inference_engine_1_1_property_vector_1aa6375da41b5fca9b709b24a17abc550b>`(const std::vector<T>& values);
		:target:`PropertyVector<doxid-class_inference_engine_1_1_property_vector_1afd9b761eac6b72e5e6ad3e3492e58a86>`(std::initializer_list<int> init_list);

		// methods
	
		T& :ref:`at<doxid-class_inference_engine_1_1_property_vector_1a30775abe05792160c5fc430d8718f29a>`(int index);
		const T& :target:`operator []<doxid-class_inference_engine_1_1_property_vector_1abf4e72f1e802130b7863fceecc1708c8>` (size_t index) const;
		T& :target:`operator []<doxid-class_inference_engine_1_1_property_vector_1afb53af73bf7bc052b81b9fe27b489e04>` (size_t index);
		PropertyVector& :target:`operator =<doxid-class_inference_engine_1_1_property_vector_1a58555d49e67fe9e2afc4a2ca0304c564>` (const PropertyVector& src);
		bool :target:`operator ==<doxid-class_inference_engine_1_1_property_vector_1aebae8e6825e30e7d5f04233454103d4a>` (const PropertyVector& src) const;
		size_t :target:`size<doxid-class_inference_engine_1_1_property_vector_1a7b1b3e6a78a0ddec54da4eac36086ed6>`() const;
		void :target:`insert<doxid-class_inference_engine_1_1_property_vector_1ae248cc0fbcadcb62fc03b6e40f0e8bf7>`(size_t axis, const T& val);
		void :target:`remove<doxid-class_inference_engine_1_1_property_vector_1ad5aaa25ef9631d6396fa6d7f02a6e91d>`(size_t axis);
		void :target:`clear<doxid-class_inference_engine_1_1_property_vector_1a3942f2c86640b95feb061f8b683e0f62>`();
		bool :target:`exist<doxid-class_inference_engine_1_1_property_vector_1a5317cc99684c0a14309606eb4eb5af54>`(size_t axis) const;
	};
.. _details-class_inference_engine_1_1_property_vector:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-class_inference_engine_1_1_property_vector_1a30775abe05792160c5fc430d8718f29a:
.. index:: pair: function; at

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	T& at(int index)

allows access up-to capacity size



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- index

		- 



.. rubric:: Returns:


