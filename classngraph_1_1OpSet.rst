.. index:: pair: class; ngraph::OpSet
.. _doxid-classngraph_1_1_op_set:

class ngraph::OpSet
===================



Overview
~~~~~~~~

Run-time opset information. :ref:`More...<details-classngraph_1_1_op_set>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <opset.hpp>
	
	class OpSet: public :ref:`ov::OpSet<doxid-classov_1_1_op_set>`
	{
	public:
		// construction
	
		:target:`OpSet<doxid-classngraph_1_1_op_set_1a7fcc4795c98b79775de428372409c11a>`(const :ref:`ov::OpSet<doxid-classov_1_1_op_set>`& opset);
		:target:`OpSet<doxid-classngraph_1_1_op_set_1aee9c87de0c41836b1a60e9029585fd18>`(const ngraph::OpSet& opset);
		:target:`OpSet<doxid-classngraph_1_1_op_set_1ac0488feca0f8b36764d0db4d14a39105>`();

		// methods
	
		void :ref:`insert<doxid-classngraph_1_1_op_set_1a5a5478fe06760fccc029cf2c6978b7aa>`(
			const std::string& name,
			const :ref:`NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>`& type_info,
			:ref:`FactoryRegistry<doxid-classngraph_1_1_factory_registry>`<Node>::Factory factory
			);
	
		template <typename OP_TYPE>
		void :ref:`insert<doxid-classngraph_1_1_op_set_1a1135d2b2dd280ca5a9ffb8c2e7440318>`(const std::string& name);
	
		template <
			typename OP_TYPE,
			typename std::enable_if<ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
			>
		void :ref:`insert<doxid-classngraph_1_1_op_set_1accc75fdcc632e191ba54ca4b132a6a78>`();
	
		:ref:`ngraph::FactoryRegistry<doxid-classngraph_1_1_factory_registry>`<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& :target:`get_factory_registry<doxid-classngraph_1_1_op_set_1a190ce4f7ccd4b00b0dc6cb5c9c0df228>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		std::set<:ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`>::size_type :ref:`size<doxid-classov_1_1_op_set_1af7baacd0daba5fddc1868444f126dd72>`() const;
	
		template <
			typename OP_TYPE,
			typename std::enable_if<!ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
			>
		void :ref:`insert<doxid-classov_1_1_op_set_1a17f280805e1f81b17c73631d9f767104>`(const std::string& name);
	
		template <
			typename OP_TYPE,
			typename std::enable_if<!ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
			>
		void :ref:`insert<doxid-classov_1_1_op_set_1a6fb32121037c5421c895c059ec36aa33>`();
	
		const std::set<:ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`>& :ref:`get_types_info<doxid-classov_1_1_op_set_1a7a5c1e9b57266d8d40388abce774a682>`() const;
		:ref:`ov::Node<doxid-classov_1_1_node>` \* :ref:`create<doxid-classov_1_1_op_set_1a95eaee3cf7988eadcc6f1d319e7318ee>`(const std::string& name) const;
		:ref:`ov::Node<doxid-classov_1_1_node>` \* :ref:`create_insensitive<doxid-classov_1_1_op_set_1a76cd2dd6326685cab19e66c5dc6f4541>`(const std::string& name) const;
		bool :ref:`contains_type<doxid-classov_1_1_op_set_1a4d266ed2b9ec6f8857cd762189571f89>`(const :ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`& type_info) const;
	
		template <
			typename OP_TYPE,
			typename std::enable_if<!ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
			>
		bool :ref:`contains_type<doxid-classov_1_1_op_set_1a80a205e0b020ba0f580bccaba10a208c>`() const;
	
		bool :ref:`contains_type<doxid-classov_1_1_op_set_1a5b07eb740d6de1cfcd060a72a7d3deba>`(const std::string& name) const;
		bool :ref:`contains_type_insensitive<doxid-classov_1_1_op_set_1ab1db6e8c1a8d4a32cfac9b1aad72453b>`(const std::string& name) const;
		bool :ref:`contains_op_type<doxid-classov_1_1_op_set_1a3a0cb9050fdce50a8f80d4435e9c3d8b>`(const :ref:`Node<doxid-classov_1_1_node>` \* node) const;
		const std::set<:ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`>& :ref:`get_type_info_set<doxid-classov_1_1_op_set_1a87677b561c9f1f3dacd5296ee635cb9a>`() const;

.. _details-classngraph_1_1_op_set:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Run-time opset information.

Methods
-------

.. _doxid-classngraph_1_1_op_set_1a5a5478fe06760fccc029cf2c6978b7aa:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void insert(
		const std::string& name,
		const :ref:`NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>`& type_info,
		:ref:`FactoryRegistry<doxid-classngraph_1_1_factory_registry>`<Node>::Factory factory
		)

Insert an op into the opset with a particular name and factory.

.. _doxid-classngraph_1_1_op_set_1a1135d2b2dd280ca5a9ffb8c2e7440318:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename OP_TYPE>
	void insert(const std::string& name)

Insert OP_TYPE into the opset with a special name and the default factory.

.. _doxid-classngraph_1_1_op_set_1accc75fdcc632e191ba54ca4b132a6a78:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename OP_TYPE,
		typename std::enable_if<ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
		>
	void insert()

Insert OP_TYPE into the opset with the default name and factory.


