.. index:: pair: class; ov::AxisSet
.. _doxid-classov_1_1_axis_set:

class ov::AxisSet
=================



A set of axes.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <axis_set.hpp>
	
	class AxisSet: public std::set< size_t >
	{
	public:
		// construction
	
		:target:`AxisSet<doxid-classov_1_1_axis_set_1a252c57f3ec5a37efb563ea838f3d8710>`();
		:target:`AxisSet<doxid-classov_1_1_axis_set_1a563f84ec83e0d7931ebb2abb6ab1a9ac>`(const std::initializer_list<size_t>& axes);
		:target:`AxisSet<doxid-classov_1_1_axis_set_1a322c8b56c1edc76947bd86cafb038ea5>`(const std::set<size_t>& axes);
		:target:`AxisSet<doxid-classov_1_1_axis_set_1a5ade45642f1ba881f02f454a6a2bfcdd>`(const std::vector<size_t>& axes);
		:target:`AxisSet<doxid-classov_1_1_axis_set_1a57c44971e08c7c2a2882f0c40ac7d299>`(const AxisSet& axes);

		// methods
	
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` AxisSet& :target:`operator =<doxid-classov_1_1_axis_set_1af07f410efdbbd351aafcc48dc7178cb8>` (const AxisSet& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` AxisSet& :target:`operator =<doxid-classov_1_1_axis_set_1a4a227c59cd445e02138c06487df4bbc4>` (AxisSet&& v);
		:ref:`OPENVINO_API<doxid-core__visibility_8hpp_1a2214190530d05477d26ce917978f1750>` std::vector<int64_t> :target:`to_vector<doxid-classov_1_1_axis_set_1a9808d8a28a991c4d01899683f520914c>`() const;
	};

