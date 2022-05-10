.. index:: pair: class; ngraph::runtime::reference::Span
.. _doxid-classngraph_1_1runtime_1_1reference_1_1_span:

class ngraph::runtime::reference::Span
======================================



Overview
~~~~~~~~

:ref:`Span <doxid-classngraph_1_1runtime_1_1reference_1_1_span>` should mimic std::span. :ref:`More...<details-classngraph_1_1runtime_1_1reference_1_1_span>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <span.hpp>
	
	template <typename Element>
	class Span
	{
	public:
		// typedefs
	
		typedef Element :target:`value_type<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a3326321ee5e2f7a9362013a60413fb21>`;
		typedef std::size_t :target:`size_type<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a1777d9cc64e072c7d609c619b75fc014>`;

		// construction
	
		:target:`Span<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a057e40260f510d110408e53be739aa83>`();
		:target:`Span<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a0666136412a884d674ab913e86d274ea>`(Element \* data, std::size_t size);

		// methods
	
		constexpr Element \* :target:`begin<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a5e15ad9ec209930b22fea2333b8f185b>`() const;
		constexpr Element \* :target:`end<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a63de254d78a4713e900baa96caf8d3d3>`() const;
		constexpr std::size_t :target:`size<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1aa818436b747b78d7f9fd9d32cf2487da>`() const;
		constexpr bool :target:`empty<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a073f579ce2c0a127c08c000c802075cc>`() const;
		constexpr Element& :target:`front<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a7f45d6b23044a3739ef8bdbc8983e3c6>`() const;
		constexpr Element& :target:`back<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a7338a03b023d5334c8f22c057481ded4>`() const;
		constexpr Element& :target:`operator []<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a4276e660b73c8728a47b8b6434f3b616>` (std::size_t idx) const;
		Element& :target:`at<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a9265fc99dfe3a7136bd844904464f091>`(std::size_t idx) const;
	
		Span :ref:`subspan<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a552c4d1c9799af5c689aba3c4b75c79b>`(
			std::size_t offset,
			std::size_t size = std::numeric_limits<std::size_t>:::ref:`max<doxid-namespacengraph_1_1runtime_1_1reference_1a92cfabd79e866544fb35d44884e7adfd>`()
			) const;
	
		Span& :ref:`drop_front<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1aeaad0322d59798aee3c2d00177554f2e>`(std::size_t number_of_elements);
		Span& :ref:`drop_back<doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a7a28b1a7effc0d7bc67057ca7004ec0d>`(std::size_t number_of_elements);
	};
.. _details-classngraph_1_1runtime_1_1reference_1_1_span:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Span <doxid-classngraph_1_1runtime_1_1reference_1_1_span>` should mimic std::span.

Methods
-------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a552c4d1c9799af5c689aba3c4b75c79b:
.. index:: pair: function; subspan

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Span subspan(
		std::size_t offset,
		std::size_t size = std::numeric_limits<std::size_t>:::ref:`max<doxid-namespacengraph_1_1runtime_1_1reference_1a92cfabd79e866544fb35d44884e7adfd>`()
		) const

return sub part of span starting from offset and not greater than size

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_span_1aeaad0322d59798aee3c2d00177554f2e:
.. index:: pair: function; drop_front

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Span& drop_front(std::size_t number_of_elements)

drop number of elements from front

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_span_1a7a28b1a7effc0d7bc67057ca7004ec0d:
.. index:: pair: function; drop_back

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Span& drop_back(std::size_t number_of_elements)

drop number of elements from back


