.. index:: pair: class; ov::AssertFailure
.. _doxid-classov_1_1_assert_failure:

class ov::AssertFailure
=======================



Base class for check failure exceptions.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <except.hpp>
	
	class AssertFailure: public :ref:`ov::Exception<doxid-classov_1_1_exception>`
	{
	public:
		// construction
	
		:target:`AssertFailure<doxid-classov_1_1_assert_failure_1aa1c4b446039497ca6253dfe7eda73ee8>`(
			const :ref:`CheckLocInfo<doxid-structov_1_1_check_loc_info>`& check_loc_info,
			const std::string& context_info,
			const std::string& explanation
			);
	};

	// direct descendants

	class :ref:`GeneralFailure<doxid-classov_1_1frontend_1_1_general_failure>`;
	class :ref:`InitializationFailure<doxid-classov_1_1frontend_1_1_initialization_failure>`;
	class :ref:`NotImplementedFailure<doxid-classov_1_1frontend_1_1_not_implemented_failure>`;
	class :ref:`OpConversionFailure<doxid-classov_1_1frontend_1_1_op_conversion_failure>`;
	class :ref:`OpValidationFailure<doxid-classov_1_1frontend_1_1_op_validation_failure>`;
	class :ref:`NodeValidationFailure<doxid-classov_1_1_node_validation_failure>`;
	class :ref:`NotImplemented<doxid-classov_1_1_not_implemented>`;

