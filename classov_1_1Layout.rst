.. index:: pair: class; ov::Layout
.. _doxid-classov_1_1_layout:

class ov::Layout
================



Overview
~~~~~~~~

:ref:`ov::Layout <doxid-classov_1_1_layout>` represents the text information of tensor's dimensions/axes. E.g. layout ``NCHW`` means that 4D tensor ``{-1, 3, 480, 640}`` will have: :ref:`More...<details-classov_1_1_layout>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layout.hpp>
	
	class Layout
	{
	public:
		// construction
	
		:ref:`Layout<doxid-classov_1_1_layout_1a5f1c0a4db337e976786c1b24775541db>`();
		:ref:`Layout<doxid-classov_1_1_layout_1ac709cca91f40043e17282c5fc8e1997e>`(const char \* layoutStr);
		:target:`Layout<doxid-classov_1_1_layout_1a0e99d2cd650282ce5407c0070f40675d>`(const std::string& layoutStr);

		// methods
	
		bool :ref:`operator ==<doxid-classov_1_1_layout_1afb8b63125fe8246f285999584ff65eb3>` (const Layout& rhs) const;
		bool :ref:`operator !=<doxid-classov_1_1_layout_1abddd5c98f6d67ad2210e389f57f7c371>` (const Layout& rhs) const;
		bool :ref:`has_name<doxid-classov_1_1_layout_1ae8aafc56d57323a6c24ad49203d9da32>`(const std::string& dimensionName) const;
		std::int64_t :ref:`get_index_by_name<doxid-classov_1_1_layout_1ab989905d6faeb454c452c88bc4ce733a>`(const std::string& dimensionName) const;
		std::string :ref:`to_string<doxid-classov_1_1_layout_1aeb5b072228164ba63fdc42fa5eafec44>`() const;
		bool :ref:`empty<doxid-classov_1_1_layout_1a137187425e1629e243579759ea58e2dd>`() const;
		static Layout :ref:`scalar<doxid-classov_1_1_layout_1a31ff108665aee6740f3337b37ecc86b7>`();
	};
.. _details-classov_1_1_layout:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`ov::Layout <doxid-classov_1_1_layout>` represents the text information of tensor's dimensions/axes. E.g. layout ``NCHW`` means that 4D tensor ``{-1, 3, 480, 640}`` will have:

* 0: ``N = -1`` : batch dimension is dynamic

* 1: ``C = 3`` : number of channels is '3'

* 2: ``H = 480`` : image height is 480

* 3: ``W = 640`` : image width is 640

Examples: ``:ref:`ov::Layout <doxid-classov_1_1_layout>``` can be specified for:

* Preprocessing purposes. E.g.
  
  * To apply normalization (means/scales) it is usually required to set 'C' dimension in a layout.
  
  * To resize the image to specified width/height it is needed to set 'H' and 'W' dimensions in a layout
  
  * To transpose image - source and target layout can be set (see ``:ref:`ov::preprocess::PreProcessSteps::convert_layout <doxid-classov_1_1preprocess_1_1_pre_process_steps_1ab5a0cd9d0090f82e0489171a057fcfd4>```)

* To set/get model's batch (see ``:ref:`ov::get_batch <doxid-namespaceov_1a07e004b4295ab71df7a23accb362486b>``` / :ref:`ov::set_batch <doxid-namespaceov_1a3314e2ff91fcc9ffec05b1a77c37862b>`) it is required in general to specify 'N' dimension in layout for appropriate inputs

Refer also to ``:ref:`ov::layout <doxid-namespaceov_1_1layout>``` namespace for various additional helper functions of ``:ref:`ov::Layout <doxid-classov_1_1_layout>```

Construction
------------

.. _doxid-classov_1_1_layout_1a5f1c0a4db337e976786c1b24775541db:
.. index:: pair: function; Layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Layout()

Constructs a dynamic :ref:`Layout <doxid-classov_1_1_layout>` with no layout information.

.. _doxid-classov_1_1_layout_1ac709cca91f40043e17282c5fc8e1997e:
.. index:: pair: function; Layout

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Layout(const char \* layoutStr)

Constructs a :ref:`Layout <doxid-classov_1_1_layout>` with static or dynamic layout information based on string representation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layoutStr

		- 
		  The string used to construct :ref:`Layout <doxid-classov_1_1_layout>` from. The string representation can be in the following form:
		  
		  * can define order and meaning for dimensions "NCHW"
		  
		  * partial layout specialization:
		    
		    * "NC?" defines 3 dimensional layout, first two NC, 3rd one is not defined
		    
		    * "N...C" defines layout with dynamic rank where 1st dimension is N, last one is C
		    
		    * "NC..." defines layout with dynamic rank where first two are NC, others are not defined
		  
		  * only order of dimensions "adbc" (0312)
		  
		  * Advanced syntax can be used for multi-character names like "[N,C,H,W,...,CustomName]"

Methods
-------

.. _doxid-classov_1_1_layout_1afb8b63125fe8246f285999584ff65eb3:
.. index:: pair: function; operator==

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator == (const Layout& rhs) const

Comparison operator (equal)

.. _doxid-classov_1_1_layout_1abddd5c98f6d67ad2210e389f57f7c371:
.. index:: pair: function; operator!=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool operator != (const Layout& rhs) const

Comparison operator (not equal)

.. _doxid-classov_1_1_layout_1ae8aafc56d57323a6c24ad49203d9da32:
.. index:: pair: function; has_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool has_name(const std::string& dimensionName) const

Checks if dimension with specified name is in layout.



.. rubric:: Returns:

``true`` if layout has information about dimension index with a given name

.. _doxid-classov_1_1_layout_1ab989905d6faeb454c452c88bc4ce733a:
.. index:: pair: function; get_index_by_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::int64_t get_index_by_name(const std::string& dimensionName) const

Gets index of dimension with a specified name.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`ov::AssertFailure <doxid-classov_1_1_assert_failure>`

		- if dimension name is not found in a layout



.. rubric:: Returns:

Index of given dimension name

.. _doxid-classov_1_1_layout_1aeb5b072228164ba63fdc42fa5eafec44:
.. index:: pair: function; to_string

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string to_string() const

String representation of :ref:`Layout <doxid-classov_1_1_layout>`.

.. _doxid-classov_1_1_layout_1a137187425e1629e243579759ea58e2dd:
.. index:: pair: function; empty

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool empty() const

Returns 'true' if layout has no information, i.e. equals to :ref:`Layout() <doxid-classov_1_1_layout_1a5f1c0a4db337e976786c1b24775541db>`

.. _doxid-classov_1_1_layout_1a31ff108665aee6740f3337b37ecc86b7:
.. index:: pair: function; scalar

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static Layout scalar()

Constructs layout representing scalar.


