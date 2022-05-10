.. index:: pair: class; ngraph::pass::low_precision::Exception
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_exception:

class ngraph::pass::low_precision::Exception
============================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_lpt_exception.hpp>
	
	class Exception: public exception
	{
	public:
		// methods
	
		template <typename T>
		Exception& :target:`operator <<<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception_1afaab8896151043d54fdaeba0c661e936>` (const T& x);
	
		const char \* :target:`what<doxid-classngraph_1_1pass_1_1low__precision_1_1_exception_1a29b84c83ff408e21d0a82ad580aa91f4>`() const;
	};

	// direct descendants

	class :ref:`InferenceEngineLptException<doxid-classngraph_1_1pass_1_1low__precision_1_1_inference_engine_lpt_exception>`;

