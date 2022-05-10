.. index:: pair: class; ov::Coordinate
.. _doxid-classov_1_1_coordinate:

class ov::Coordinate
====================



Coordinates for a tensor element.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <coordinate.hpp>
	
	class Coordinate: public std::vector< size_t >
	{
	public:
		// construction
	
		:target:`Coordinate<doxid-classov_1_1_coordinate_1a6696b2903143764bb204a8a386516501>`();
		:target:`Coordinate<doxid-classov_1_1_coordinate_1a5fa634fdfcd3e5c281058a62f6e089f7>`(const std::initializer_list<size_t>& axes);
		:target:`Coordinate<doxid-classov_1_1_coordinate_1aa835d038fb93058d6ab07c40decab946>`(const :ref:`Shape<doxid-classov_1_1_shape>`& shape);
		:target:`Coordinate<doxid-classov_1_1_coordinate_1a55befeb8b20f31a91e97c26cf4eaced5>`(const std::vector<size_t>& axes);
		:target:`Coordinate<doxid-classov_1_1_coordinate_1a16f343ee92dece1711d5ae361af56984>`(const Coordinate& axes);
		:target:`Coordinate<doxid-classov_1_1_coordinate_1a60c32a9133b7f9b1deae6184fef21f30>`(size_t n, size_t initial_value = 0);
	
		template <class InputIterator>
		:target:`Coordinate<doxid-classov_1_1_coordinate_1a844993071b1f0e3d701b773c8b685433>`(
			InputIterator first,
			InputIterator last
			);

		// methods
	
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` Coordinate& :target:`operator =<doxid-classov_1_1_coordinate_1ae3e5a713bd5fa58b62f08b240be09b87>` (const Coordinate& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` Coordinate& :target:`operator =<doxid-classov_1_1_coordinate_1a7462c4cb072791b258fb4d3e493710e8>` (Coordinate&& v);
	};

