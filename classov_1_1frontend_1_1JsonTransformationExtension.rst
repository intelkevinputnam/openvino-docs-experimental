.. index:: pair: class; ov::frontend::JsonTransformationExtension
.. _doxid-classov_1_1frontend_1_1_json_transformation_extension:

class ov::frontend::JsonTransformationExtension
===============================================



Overview
~~~~~~~~

Describes transformation that :ref:`JsonConfigExtension <doxid-classov_1_1frontend_1_1_json_config_extension>` can use as a target transformation specified by ID. :ref:`JsonTransformationExtension <doxid-classov_1_1frontend_1_1_json_transformation_extension>` passes JSON parsed object and matched points in the graph to :ref:`JsonTransformationExtension <doxid-classov_1_1frontend_1_1_json_transformation_extension>` instance, which is derived from :ref:`DecoderTransformationExtension <doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`. :ref:`DecoderTransformationExtension <doxid-classov_1_1frontend_1_1_decoder_transformation_extension>` itself cannot be used for this purpose because we need to pass those additional objects which are the result of JSON parsing and graph matching that :ref:`JsonTransformationExtension <doxid-classov_1_1frontend_1_1_json_transformation_extension>` performs. :ref:`More...<details-classov_1_1frontend_1_1_json_transformation_extension>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <json_transformation.hpp>
	
	class JsonTransformationExtension: public :ref:`ov::frontend::DecoderTransformationExtension<doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`
	{
	public:
		// construction
	
		:target:`JsonTransformationExtension<doxid-classov_1_1frontend_1_1_json_transformation_extension_1a78a096c942eb19e4a161a044305ac221>`(const std::string& id);

		// methods
	
		const std::string& :ref:`id<doxid-classov_1_1frontend_1_1_json_transformation_extension_1a5986ce97364ab4857383c3def7e47ebf>`() const;
	
		virtual bool :ref:`transform<doxid-classov_1_1frontend_1_1_json_transformation_extension_1ad692d215998250ca33777d419b07f233>`(
			const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& function,
			const std::string& replacement_descriptions
			) const = 0;
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

.. _details-classov_1_1frontend_1_1_json_transformation_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Describes transformation that :ref:`JsonConfigExtension <doxid-classov_1_1frontend_1_1_json_config_extension>` can use as a target transformation specified by ID. :ref:`JsonTransformationExtension <doxid-classov_1_1frontend_1_1_json_transformation_extension>` passes JSON parsed object and matched points in the graph to :ref:`JsonTransformationExtension <doxid-classov_1_1frontend_1_1_json_transformation_extension>` instance, which is derived from :ref:`DecoderTransformationExtension <doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`. :ref:`DecoderTransformationExtension <doxid-classov_1_1frontend_1_1_decoder_transformation_extension>` itself cannot be used for this purpose because we need to pass those additional objects which are the result of JSON parsing and graph matching that :ref:`JsonTransformationExtension <doxid-classov_1_1frontend_1_1_json_transformation_extension>` performs.

This class is left for backward compatibility only. In the future we would like to get rid off this class as well as from :ref:`JsonConfigExtension <doxid-classov_1_1frontend_1_1_json_config_extension>`, and users will use :ref:`DecoderTransformationExtension <doxid-classov_1_1frontend_1_1_decoder_transformation_extension>` only to match sub-graph and modify it like we do in any other transformations.

Unlike :ref:`DecoderTransformationExtension <doxid-classov_1_1frontend_1_1_decoder_transformation_extension>`, which is initialized by some ready-to-use transformation code and is not used to derive new classes by regular users, this class is intended to be derived from and it doesn't have convenient ctos to be initialized. So it is intended for more advanced, internal users inside such components like :ref:`Model <doxid-classov_1_1_model>` Optimizer.

Methods
-------

.. _doxid-classov_1_1frontend_1_1_json_transformation_extension_1a5986ce97364ab4857383c3def7e47ebf:
.. index:: pair: function; id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::string& id() const

The name of the transformation to identify it from JSON file field 'id'.

.. _doxid-classov_1_1frontend_1_1_json_transformation_extension_1ad692d215998250ca33777d419b07f233:
.. index:: pair: function; transform

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool transform(
		const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& function,
		const std::string& replacement_descriptions
		) const = 0

Modifies OV :ref:`Model <doxid-classov_1_1_model>` according to the provided rules.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- function

		- The OV :ref:`Model <doxid-classov_1_1_model>` object.

	*
		- replacement_descriptions

		- The rules to modify the model in .json format.


