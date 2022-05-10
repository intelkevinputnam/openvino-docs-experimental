.. index:: pair: class; ov::Extension
.. _doxid-classov_1_1_extension:

class ov::Extension
===================



The class provides the base interface for OpenVINO extensions.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <extension.hpp>
	
	class Extension
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Extension> :target:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;
	};

	// direct descendants

	class :ref:`BaseOpExtension<doxid-classov_1_1_base_op_extension>`;
	class :ref:`ConversionExtensionBase<doxid-classov_1_1frontend_1_1_conversion_extension_base>`;
	class :ref:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`;
	class :ref:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension>`;
	class :ref:`TelemetryExtension<doxid-classov_1_1frontend_1_1_telemetry_extension>`;

