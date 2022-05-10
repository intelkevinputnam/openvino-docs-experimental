.. index:: pair: class; ngraph::Mask
.. _doxid-classngraph_1_1_mask:

class ngraph::Mask
==================



each element in vector represents dimension and each element in set is an id of dimensions which contains zeros.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <mask_attribute.hpp>
	
	class Mask:
	    public std::vector< std::set< uint64_t > >,
	    public std::enable_shared_from_this< Mask >
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Mask> :target:`Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>`;

		// construction
	
		:target:`Mask<doxid-classngraph_1_1_mask_1ab0d6da71112db613a87c47c62ded0a30>`();
		:target:`Mask<doxid-classngraph_1_1_mask_1ad626d8eb3b12cbb2581e7c99f695ccc8>`(const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& shape);
		:target:`Mask<doxid-classngraph_1_1_mask_1af80775639003bbe449bffd434e0eea3e>`(const size_t& size);
		:target:`Mask<doxid-classngraph_1_1_mask_1aefa8dd780ffd13a7a2c0ff4d8f4bc806>`(const size_t& size, const bool adjust_value);
		:target:`Mask<doxid-classngraph_1_1_mask_1adf2e2c857f1622405c404a7da978c17c>`(const std::vector<value_type> val);
		:target:`Mask<doxid-classngraph_1_1_mask_1aeafe75bc8490ffe5daad29e26e920960>`(std::initializer_list<std::initializer_list<uint64_t>> list);

		// methods
	
		static const :::ref:`ov::DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info_static<doxid-classngraph_1_1_mask_1ad2cd96accc2369ffb6d908e1a3feb4ef>`();
		bool :target:`all_dims_are_empty<doxid-classngraph_1_1_mask_1a9441d9c7a73a32092f54b171e0395c97>`() const;
		std::vector<size_t> :target:`get_not_empty_dims<doxid-classngraph_1_1_mask_1a3e0ea11885aee7a2ec1823c9a6828a2a>`();
		bool :target:`is_shape_like<doxid-classngraph_1_1_mask_1a0ad2353b35efba7fb3fcc0a1541e7361>`() const;
		void :target:`set_shape_like<doxid-classngraph_1_1_mask_1a1da68da87fe7483bebf1f77a1e29ccd1>`(bool flag);
		void :target:`copy_value_from_mask<doxid-classngraph_1_1_mask_1aea1e8f612892ec55b8d27346185ff6bd>`(Mask \*const mask);
		void :target:`copy_value_from_mask_reversed<doxid-classngraph_1_1_mask_1ad7bdb401ffede2e02d137dab4facc3d8>`(Mask \*const mask);
		:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>` :target:`intersect_masks_reversed<doxid-classngraph_1_1_mask_1aa0a9522eb2de28abae116b6cff2f2e8f>`(Mask \*const mask);
		:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>` :target:`union_masks_reversed<doxid-classngraph_1_1_mask_1aaf5b03294bd1654f30fcde1eb325e75f>`(Mask \*const mask) const;
	
		bool :target:`add_callback<doxid-classngraph_1_1_mask_1a0ea0d0ab67a2c229adad71b35c06f49e>`(
			const std::function<bool(:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>`)>& receive_callback,
			:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>` mask
			);
	
		bool :target:`apply_callback<doxid-classngraph_1_1_mask_1a9ddc87568580b9fdac67febf5e8cfe55>`(:ref:`Mask::Ptr<doxid-classngraph_1_1_mask_1a630cd1649de5c00bdff3faf0845e15b2>` mask);
		void :target:`invalidate<doxid-classngraph_1_1_mask_1aac21b960b2af5e3f18ff13046b78eca5>`();
		void :target:`clean_dim_values<doxid-classngraph_1_1_mask_1a7d96b870088143dcdc2993f2f0e54efe>`();
		void :target:`initialize_dependencies<doxid-classngraph_1_1_mask_1aee73d6f40391b8754273de1a3adb8347>`();
		bool :target:`adjust_value<doxid-classngraph_1_1_mask_1a4e161290a02651b5207c110515feb11c>`() const;
	};

