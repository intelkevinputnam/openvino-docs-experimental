.. index:: pair: struct; ov::frontend::ExtensionHolder
.. _doxid-structov_1_1frontend_1_1_extension_holder:

struct ov::frontend::ExtensionHolder
====================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <holder.hpp>
	
	struct ExtensionHolder
	{
		// fields
	
		std::shared_ptr<:ref:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension>`> :target:`progress_reporter<doxid-structov_1_1frontend_1_1_extension_holder_1aef4d723b80bf28c512e49ae2476325b6>` {std::make_shared<:ref:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension>`>()};
		std::shared_ptr<:ref:`TelemetryExtension<doxid-classov_1_1frontend_1_1_telemetry_extension>`> :target:`telemetry<doxid-structov_1_1frontend_1_1_extension_holder_1a61c6875fc9f99e4434ecbe893b373c32>`;
		std::vector<std::shared_ptr<:ref:`ConversionExtensionBase<doxid-classov_1_1frontend_1_1_conversion_extension_base>`>> :target:`conversions<doxid-structov_1_1frontend_1_1_extension_holder_1ad081ccf1cad1ab28cddd015dc78efb45>`;
	};

