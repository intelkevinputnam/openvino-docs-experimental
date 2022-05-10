.. index:: pair: class; ov::Exception
.. _doxid-classov_1_1_exception:

class ov::Exception
===================



Base error for ov runtime errors.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <except.hpp>
	
	class Exception: public runtime_error
	{
	public:
		// construction
	
		:target:`Exception<doxid-classov_1_1_exception_1a35f81e44f2fcfd71d9a6c2557b8e980d>`(const std::string& what_arg);
		:target:`Exception<doxid-classov_1_1_exception_1a0649d6110f36514a08b637946206d822>`(const char \* what_arg);
		:target:`Exception<doxid-classov_1_1_exception_1ac5210a68cc20207ec0781e7e0422f97c>`(const std::stringstream& what_arg);
	};

	// direct descendants

	class :ref:`AssertFailure<doxid-classov_1_1_assert_failure>`;
	class :ref:`Busy<doxid-classov_1_1_busy>`;
	class :ref:`Cancelled<doxid-classov_1_1_cancelled>`;
	struct :ref:`UnknownActivationFunction<doxid-structov_1_1op_1_1util_1_1error_1_1_unknown_activation_function>`;

