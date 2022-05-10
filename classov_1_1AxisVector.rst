.. index:: pair: class; ov::AxisVector
.. _doxid-classov_1_1_axis_vector:

class ov::AxisVector
====================



A vector of axes.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <axis_vector.hpp>
	
	class AxisVector: public std::vector< size_t >
	{
	public:
		// construction
	
		:target:`AxisVector<doxid-classov_1_1_axis_vector_1a1b14bdcd078873d48658c03ce434eeaf>`(const std::initializer_list<size_t>& axes);
		:target:`AxisVector<doxid-classov_1_1_axis_vector_1a05256f4b58543c3d854b43ae3fcc4efd>`(const std::vector<size_t>& axes);
		:target:`AxisVector<doxid-classov_1_1_axis_vector_1a0bd0116709c6cd948a70c97d01451d55>`(const AxisVector& axes);
		:target:`AxisVector<doxid-classov_1_1_axis_vector_1a6eb80ce5601afb1431524da789507264>`(size_t n);
	
		template <class InputIterator>
		:target:`AxisVector<doxid-classov_1_1_axis_vector_1a11a97436826ad2116a5532c5f4b86ee1>`(
			InputIterator first,
			InputIterator last
			);
	
		:target:`AxisVector<doxid-classov_1_1_axis_vector_1a61e851bee96b871bc94517181f0ebbf9>`();

		// methods
	
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` AxisVector& :target:`operator =<doxid-classov_1_1_axis_vector_1aec864b313fa2397959a8b6add93aa436>` (const AxisVector& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` AxisVector& :target:`operator =<doxid-classov_1_1_axis_vector_1ab63825f68234ff0ef0f1a769526ae5bf>` (AxisVector&& v);
	};

