.. index:: pair: class; ngraph::pass::low_precision::InferenceEngineLptException
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_inference_engine_lpt_exception:

class ngraph::pass::low_precision::InferenceEngineLptException
==============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_lpt_exception.hpp>
	
	class InferenceEngineLptException: public :ref:`ngraph::pass::low_precision::Exception<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception>`
	{
	public:
		// construction
	
		:target:`InferenceEngineLptException<doxid-classngraph_1_1pass_1_1low__precision_1_1_inference_engine_lpt_exception_1af565b331c12bdfd47baf2915b302b3a1>`(
			const std::string& filename,
			const size_t line,
			const :ref:`Node<doxid-classov_1_1_node>`& node
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		template <typename T>
		:ref:`Exception<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception>`& :ref:`operator <<<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception_1afaab8896151043d54fdaeba0c661e936>` (const T& x);
	
		const char \* :ref:`what<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception_1a29b84c83ff408e21d0a82ad580aa91f4>`() const;


