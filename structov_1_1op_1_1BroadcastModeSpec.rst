.. index:: pair: struct; ov::op::BroadcastModeSpec
.. _doxid-structov_1_1op_1_1_broadcast_mode_spec:

struct ov::op::BroadcastModeSpec
================================



Implicit broadcast specification.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <attr_types.hpp>
	
	struct BroadcastModeSpec
	{
		// fields
	
		:ref:`BroadcastType<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>` :target:`m_type<doxid-structov_1_1op_1_1_broadcast_mode_spec_1a88f4f267313b230b5f118f6373e0e064>`;
		int64_t :target:`m_axis<doxid-structov_1_1op_1_1_broadcast_mode_spec_1a41b8d91e61c5ff9f7213f909d3220cc1>`;

		// construction
	
		:target:`BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec_1a89c970f1c6d4f089791bb5a41ae2d47a>`();
		:target:`BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec_1abbb90930ce33d5030d42b349bcb11dcc>`(:ref:`BroadcastType<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>` type);
		:target:`BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec_1a639bd4ae9f95d46fea46f5b5dc2a3707>`(const char \* type);
		:target:`BroadcastModeSpec<doxid-structov_1_1op_1_1_broadcast_mode_spec_1a9066ea2a79b868b612ccc43d1a8e70a9>`(:ref:`BroadcastType<doxid-namespaceov_1_1op_1a6dc7edf14421aa3ec0072ef976f0bdea>` type, int64_t axis);

		// methods
	
		bool :target:`operator ==<doxid-structov_1_1op_1_1_broadcast_mode_spec_1aa6d16a57ff67e1d0698527597ce423c8>` (const BroadcastModeSpec& a) const;
	};

