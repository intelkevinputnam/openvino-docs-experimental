.. index:: pair: class; ov::CoordinateDiff
.. _doxid-classov_1_1_coordinate_diff:

class ov::CoordinateDiff
========================



A difference (signed) of tensor element coordinates.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <coordinate_diff.hpp>
	
	class CoordinateDiff: public std::vector< std::ptrdiff_t >
	{
	public:
		// construction
	
		:target:`CoordinateDiff<doxid-classov_1_1_coordinate_diff_1a450de94c8b9c8e374558f0b20942c314>`(const std::initializer_list<std::ptrdiff_t>& diffs);
		:target:`CoordinateDiff<doxid-classov_1_1_coordinate_diff_1a971861f4ee4274e75782a05f6f9047c1>`(const std::vector<std::ptrdiff_t>& diffs);
		:target:`CoordinateDiff<doxid-classov_1_1_coordinate_diff_1af61228c32f80712e1abcdf5ef2c8c5de>`(const CoordinateDiff& diffs);
		:target:`CoordinateDiff<doxid-classov_1_1_coordinate_diff_1a52ac9b0516cca4e438e178525ebb8932>`(size_t n, std::ptrdiff_t initial_value = 0);
	
		template <class InputIterator>
		:target:`CoordinateDiff<doxid-classov_1_1_coordinate_diff_1a7f183ac648361d7a2a7e4972d6937b49>`(
			InputIterator first,
			InputIterator last
			);
	
		:target:`CoordinateDiff<doxid-classov_1_1_coordinate_diff_1a2be519e79f2932c5304c5bde3e2197e5>`();

		// methods
	
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` CoordinateDiff& :target:`operator =<doxid-classov_1_1_coordinate_diff_1a481c0d37f247b104955c9799804f0657>` (const CoordinateDiff& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` CoordinateDiff& :target:`operator =<doxid-classov_1_1_coordinate_diff_1a085b17e36e32d94f6bc93a48e531e25b>` (CoordinateDiff&& v);
	};

