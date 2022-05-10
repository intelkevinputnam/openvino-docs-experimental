.. index:: pair: class; ov::OpSet
.. _doxid-classov_1_1_op_set:

class ov::OpSet
===============



Overview
~~~~~~~~

Run-time opset information. :ref:`More...<details-classov_1_1_op_set>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <opset.hpp>
	
	class OpSet
	{
	public:
		// methods
	
		std::set<:ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`>::size_type :target:`size<doxid-classov_1_1_op_set_1af7baacd0daba5fddc1868444f126dd72>`() const;
	
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
	
		const std::set<:ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`>& :target:`get_types_info<doxid-classov_1_1_op_set_1a7a5c1e9b57266d8d40388abce774a682>`() const;
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
		const std::set<:ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`>& :target:`get_type_info_set<doxid-classov_1_1_op_set_1a87677b561c9f1f3dacd5296ee635cb9a>`() const;
	};

	// direct descendants

	class :ref:`OpSet<doxid-classngraph_1_1_op_set>`;
.. _details-classov_1_1_op_set:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Run-time opset information.

Methods
-------

.. _doxid-classov_1_1_op_set_1a17f280805e1f81b17c73631d9f767104:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename OP_TYPE,
		typename std::enable_if<!ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
		>
	void insert(const std::string& name)

Insert OP_TYPE into the opset with a special name and the default factory.

.. _doxid-classov_1_1_op_set_1a6fb32121037c5421c895c059ec36aa33:
.. index:: pair: function; insert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename OP_TYPE,
		typename std::enable_if<!ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
		>
	void insert()

Insert OP_TYPE into the opset with the default name and factory.

.. _doxid-classov_1_1_op_set_1a95eaee3cf7988eadcc6f1d319e7318ee:
.. index:: pair: function; create

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Node<doxid-classov_1_1_node>` \* create(const std::string& name) const

Create the op named name using it's factory.

.. _doxid-classov_1_1_op_set_1a76cd2dd6326685cab19e66c5dc6f4541:
.. index:: pair: function; create_insensitive

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ov::Node<doxid-classov_1_1_node>` \* create_insensitive(const std::string& name) const

Create the op named name using it's factory.

.. _doxid-classov_1_1_op_set_1a4d266ed2b9ec6f8857cd762189571f89:
.. index:: pair: function; contains_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool contains_type(const :ref:`NodeTypeInfo<doxid-namespaceov_1a79488905863d76f31e968e3abc04eb62>`& type_info) const

Return true if OP_TYPE is in the opset.

.. _doxid-classov_1_1_op_set_1a80a205e0b020ba0f580bccaba10a208c:
.. index:: pair: function; contains_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		typename OP_TYPE,
		typename std::enable_if<!ngraph::HasTypeInfoMember<OP_TYPE>::value, bool>::type = true
		>
	bool contains_type() const

Return true if OP_TYPE is in the opset.

.. _doxid-classov_1_1_op_set_1a5b07eb740d6de1cfcd060a72a7d3deba:
.. index:: pair: function; contains_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool contains_type(const std::string& name) const

Return true if name is in the opset.

.. _doxid-classov_1_1_op_set_1ab1db6e8c1a8d4a32cfac9b1aad72453b:
.. index:: pair: function; contains_type_insensitive

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool contains_type_insensitive(const std::string& name) const

Return true if name is in the opset.

.. _doxid-classov_1_1_op_set_1a3a0cb9050fdce50a8f80d4435e9c3d8b:
.. index:: pair: function; contains_op_type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool contains_op_type(const :ref:`Node<doxid-classov_1_1_node>` \* node) const

Return true if node's type is in the opset.


