.. index:: pair: class; ngraph::runtime::SharedBuffer
.. _doxid-classngraph_1_1runtime_1_1_shared_buffer:

class ngraph::runtime::SharedBuffer
===================================



:ref:`SharedBuffer <doxid-classngraph_1_1runtime_1_1_shared_buffer>` class to store pointer to pre-acclocated buffer.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <shared_buffer.hpp>
	
	template <typename T>
	class SharedBuffer: public :ref:`ngraph::runtime::AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer>`
	{
	public:
		// construction
	
		:target:`SharedBuffer<doxid-classngraph_1_1runtime_1_1_shared_buffer_1a42beecb7a12caba335dd31783dd105dd>`(char \* data, size_t size, const T& shared_object);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		:ref:`AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer>`& :ref:`operator =<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a83a5ec032c4fb86c4299cc7cecbe8ea7>` (:ref:`AlignedBuffer<doxid-classngraph_1_1runtime_1_1_aligned_buffer>`&& other);
		size_t :ref:`size<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a514fa275fa2539bd7f850fa21c77fc59>`() const;
		void \* :ref:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a4e662bc9243f36a69ae58d108813ffff>`(size_t offset) const;
		void \* :ref:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a5e725de1498c1eb406822fd82bdec4a6>`();
		const void \* :ref:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1aeeeeb6d37d8f07d4cd6864a6b1464009>`() const;
	
		template <typename T>
		T \* :ref:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1a3390474a867f39ba04e9a558876e28e0>`();
	
		template <typename T>
		const T \* :ref:`get_ptr<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1acac9908479f33d4d41e96f5273538fad>`() const;
	
		template <typename T>
		:ref:`operator T\*<doxid-classngraph_1_1runtime_1_1_aligned_buffer_1ab1f956dae85e78b1518c39ecb97bc280>` ();


