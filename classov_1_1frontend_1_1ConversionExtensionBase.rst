.. index:: pair: class; ov::frontend::ConversionExtensionBase
.. _doxid-classov_1_1frontend_1_1_conversion_extension_base:

class ov::frontend::ConversionExtensionBase
===========================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <conversion.hpp>
	
	class ConversionExtensionBase: public :ref:`ov::Extension<doxid-classov_1_1_extension>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<ConversionExtensionBase> :target:`Ptr<doxid-classov_1_1frontend_1_1_conversion_extension_base_1aaa0c601fa825e84ca29256d08b28acdf>`;

		// construction
	
		:target:`ConversionExtensionBase<doxid-classov_1_1frontend_1_1_conversion_extension_base_1ad3bf7b7c3b99d96b3b362f98f0af1aaf>`(const std::string& op_type);

		// methods
	
		const std::string& :target:`get_op_type<doxid-classov_1_1frontend_1_1_conversion_extension_base_1a3133218594a841b365b3c911e98b86a2>`() const;
	};

	// direct descendants

	class :ref:`ConversionExtension<doxid-classov_1_1frontend_1_1_conversion_extension>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;


