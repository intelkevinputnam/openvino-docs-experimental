.. index:: pair: class; ov::Shape
.. _doxid-classov_1_1_shape:

class ov::Shape
===============



:ref:`Shape <doxid-classov_1_1_shape>` for a tensor.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <shape.hpp>
	
	class Shape: public std::vector< size_t >
	{
	public:
		// construction
	
		:target:`Shape<doxid-classov_1_1_shape_1af5e010b1c5ed4100dec00fde099a7c0e>`();
		:target:`Shape<doxid-classov_1_1_shape_1a208a3ef3ee230f0753d0f8f2d19eb50a>`(const std::initializer_list<size_t>& axis_lengths);
		:target:`Shape<doxid-classov_1_1_shape_1a1769ddc73ef3437c9ad24b303eb5f4ce>`(const std::vector<size_t>& axis_lengths);
		:target:`Shape<doxid-classov_1_1_shape_1a03d865c960f02f6abb29dc98821534a1>`(const Shape& axis_lengths);
		:target:`Shape<doxid-classov_1_1_shape_1aae34d5baff3b85494da8559e4572d860>`(size_t n, size_t initial_value = 0);
	
		template <class InputIterator>
		:target:`Shape<doxid-classov_1_1_shape_1ade676d08f707a9b8c0a0332eddc73c17>`(InputIterator first, InputIterator last);

		// methods
	
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` Shape& :target:`operator =<doxid-classov_1_1_shape_1ad7850ba9a9fdb555d0e2b5c8e5f1ad54>` (const Shape& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` Shape& :target:`operator =<doxid-classov_1_1_shape_1af5e29551eed57e07e1c21b09426606f1>` (Shape&& v);
	};

