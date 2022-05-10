.. index:: pair: class; ov::frontend::ConversionExtension
.. _doxid-classov_1_1frontend_1_1_conversion_extension:

class ov::frontend::ConversionExtension
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <conversion.hpp>
	
	class ConversionExtension: public :ref:`ov::frontend::ConversionExtensionBase<doxid-classov_1_1frontend_1_1_conversion_extension_base>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<ConversionExtension> :target:`Ptr<doxid-classov_1_1frontend_1_1_conversion_extension_1aa2501008db75bd4f96c766e30abf5908>`;

		// construction
	
		:target:`ConversionExtension<doxid-classov_1_1frontend_1_1_conversion_extension_1aecda5757f220141138bdcc56b3c1cdca>`(
			const std::string& op_type,
			const :ref:`CreatorFunction<doxid-namespaceov_1_1frontend_1aa8aab3222c4b95dbd11746783646cb3c>`& converter
			);
	
		:target:`ConversionExtension<doxid-classov_1_1frontend_1_1_conversion_extension_1ac12b6113435c28e9f01afc47b5ccc524>`(
			const std::string& op_type,
			const :ref:`CreatorFunctionNamed<doxid-namespaceov_1_1frontend_1a9a8b976c6b2003da87f8d8dfedaa99f0>`& converter
			);

		// methods
	
		const :ref:`CreatorFunction<doxid-namespaceov_1_1frontend_1aa8aab3222c4b95dbd11746783646cb3c>`& :target:`get_converter<doxid-classov_1_1frontend_1_1_conversion_extension_1a6cadcf94499b86276dad555de9c011ab>`() const;
		const :ref:`CreatorFunctionNamed<doxid-namespaceov_1_1frontend_1a9a8b976c6b2003da87f8d8dfedaa99f0>`& :target:`get_converter_named<doxid-classov_1_1frontend_1_1_conversion_extension_1afd29f31d856e79153bd8b84ffaf0c304>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;
		typedef std::shared_ptr<:ref:`ConversionExtensionBase<doxid-classov_1_1frontend_1_1_conversion_extension_base>`> :ref:`Ptr<doxid-classov_1_1frontend_1_1_conversion_extension_base_1aaa0c601fa825e84ca29256d08b28acdf>`;

		// methods
	
		const std::string& :ref:`get_op_type<doxid-classov_1_1frontend_1_1_conversion_extension_base_1a3133218594a841b365b3c911e98b86a2>`() const;


