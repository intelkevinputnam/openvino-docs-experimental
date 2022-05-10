.. index:: pair: class; ov::Strides
.. _doxid-classov_1_1_strides:

class ov::Strides
=================



:ref:`Strides <doxid-classov_1_1_strides>` for a tensor.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <strides.hpp>
	
	class Strides: public std::vector< size_t >
	{
	public:
		// construction
	
		:target:`Strides<doxid-classov_1_1_strides_1a57a0fd1aa1bd82548011bb753e03adb0>`();
		:target:`Strides<doxid-classov_1_1_strides_1a2f2d19dff4dc95972ae206850d8997af>`(const std::initializer_list<size_t>& axis_strides);
		:target:`Strides<doxid-classov_1_1_strides_1abf042f1073e78c85d8484fc8ea8f70cc>`(const std::vector<size_t>& axis_strides);
		:target:`Strides<doxid-classov_1_1_strides_1a2c7abb4522746330e600b10b533e74b4>`(const Strides& axis_strides);
		:target:`Strides<doxid-classov_1_1_strides_1a9d7bfbaffbb95ec81fae12f4e2f724dc>`(size_t n, size_t initial_value = 0);
	
		template <class InputIterator>
		:target:`Strides<doxid-classov_1_1_strides_1ac955a1bbc7a7ed20f8217ff02156794f>`(InputIterator first, InputIterator last);

		// methods
	
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` Strides& :target:`operator =<doxid-classov_1_1_strides_1a2514f56ffb9ea051560d10c550ae852e>` (const Strides& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` Strides& :target:`operator =<doxid-classov_1_1_strides_1a7500eade79d938f0cb18a56c7b4f008e>` (Strides&& v);
	};

