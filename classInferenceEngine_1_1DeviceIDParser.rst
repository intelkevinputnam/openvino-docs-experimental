.. index:: pair: class; InferenceEngine::DeviceIDParser
.. _doxid-class_inference_engine_1_1_device_i_d_parser:

class InferenceEngine::DeviceIDParser
=====================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class DeviceIDParser
	{
	public:
		// construction
	
		:target:`DeviceIDParser<doxid-class_inference_engine_1_1_device_i_d_parser_1a8564447be0ac0e48c1795b2aaf1d560e>`(const std::string& deviceNameWithID);

		// methods
	
		std::string :target:`getDeviceID<doxid-class_inference_engine_1_1_device_i_d_parser_1a003f568077f4fb4f574db8295cc55774>`() const;
		std::string :target:`getDeviceName<doxid-class_inference_engine_1_1_device_i_d_parser_1ad0e83f69d5b407f9f2a17abc8f55b883>`() const;
		static std::vector<std::string> :target:`getHeteroDevices<doxid-class_inference_engine_1_1_device_i_d_parser_1a06cf35298d28181f32be95ceb0fbdc0b>`(std::string fallbackDevice);
		static std::vector<std::string> :target:`getMultiDevices<doxid-class_inference_engine_1_1_device_i_d_parser_1a342efefa94b9821ec2611166e351e193>`(std::string devicesList);
		static std::string :target:`getBatchDevice<doxid-class_inference_engine_1_1_device_i_d_parser_1af955877e0d9e8cbd25ceee7f1a7087e5>`(std::string devicesList);
	};

