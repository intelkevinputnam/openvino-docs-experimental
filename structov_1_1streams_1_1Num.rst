.. index:: pair: struct; ov::streams::Num
.. _doxid-structov_1_1streams_1_1_num:

struct ov::streams::Num
=======================



Overview
~~~~~~~~

Class to represent number of streams in streams executor. :ref:`More...<details-structov_1_1streams_1_1_num>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>
	
	struct Num
	{
		// typedefs
	
		typedef std::tuple<int32_t> :ref:`Base<doxid-structov_1_1streams_1_1_num_1addf606043a7a938691a5e2f56250c3a2>`;

		// fields
	
		int32_t :target:`num<doxid-structov_1_1streams_1_1_num_1a8fae613a0fa062dcda6c2a402006202a>` = 0;

		// construction
	
		:target:`Num<doxid-structov_1_1streams_1_1_num_1ad71a814366aee0b095ce01a1a682d86f>`();
		:target:`Num<doxid-structov_1_1streams_1_1_num_1a4db8c8dcee5557ea756f1b7d2ab89e32>`(const int32_t num_);

		// methods
	
		constexpr :target:`operator int32_t<doxid-structov_1_1streams_1_1_num_1adcbd03b0315607a96fcd9c09d6ec82b8>` () const;
	};
.. _details-structov_1_1streams_1_1_num:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class to represent number of streams in streams executor.

Typedefs
--------

.. _doxid-structov_1_1streams_1_1_num_1addf606043a7a938691a5e2f56250c3a2:
.. index:: pair: typedef; Base

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::tuple<int32_t> Base

NumStreams is representable as int32_t.


