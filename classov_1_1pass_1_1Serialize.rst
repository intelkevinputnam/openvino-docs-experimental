.. index:: pair: class; ov::pass::Serialize
.. _doxid-classov_1_1pass_1_1_serialize:

class ov::pass::Serialize
=========================

.. toctree::
	:hidden:

	Version <enumov_1_1pass_1_1Serialize_1_1Version.rst>

Overview
~~~~~~~~

:ref:`Serialize <doxid-classov_1_1pass_1_1_serialize>` transformation converts :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` into IR files. :ref:`More...<details-classov_1_1pass_1_1_serialize>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <serialize.hpp>
	
	class Serialize: public :ref:`ov::pass::ModelPass<doxid-classov_1_1pass_1_1_model_pass>`
	{
	public:
		// enums
	
		enum :ref:`Version<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86b>`;

		// construction
	
		:target:`Serialize<doxid-classov_1_1pass_1_1_serialize_1a7eaff690f2b8193ea926be50cd23364b>`(
			std::ostream& xmlFile,
			std::ostream& binFile,
			std::map<std::string, :ref:`ngraph::OpSet<doxid-classngraph_1_1_op_set>`> custom_opsets,
			:ref:`Version<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86b>` version = :ref:`Version::UNSPECIFIED<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86ba1c04cc3823d476c3017238679a0fdf52>`
			);
	
		:target:`Serialize<doxid-classov_1_1pass_1_1_serialize_1a08b4135837f7afc490d6a0bdc38971fd>`(
			std::ostream& xmlFile,
			std::ostream& binFile,
			:ref:`Version<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86b>` version = :ref:`Version::UNSPECIFIED<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86ba1c04cc3823d476c3017238679a0fdf52>`
			);
	
		:target:`Serialize<doxid-classov_1_1pass_1_1_serialize_1a8453e93d0e018b4dcb834748d696511c>`(
			const std::string& xmlPath,
			const std::string& binPath,
			std::map<std::string, :ref:`ngraph::OpSet<doxid-classngraph_1_1_op_set>`> custom_opsets,
			:ref:`Version<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86b>` version = :ref:`Version::UNSPECIFIED<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86ba1c04cc3823d476c3017238679a0fdf52>`
			);
	
		:target:`Serialize<doxid-classov_1_1pass_1_1_serialize_1a988afe82ef4de645d8dcc0e0e8660cbf>`(
			const std::string& xmlPath,
			const std::string& binPath,
			:ref:`Version<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86b>` version = :ref:`Version::UNSPECIFIED<doxid-classov_1_1pass_1_1_serialize_1aa77d8b2fefd8aec27f6d732cc620d86ba1c04cc3823d476c3017238679a0fdf52>`
			);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-classov_1_1pass_1_1_serialize_1afdba905bb8757cd7ffb6602c95c0f832>`("Serialize");
		virtual bool :target:`run_on_model<doxid-classov_1_1pass_1_1_serialize_1a6bdbc000c5a7d0914b8ae5f58084f553>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& m);
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

.. _details-classov_1_1pass_1_1_serialize:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Serialize <doxid-classov_1_1pass_1_1_serialize>` transformation converts :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` into IR files.

* dynamic shapes are not supported

* order of generated layers in xml file is ngraph specific (given by get_ordered_ops()); MO generates file with different order, but they are logically equivalent


