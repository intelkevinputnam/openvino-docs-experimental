.. index:: pair: class; ov::frontend::JsonConfigExtension
.. _doxid-classov_1_1frontend_1_1_json_config_extension:

class ov::frontend::JsonConfigExtension
=======================================



:ref:`JsonConfigExtension <doxid-classov_1_1frontend_1_1_json_config_extension>` reads MO config file and delegate transformation functionality to specified transformation ID specified in the config.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <json_config.hpp>
	
	class JsonConfigExtension: public :ref:`ov::frontend::DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`
	{
	public:
		// construction
	
		:target:`JsonConfigExtension<doxid-classov_1_1frontend_1_1_json_config_extension_1ad20d7bc3fcab84a7a855c7f7e1c88984>`(const std::string& config_path);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;
		typedef std::shared_ptr<:ref:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`> :ref:`Ptr<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a2fa191b1c769551b1cb33c946aa979d3>`;

		// methods
	
		void :ref:`register_pass<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1ae64bff80d11b145eee233c04175ccd66>`(:ref:`ov::pass::Manager<doxid-classov_1_1pass_1_1_manager>`& manager) const;


