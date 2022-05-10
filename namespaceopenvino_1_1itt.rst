.. index:: pair: namespace; openvino::itt
.. _doxid-namespaceopenvino_1_1itt:

namespace openvino::itt
=======================

.. toctree::
	:hidden:

	domain_ <structopenvino_1_1itt_1_1domain_.rst>
	handle_ <structopenvino_1_1itt_1_1handle_.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace itt {

	// typedefs

	typedef struct :ref:`openvino::itt::domain_<doxid-structopenvino_1_1itt_1_1domain__>` \* :ref:`domain_t<doxid-group__ie__dev__profiling_1gaf592f242d12fecb8f6bd3391ae8bf52a>`;
	typedef struct :ref:`openvino::itt::handle_<doxid-structopenvino_1_1itt_1_1handle__>` \* :ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>`;

	// structs

	struct :ref:`domain_<doxid-structopenvino_1_1itt_1_1domain__>`;
	struct :ref:`handle_<doxid-structopenvino_1_1itt_1_1handle__>`;

	// classes

	template <domain_t(\*)() domain>
	class :ref:`ScopedTask<doxid-structopenvino_1_1itt_1_1_scoped_task>`;
	template <domain_t(\*)() domain>
	class :ref:`TaskChain<doxid-classopenvino_1_1itt_1_1_task_chain>`;

	// global functions

	void :ref:`threadName<doxid-group__ie__dev__profiling_1gaf246080ccfe9616f6fa6853e684dee45>`(const char \* name);
	void :target:`threadName<doxid-namespaceopenvino_1_1itt_1aa71e7748aef91ce5f9802f850d493079>`(const std::string& name);
	:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` :ref:`handle<doxid-group__ie__dev__profiling_1ga8579f29ef5313d519bcaee20dd543a1b>`(char const \* name);
	:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` :target:`handle<doxid-namespaceopenvino_1_1itt_1a683b13a697f5063269ee720ac4a0877b>`(const std::string& name);

	template <typename Tag>
	:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` :target:`handle<doxid-namespaceopenvino_1_1itt_1a0080337cce210399c8166a5a8bb6d542>`(:ref:`handle_t<doxid-group__ie__dev__profiling_1gadd0b8dfc02acc43373c379e697a84eb7>` h);

	} // namespace itt
