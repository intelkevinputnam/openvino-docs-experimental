.. index:: pair: namespace; ov::intel_myriad::hddl
.. _doxid-namespaceov_1_1intel__myriad_1_1hddl:

namespace ov::intel_myriad::hddl
================================



Namespace with Intel HDDL specific properties.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace hddl {

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> :ref:`device_num<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga9740aba723611275b3803112164753f3>` {"HDDL_DEVICE_NUM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<float>, PropertyMutability::RO> :ref:`device_thermal<doxid-group__ov__runtime__hddl__prop__cpp__api_1gae552f18765b483940fd01650fde95851>` {"HDDL_DEVICE_THERMAL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> :ref:`device_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1gacf4f1614d58d0d3935a3b397b00f6842>` {"HDDL_DEVICE_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<int>, PropertyMutability::RO> :ref:`device_subclass<doxid-group__ov__runtime__hddl__prop__cpp__api_1gac560203cf781593c05025723d3d5451c>` {"HDDL_DEVICE_SUBCLASS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> :ref:`device_memory_total<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga0259592ec2148de4810110831b0f8b6f>` {     "HDDL_DEVICE_MEMORY_TOTAL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> :ref:`device_memory_used<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga3458dd969123814b14c9e890ee24e4fc>` {     "HDDL_DEVICE_MEMORY_USED"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<float>, PropertyMutability::RO> :ref:`device_utilization<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga2efc734e51f387bbfc338e919a51c805>` {"HDDL_DEVICE_UTILIZATION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`stream_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1gafea8b6c0cf6c262ec49d6d18a4c93658>` {"HDDL_STREAM_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`device_tag<doxid-group__ov__runtime__hddl__prop__cpp__api_1gabd3a69621f032384ec51362f0aff60fc>` {"HDDL_DEVICE_TAG"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<int>, PropertyMutability::RO> :ref:`group_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga96d3511530edce78a2a4cceaf1e9f81d>` {"HDDL_GROUP_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> :ref:`device_group_using_num<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga186c1f3f7544108ff70e8c610238b8e9>` {"HDDL_DEVICE_GROUP_USING_NUM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> :ref:`device_total_num<doxid-group__ov__runtime__hddl__prop__cpp__api_1gab63aacf49ad9858d0949922f00031191>` {"HDDL_DEVICE_TOTAL_NUM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`graph_tag<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga84172e57b3d168c126b039830406be21>` {"HDDL_GRAPH_TAG"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`set_stream_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga591d5aa119bb7307c8251f1f971a4df1>` {"HDDL_SET_STREAM_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`set_device_tag<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga9ae718698f02a76ebb88cb6f4e5513c6>` {"HDDL_SET_DEVICE_TAG"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`bind_device<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga268df1558aba168766995fdf764d5db2>` {"HDDL_BIND_DEVICE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`runtime_priority<doxid-group__ov__runtime__hddl__prop__cpp__api_1gab920a771ac462a7e0290834231ecb90f>` {"HDDL_RUNTIME_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`use_sgad<doxid-group__ov__runtime__hddl__prop__cpp__api_1gaeaee6296c19e498f97866806536dc7a7>` {"HDDL_USE_SGAD"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`group_device<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga11893faf0c25782e86653e0e10ae6d17>` {"HDDL_GROUP_DEVICE"};

	} // namespace hddl
