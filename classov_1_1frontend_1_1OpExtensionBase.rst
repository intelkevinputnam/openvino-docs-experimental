.. index:: pair: class; ov::frontend::OpExtensionBase<BaseConversionType, void>
.. _doxid-classov_1_1frontend_1_1_op_extension_base_3_01_base_conversion_type_00_01void_01_4:

class ov::frontend::OpExtensionBase<BaseConversionType, void>
=============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <op.hpp>
	
	template <typename BaseConversionType>
	class OpExtensionBase<BaseConversionType, void>: public BaseConversionType
	{
	public:
		// construction
	
		:target:`OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base_3_01_base_conversion_type_00_01void_01_4_1acf7eff0b4db4f87ee5125a25633bafab>`();
	
		:target:`OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base_3_01_base_conversion_type_00_01void_01_4_1a963ae9201360be79d9444a8b1a2caa41>`(
			const std::string& fw_ov_type_name,
			const std::map<std::string, std::string>& attr_names_map = {},
			const std::map<std::string, :ref:`ov::Any<doxid-classov_1_1_any>`>& attr_values_map = {}
			);
	
		:target:`OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base_3_01_base_conversion_type_00_01void_01_4_1afa13111acba433f8ac3cd34f94e9786c>`(
			const std::string& ov_type_name,
			const std::string& fw_type_name,
			const std::map<std::string, std::string>& attr_names_map = {},
			const std::map<std::string, :ref:`ov::Any<doxid-classov_1_1_any>`>& attr_values_map = {}
			);
	};

.. index:: pair: class; ov::frontend::OpExtensionBase
.. _doxid-classov_1_1frontend_1_1_op_extension_base:

class ov::frontend::OpExtensionBase
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <op.hpp>
	
	template <typename BaseConversionType, typename OVOpType = void>
	class OpExtensionBase: public BaseConversionType
	{
	public:
		// construction
	
		:target:`OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base_1a4fe2bec5a4164d6e2288efb5f52e49d4>`(
			const std::map<std::string, std::string>& attr_names_map = {},
			const std::map<std::string, :ref:`ov::Any<doxid-classov_1_1_any>`>& attr_values_map = {}
			);
	
		:target:`OpExtensionBase<doxid-classov_1_1frontend_1_1_op_extension_base_1a8d0284577113207fef800b8016af80c1>`(
			const std::string& fw_type_name,
			const std::map<std::string, std::string>& attr_names_map = {},
			const std::map<std::string, :ref:`ov::Any<doxid-classov_1_1_any>`>& attr_values_map = {}
			);
	};

