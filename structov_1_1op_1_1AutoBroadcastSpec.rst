.. index:: pair: struct; ov::op::AutoBroadcastSpec
.. _doxid-structov_1_1op_1_1_auto_broadcast_spec:

struct ov::op::AutoBroadcastSpec
================================



Implicit broadcast specification.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	struct AutoBroadcastSpec
	{
		// fields
	
		:ref:`AutoBroadcastType<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>` :target:`m_type<doxid-structov_1_1op_1_1_auto_broadcast_spec_1a0d42b34ec3b072089c67f9bd58a91240>`;
		int64_t :target:`m_axis<doxid-structov_1_1op_1_1_auto_broadcast_spec_1a73d3915f416e985b236e798065a8eb6c>`;
		static const AutoBroadcastSpec :target:`NUMPY<doxid-structov_1_1op_1_1_auto_broadcast_spec_1a795ebf171f5cd0bf91050f1e466a6162>`;
		static const AutoBroadcastSpec :target:`NONE<doxid-structov_1_1op_1_1_auto_broadcast_spec_1aa036f0cf98d7bd2181340352ac56f282>`;

		// construction
	
		:target:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec_1aedcd8269a4b12550fe8fa09c555e5a31>`();
		:target:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec_1a28a88c5c4ec20e3d906a7961a410f6a0>`(:ref:`AutoBroadcastType<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>` type);
		:target:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec_1a4abd2e94fce160a40f282e934528e177>`(const char \* type);
		:target:`AutoBroadcastSpec<doxid-structov_1_1op_1_1_auto_broadcast_spec_1ae09151354e6da59b05e53dac6e93f10f>`(:ref:`AutoBroadcastType<doxid-namespaceov_1_1op_1a8712da46ddf6f14ef5a6f46a82219ace>` type, int64_t axis);

		// methods
	
		bool :target:`operator ==<doxid-structov_1_1op_1_1_auto_broadcast_spec_1ab55f890880c92e98703e136d3ac4e48c>` (const AutoBroadcastSpec& a) const;
		bool :target:`operator !=<doxid-structov_1_1op_1_1_auto_broadcast_spec_1a859e2cabcbe49505eaa7710be95b17c5>` (const AutoBroadcastSpec& a) const;
	};

