.. index:: pair: group; Runtime information
.. _doxid-group__ie__runtime__attr__api:

Runtime information
===================

.. toctree::
	:hidden:

	Decompression <classov_1_1Decompression.rst>
	DisableFP16Compression <classov_1_1DisableFP16Compression.rst>
	NonconvertibleDivide <classov_1_1NonconvertibleDivide.rst>
	OldApiMapElementType <classov_1_1OldApiMapElementType.rst>
	OldApiMapOrder <classov_1_1OldApiMapOrder.rst>

Overview
~~~~~~~~

A mechanism of runtime information extension. :ref:`More...<details-group__ie__runtime__attr__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`ov::Decompression<doxid-classov_1_1_decompression>`;
	class :ref:`ov::DisableFP16Compression<doxid-classov_1_1_disable_f_p16_compression>`;
	class :ref:`ov::NonconvertibleDivide<doxid-classov_1_1_nonconvertible_divide>`;
	class :ref:`ov::OldApiMapElementType<doxid-classov_1_1_old_api_map_element_type>`;
	class :ref:`ov::OldApiMapOrder<doxid-classov_1_1_old_api_map_order>`;

	// global functions

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`ngraph::getFusedNames<doxid-group__ie__runtime__attr__api_1ga6e1dc6900c46d5648f89f51e62654768>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<std::string> :ref:`ngraph::getFusedNamesVector<doxid-group__ie__runtime__attr__api_1ga927345dceac1f145e05e7b7af4600946>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string :ref:`ov::getPrimitivesPriority<doxid-group__ie__runtime__attr__api_1ga2ff82c72f78777411e625a407823098d>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);

.. _details-group__ie__runtime__attr__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A mechanism of runtime information extension.

Global Functions
----------------

.. _doxid-group__ie__runtime__attr__api_1ga6e1dc6900c46d5648f89f51e62654768:
.. index:: pair: function; getFusedNames

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string ngraph::getFusedNames(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node)

getFusedNames return string with operation names separated by coma in alphabetical order



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node will be used to get :ref:`FusedNames <doxid-classngraph_1_1_fused_names>` attribute

.. _doxid-group__ie__runtime__attr__api_1ga927345dceac1f145e05e7b7af4600946:
.. index:: pair: function; getFusedNamesVector

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::vector<std::string> ngraph::getFusedNamesVector(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node)

getFusedNamesVector return vector of fused names sorted in alphabetical order



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node will be used to get :ref:`FusedNames <doxid-classngraph_1_1_fused_names>` attribute



.. rubric:: Returns:

vector of strings

.. _doxid-group__ie__runtime__attr__api_1ga2ff82c72f78777411e625a407823098d:
.. index:: pair: function; getPrimitivesPriority

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NGRAPH_API<doxid-ngraph__visibility_8hpp_1a20191679dd9789fbe0f132b3a7e4cee3>` std::string ov::getPrimitivesPriority(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node)

getPrimitivesPriority return string with primitive priorities value



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- The node will be used to get :ref:`PrimitivesPriority <doxid-classov_1_1_primitives_priority>` attribute

