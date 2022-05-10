.. index:: pair: struct; ov::RawNodeOutput
.. _doxid-structov_1_1_raw_node_output:

struct ov::RawNodeOutput
========================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <node.hpp>
	
	struct RawNodeOutput
	{
		// fields
	
		:ref:`Node<doxid-classov_1_1_node>` \* :target:`node<doxid-structov_1_1_raw_node_output_1af7ea87233d0630b154cc23b88c7c1889>`;
		size_t :target:`index<doxid-structov_1_1_raw_node_output_1a04ad53d3abb5830b7a3a313b84bbdad4>` {0};

		// construction
	
		:target:`RawNodeOutput<doxid-structov_1_1_raw_node_output_1ae841dc0498dd8cf9461ade19b4369165>`(const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& value);
		:target:`RawNodeOutput<doxid-structov_1_1_raw_node_output_1af074b4db03f36382573e9b4d08db95cc>`(:ref:`Node<doxid-classov_1_1_node>` \* node, size_t index);
		:target:`RawNodeOutput<doxid-structov_1_1_raw_node_output_1ad6561e45a114396d7e041efa151f4ce7>`(const RawNodeOutput&);
		:target:`RawNodeOutput<doxid-structov_1_1_raw_node_output_1a0af73ce001b06989f30ea53a2f4cd1b4>`();

		// methods
	
		RawNodeOutput& :target:`operator =<doxid-structov_1_1_raw_node_output_1a144fbb4b5ff7ac7d481e327fdd00d074>` (const RawNodeOutput&);
		:target:`operator Output< Node ><doxid-structov_1_1_raw_node_output_1a611d0c19c01117bc20ffe98aeadb9458>` ();
		bool :target:`operator ==<doxid-structov_1_1_raw_node_output_1a8545f0c3826f7a10be8658a7f7535b90>` (const RawNodeOutput& other) const;
		bool :target:`operator !=<doxid-structov_1_1_raw_node_output_1aecba61ca4868ea7e77a1b4441121a9c7>` (const RawNodeOutput& other) const;
		bool :target:`operator <<doxid-structov_1_1_raw_node_output_1afa619b10e8918984800e040e57cc04de>` (const RawNodeOutput& other) const;
		bool :target:`operator ><doxid-structov_1_1_raw_node_output_1a67f027210a9704167e3a9984b0573d18>` (const RawNodeOutput& other) const;
		bool :target:`operator <=<doxid-structov_1_1_raw_node_output_1a6416e9ca2c3a623923d33e00b6e8082b>` (const RawNodeOutput& other) const;
		bool :target:`operator >=<doxid-structov_1_1_raw_node_output_1add36d80d5431692ca0995aec9a26e25c>` (const RawNodeOutput& other) const;
	};

