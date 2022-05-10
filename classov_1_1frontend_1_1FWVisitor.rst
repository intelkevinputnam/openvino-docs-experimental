.. index:: pair: class; ov::frontend::FWVisitor
.. _doxid-classov_1_1frontend_1_1_f_w_visitor:

class ov::frontend::FWVisitor
=============================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <op.hpp>
	
	class FWVisitor: public :ref:`ov::AttributeVisitor<doxid-classov_1_1_attribute_visitor>`
	{
	public:
		// construction
	
		:target:`FWVisitor<doxid-classov_1_1frontend_1_1_f_w_visitor_1a7800ca0f695a01e6a1eef3b383454ae8>`(
			const :ref:`NodeContext<doxid-classov_1_1frontend_1_1_node_context>`& context,
			const std::map<std::string, std::string>& attr_names_map = {},
			const std::map<std::string, :ref:`ov::Any<doxid-classov_1_1_any>`>& attr_values_map = {}
			);

		// methods
	
		virtual void :ref:`on_adapter<doxid-classov_1_1frontend_1_1_f_w_visitor_1ad093c895d1a8f4228ee8b3b0ad2fb350>`(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<void>& adapter);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::string :ref:`node_id_t<doxid-classov_1_1_attribute_visitor_1a10f4bb94faebc77286c7931404d1ca4c>`;

		// fields
	
		static constexpr const char \* :ref:`invalid_node_id<doxid-classov_1_1_attribute_visitor_1a62abdd33ddb8bb70d22c81316c81b97b>` = "";

		// methods
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1aa2db9dc01b6d21ec1644b40396e99e1b>`(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<void>& adapter) = 0;
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1ae08b407f5829871d6d850bcb26f801e1>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<void \*>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1aa1cb0900beccd00eb640e9a11efe52da>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::string>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a691a8d0e40b3e70bf5d9cc4468e032b3>`(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<bool>& adapter);
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a7d087ad13319989b5d9e5e5bb56b650b>`(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<int8_t>& adapter);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a06c12814b5543ad64e4226335b3d79df>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<int16_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a637eda52d59a4d3967470a044ad27d65>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<int32_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a3dfd5ee1b830cb1bbff325f4bbd0d4af>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<int64_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a2f607f62719405dfa893171ee23d54cf>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<uint8_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1ae2b91a59727fc048cb4167fd80853e51>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<uint16_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1ab6e2428c5a0fd08b2139a1947f555285>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<uint32_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1af75e2fd7fffe9ef6902b5b695bebc2b1>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<uint64_t>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1aefcded594839287d2587a2714bcaca20>`(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<float>& adapter);
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a7a9a1eb11bf583c929e945671a56323e>`(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<double>& adapter);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a3ecc0145eaa0cf7281dccef31bfc1d8d>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<int8_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1ad5b37f92580290296211135daa924d0d>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<int16_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a04d610f7efdcdd23b967ed57fe65dc0e>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<int32_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1ab9313b50eab152dd09c539f7f0881780>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<int64_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a8519a07f9bedc7791e874b7545e48293>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<uint8_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a46d12593fb6b57c9b3f408eb1b973985>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<uint16_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1ac05c5c51116a57a8fa21f4f1158a6730>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<uint32_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a1d14a8c73df592271b09dca328bed485>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<uint64_t>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1aaf6548903e306ad653f552ebf4d68eb9>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<float>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a26d1ec25b4dfebf36de332cdc301272b>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<double>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a712a933606074d8603e636e0711f3291>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::vector<std::string>>& adapter
			);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1a9da5b1a86f11a69162028561be7385b4>`(const std::string& name, :ref:`VisitorAdapter<doxid-classov_1_1_visitor_adapter>`& adapter);
	
		virtual void :ref:`on_adapter<doxid-classov_1_1_attribute_visitor_1adfbeec4b1db804c58d18c859bb272375>`(
			const std::string& name,
			:ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>>& adapter
			);
	
		template <typename AT>
		void :ref:`on_attribute<doxid-classov_1_1_attribute_visitor_1a8323bb5b84f0a074a6fbedf32e0efa6f>`(const std::string& name, AT& value);
	
		const std::vector<std::string>& :ref:`get_context<doxid-classov_1_1_attribute_visitor_1abc801b32f38a08603435968dba835c12>`() const;
		virtual std::string :ref:`get_name_with_context<doxid-classov_1_1_attribute_visitor_1a0007b39f96410caa43df659979cbc22b>`();
		virtual void :ref:`start_structure<doxid-classov_1_1_attribute_visitor_1a891a8b0975fdaf7f31837be466507be8>`(const std::string& name);
		virtual std::string :ref:`finish_structure<doxid-classov_1_1_attribute_visitor_1a7e874cdf8b2cfa95416766c323e3e596>`();
	
		virtual void :ref:`register_node<doxid-classov_1_1_attribute_visitor_1a77c1faa41585ea1d5971ca2ec4492cf4>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
			:ref:`node_id_t<doxid-classov_1_1_attribute_visitor_1a10f4bb94faebc77286c7931404d1ca4c>` id = :ref:`invalid_node_id<doxid-classov_1_1_attribute_visitor_1a62abdd33ddb8bb70d22c81316c81b97b>`
			);
	
		virtual std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :ref:`get_registered_node<doxid-classov_1_1_attribute_visitor_1af5954b2ac96f14f59174764f4a34af22>`(:ref:`node_id_t<doxid-classov_1_1_attribute_visitor_1a10f4bb94faebc77286c7931404d1ca4c>` id);
		virtual :ref:`node_id_t<doxid-classov_1_1_attribute_visitor_1a10f4bb94faebc77286c7931404d1ca4c>` :ref:`get_registered_node_id<doxid-classov_1_1_attribute_visitor_1acf04b80c1569d14fe0cb3cee81cfaa61>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);

.. _details-classov_1_1frontend_1_1_f_w_visitor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. _doxid-classov_1_1frontend_1_1_f_w_visitor_1ad093c895d1a8f4228ee8b3b0ad2fb350:
.. index:: pair: function; on_adapter

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void on_adapter(const std::string& name, :ref:`ValueAccessor<doxid-classov_1_1_value_accessor>`<void>& adapter)

handles all specialized on_adapter methods implemented by the visitor.

The adapter implements get_type_info(), which can be used to determine the adapter directly or via is_type and as_type on any platform


