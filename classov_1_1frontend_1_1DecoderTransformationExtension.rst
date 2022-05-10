.. index:: pair: class; ov::frontend::DecoderTransformationExtension
.. _doxid-classov_1_1frontend_1_1_decoder_transformation_extension:

class ov::frontend::DecoderTransformationExtension
==================================================



Overview
~~~~~~~~

Holds a transformation that is applied just after the original model graph is decoded. This class is a holder for transformation. The transformation can be specified as FunctionPass or MathcerPass derivatives or as a function that can be used to build corresponding FunctionPass or MatcherPass object. The type of the extension is determined in the moment of creation by calling corresponding ctor. :ref:`More...<details-classov_1_1frontend_1_1_decoder_transformation_extension>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <decoder_transformation.hpp>
	
	class DecoderTransformationExtension: public :ref:`ov::Extension<doxid-classov_1_1_extension>`
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<DecoderTransformationExtension> :target:`Ptr<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a2fa191b1c769551b1cb33c946aa979d3>`;

		// construction
	
		:target:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a6f8feb7be6186aec354194f44bfb27b8>`();
		:ref:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a32c91ba446a61e879c8c57d5101d063c>`(const std::function<bool(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>)>& function_pass);
		:ref:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a4b06438f2e3651e1cdb602c379b9eb74>`(const std::function<void(:ref:`ov::pass::MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>` \*)>& matcher_pass_initializer);
	
		template <
			typename Transformation,
			typename std::enable_if<std::is_base_of<ov::pass::PassBase, Transformation>::value, bool>::type = true
			>
		:ref:`DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1aa45c9d31cff76398810588ecca5b30b0>`(const Transformation& transformation);

		// methods
	
		void :ref:`register_pass<doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1ae64bff80d11b145eee233c04175ccd66>`(:ref:`ov::pass::Manager<doxid-classov_1_1pass_1_1_manager>`& manager) const;
	};

	// direct descendants

	class :ref:`JsonConfigExtension<doxid-classov_1_1frontend_1_1_json_config_extension>`;
	class :ref:`JsonTransformationExtension<doxid-classov_1_1frontend_1_1_json_transformation_extension>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;

.. _details-classov_1_1frontend_1_1_decoder_transformation_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Holds a transformation that is applied just after the original model graph is decoded. This class is a holder for transformation. The transformation can be specified as FunctionPass or MathcerPass derivatives or as a function that can be used to build corresponding FunctionPass or MatcherPass object. The type of the extension is determined in the moment of creation by calling corresponding ctor.

Construction
------------

.. _doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a32c91ba446a61e879c8c57d5101d063c:
.. index:: pair: function; DecoderTransformationExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DecoderTransformationExtension(const std::function<bool(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>)>& function_pass)

Create a custom functional pass where code of the pass is implemented as a function.

.. _doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1a4b06438f2e3651e1cdb602c379b9eb74:
.. index:: pair: function; DecoderTransformationExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DecoderTransformationExtension(const std::function<void(:ref:`ov::pass::MatcherPass<doxid-classov_1_1pass_1_1_matcher_pass>` \*)>& matcher_pass_initializer)

Create a custom matcher pass where the code of matcher pass initialization is a given function.

.. _doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1aa45c9d31cff76398810588ecca5b30b0:
.. index:: pair: function; DecoderTransformationExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename Transformation,
		typename std::enable_if<std::is_base_of<ov::pass::PassBase, Transformation>::value, bool>::type = true
		>
	DecoderTransformationExtension(const Transformation& transformation)

Register existing transformation object which will be copied and kept for further registration.

Methods
-------

.. _doxid-classov_1_1frontend_1_1_decoder_transformation_extension_1ae64bff80d11b145eee233c04175ccd66:
.. index:: pair: function; register_pass

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void register_pass(:ref:`ov::pass::Manager<doxid-classov_1_1pass_1_1_manager>`& manager) const

Register pass from this object in a given pass manager object.


