.. index:: pair: class; ngraph::runtime::AlignedBuffer
.. _doxid-classngraph_1_1runtime_1_1_aligned_buffer:

class ngraph::runtime::AlignedBuffer
====================================



Allocates a block of memory on the specified alignment. The actual size of the allocated memory is larger than the requested size by the alignment, so allocating 1 byte on 64 byte alignment will allocate 65 bytes.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <aligned_buffer.hpp>
	
	class AlignedBuffer
	{
	public:
		// construction
	
		:target:`AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a5a8243165c602225ee9c3219f000c7cd>`(size_t byte_size, size_t alignment = 64);
		:target:`AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1ac08241ec613ba56b66444d53a91be683>`();
		:target:`AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a1303de657eb30a4c35d1dafbc964b29a>`(AlignedBuffer&& other);

		// methods
	
		AlignedBuffer& :target:`operator =<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a83a5ec032c4fb86c4299cc7cecbe8ea7>` (AlignedBuffer&& other);
		size_t :target:`size<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a514fa275fa2539bd7f850fa21c77fc59>`() const;
		void \* :target:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a4e662bc9243f36a69ae58d108813ffff>`(size_t offset) const;
		void \* :target:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a5e725de1498c1eb406822fd82bdec4a6>`();
		const void \* :target:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1aeeeeb6d37d8f07d4cd6864a6b1464009>`() const;
	
		template <typename T>
		T \* :target:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a3390474a867f39ba04e9a558876e28e0>`();
	
		template <typename T>
		const T \* :target:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1acac9908479f33d4d41e96f5273538fad>`() const;
	
		template <typename T>
		:target:`operator T\*<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1ab1f956dae85e78b1518c39ecb97bc280>` ();
	};

	// direct descendants

	template <typename T>
	class :ref:`SharedBuffer<doxid-classngraph_1_1runtime_1_1_shared_buffer>`;

