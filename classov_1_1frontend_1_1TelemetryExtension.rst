.. index:: pair: class; ov::frontend::TelemetryExtension
.. _doxid-classov_1_1frontend_1_1_telemetry_extension:

class ov::frontend::TelemetryExtension
======================================



Provides callback to report telemetry information back to Python code.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <telemetry.hpp>
	
	class TelemetryExtension: public :ref:`ov::Extension<doxid-classov_1_1_extension>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<TelemetryExtension> :target:`Ptr<doxid-classov_1_1frontend_1_1_telemetry_extension_1adac177aee9d75c7aac07429c92d85625>`;
		typedef std::function<void(const std::string&category, const std::string&error_message)> :target:`error_callback<doxid-classov_1_1frontend_1_1_telemetry_extension_1a54532cfdff5883c8d218be3c948d687f>`;
		typedef std::function<void(const std::string&category, const std::string&action, const std::string&label, int value)> :target:`event_callback<doxid-classov_1_1frontend_1_1_telemetry_extension_1a9f7c7dcbd521ea7ca319f8de33fdef0a>`;

		// construction
	
		:target:`TelemetryExtension<doxid-classov_1_1frontend_1_1_telemetry_extension_1adcb849543aaa8780c8577a1ebc1f95e1>`(
			const std::string& event_category,
			const :ref:`event_callback<doxid-classov_1_1frontend_1_1_telemetry_extension_1a9f7c7dcbd521ea7ca319f8de33fdef0a>`& send_event,
			const :ref:`error_callback<doxid-classov_1_1frontend_1_1_telemetry_extension_1a54532cfdff5883c8d218be3c948d687f>`& send_error,
			const :ref:`error_callback<doxid-classov_1_1frontend_1_1_telemetry_extension_1a54532cfdff5883c8d218be3c948d687f>`& send_stack_trace
			);

		// methods
	
		void :target:`send_event<doxid-classov_1_1frontend_1_1_telemetry_extension_1ae258b8fad34817003950d388e9332c36>`(
			const std::string& action,
			const std::string& label,
			int value = 1
			);
	
		void :target:`send_error<doxid-classov_1_1frontend_1_1_telemetry_extension_1a16c361a390fd0d1c4247344a6cb8954c>`(const std::string& error_message);
		void :target:`send_stack_trace<doxid-classov_1_1frontend_1_1_telemetry_extension_1a93400d024b734358efc263e2a9f57f3b>`(const std::string& error_message);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;


