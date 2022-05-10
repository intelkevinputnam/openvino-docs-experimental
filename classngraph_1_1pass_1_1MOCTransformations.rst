.. index:: pair: class; ngraph::pass::MOCTransformations
.. _doxid-classngraph_1_1pass_1_1_m_o_c_transformations:

class ngraph::pass::MOCTransformations
======================================



Overview
~~~~~~~~

This transformation is an entry point for nGraph transformations that will be applied inside MOC. And in future this transformations container will be filled with transformations pipeline but now it remains empty. :ref:`More...<details-classngraph_1_1pass_1_1_m_o_c_transformations>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <moc_transformations.hpp>
	
	class MOCTransformations: public :ref:`ov::pass::ModelPass<doxid-classov_1_1pass_1_1_model_pass>`
	{
	public:
		// construction
	
		:ref:`MOCTransformations<doxid-classngraph_1_1pass_1_1_m_o_c_transformations_1a19d3815ae727cf7c6a13e03cf9b3b6c8>`(bool use_shapes, bool low_precision_enabled = true);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classngraph_1_1pass_1_1_m_o_c_transformations_1a5ba0847c05495c3616d63df92bd76333>`("MOCTransformations", "0");
		bool :target:`run_on_model<doxid-classngraph_1_1pass_1_1_m_o_c_transformations_1a96319ea53f01f2f401ce46d19de3302d>`(const std::shared_ptr<:ref:`ngraph::Function<doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>`>& m);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>` :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`;

		// methods
	
		bool :ref:`get_property<doxid-classov_1_1pass_1_1_pass_base_1a3107964f6c4d4bf1d3fbc2bf97ccc0b8>`(const :ref:`PassPropertyMask<doxid-namespaceov_1_1pass_1a4a61a9b72db0e4ed511e6da0d0619e05>`& prop_mask) const;
		void :ref:`set_name<doxid-classov_1_1pass_1_1_pass_base_1a78ddde2a8770041d2f23ce59af908f5d>`(const std::string& name);
		std::string :ref:`get_name<doxid-classov_1_1pass_1_1_pass_base_1a6cd527d2176f1350dd999dc4632a576b>`() const;
		void :ref:`set_callback<doxid-classov_1_1pass_1_1_pass_base_1a6a56827a1cf76be99289bab703982869>`(const :ref:`param_callback<doxid-namespaceov_1_1pass_1a0628acbe84362598648bb66624d4db5c>`& callback);
		virtual void :ref:`set_pass_config<doxid-classov_1_1pass_1_1_pass_base_1abe74bba4b563ad367f2fdc7836016391>`(const std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`>& pass_config);
		std::shared_ptr<:ref:`PassConfig<doxid-classov_1_1pass_1_1_pass_config>`> :ref:`get_pass_config<doxid-classov_1_1pass_1_1_pass_base_1a4902f6ed9322e0fd38810d701f4409df>`();
		bool :ref:`m_transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1a568e5b1f0e01f221d36dffabbf156b3d>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		bool :ref:`transformation_callback<doxid-classov_1_1pass_1_1_pass_base_1aa5265bf720996877709aa990f49d2dab>`(const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node);
		virtual const :ref:`type_info_t<doxid-classov_1_1pass_1_1_pass_base_1a91aae259b4676ba5aca057d542d44b77>`& :ref:`get_type_info<doxid-classov_1_1pass_1_1_pass_base_1ab7020db2fcebc9b6e0741a451778fb0c>`() const = 0;
		:ref:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_model_pass_1a718f43e809339887547f5c96b84ea00a>`("ov::pass::ModelPass");
		virtual bool :ref:`run_on_function<doxid-classov_1_1pass_1_1_model_pass_1a58cf259fa3f2d8b565e6929832656aa9>`(std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> m);
		virtual bool :ref:`run_on_model<doxid-classov_1_1pass_1_1_model_pass_1afdce6ef577b36b5127115dd574b6615e>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);

.. _details-classngraph_1_1pass_1_1_m_o_c_transformations:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This transformation is an entry point for nGraph transformations that will be applied inside MOC. And in future this transformations container will be filled with transformations pipeline but now it remains empty.

Construction
------------

.. _doxid-classngraph_1_1pass_1_1_m_o_c_transformations_1a19d3815ae727cf7c6a13e03cf9b3b6c8:
.. index:: pair: function; MOCTransformations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MOCTransformations(bool use_shapes, bool low_precision_enabled = true)

use_shapes = True enables transformations which are depends on shapes and also it enables ConstantFolding for all ShapeOf operations.

low_precision_enabled = True enables preserving mechanisms that helps to keep :ref:`low_precision <doxid-namespacengraph_1_1pass_1_1low__precision>` sub-graphs as is.


