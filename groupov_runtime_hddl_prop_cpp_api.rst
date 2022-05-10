.. index:: pair: group; Intel HDDL specific properties
.. _doxid-group__ov__runtime__hddl__prop__cpp__api:

Intel HDDL specific properties
==============================



Overview
~~~~~~~~

Set of Intel HDDL specific properties. :ref:`More...<details-group__ov__runtime__hddl__prop__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_num<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga9740aba723611275b3803112164753f3>` {"HDDL_DEVICE_NUM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<float>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_thermal<doxid-group__ov__runtime__hddl__prop__cpp__api_1gae552f18765b483940fd01650fde95851>` {"HDDL_DEVICE_THERMAL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1gacf4f1614d58d0d3935a3b397b00f6842>` {"HDDL_DEVICE_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<int>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_subclass<doxid-group__ov__runtime__hddl__prop__cpp__api_1gac560203cf781593c05025723d3d5451c>` {"HDDL_DEVICE_SUBCLASS"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_memory_total<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga0259592ec2148de4810110831b0f8b6f>` {     "HDDL_DEVICE_MEMORY_TOTAL"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_memory_used<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga3458dd969123814b14c9e890ee24e4fc>` {     "HDDL_DEVICE_MEMORY_USED"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<float>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_utilization<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga2efc734e51f387bbfc338e919a51c805>` {"HDDL_DEVICE_UTILIZATION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::stream_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1gafea8b6c0cf6c262ec49d6d18a4c93658>` {"HDDL_STREAM_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_tag<doxid-group__ov__runtime__hddl__prop__cpp__api_1gabd3a69621f032384ec51362f0aff60fc>` {"HDDL_DEVICE_TAG"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<int>, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::group_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga96d3511530edce78a2a4cceaf1e9f81d>` {"HDDL_GROUP_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_group_using_num<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga186c1f3f7544108ff70e8c610238b8e9>` {"HDDL_DEVICE_GROUP_USING_NUM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> :ref:`ov::intel_myriad::hddl::device_total_num<doxid-group__ov__runtime__hddl__prop__cpp__api_1gab63aacf49ad9858d0949922f00031191>` {"HDDL_DEVICE_TOTAL_NUM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::graph_tag<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga84172e57b3d168c126b039830406be21>` {"HDDL_GRAPH_TAG"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::set_stream_id<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga591d5aa119bb7307c8251f1f971a4df1>` {"HDDL_SET_STREAM_ID"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::set_device_tag<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga9ae718698f02a76ebb88cb6f4e5513c6>` {"HDDL_SET_DEVICE_TAG"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::bind_device<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga268df1558aba168766995fdf764d5db2>` {"HDDL_BIND_DEVICE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::runtime_priority<doxid-group__ov__runtime__hddl__prop__cpp__api_1gab920a771ac462a7e0290834231ecb90f>` {"HDDL_RUNTIME_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::use_sgad<doxid-group__ov__runtime__hddl__prop__cpp__api_1gaeaee6296c19e498f97866806536dc7a7>` {"HDDL_USE_SGAD"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`ov::intel_myriad::hddl::group_device<doxid-group__ov__runtime__hddl__prop__cpp__api_1ga11893faf0c25782e86653e0e10ae6d17>` {"HDDL_GROUP_DEVICE"};

.. _details-group__ov__runtime__hddl__prop__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of Intel HDDL specific properties.

Global Variables
----------------

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga9740aba723611275b3803112164753f3:
.. index:: pair: variable; device_num

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> ov::intel_myriad::hddl::device_num {"HDDL_DEVICE_NUM"}

:ref:`Property <doxid-classov_1_1_property>` to get a int of the device number.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gae552f18765b483940fd01650fde95851:
.. index:: pair: variable; device_thermal

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<float>, PropertyMutability::RO> ov::intel_myriad::hddl::device_thermal {"HDDL_DEVICE_THERMAL"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<float> of device thermal.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gacf4f1614d58d0d3935a3b397b00f6842:
.. index:: pair: variable; device_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> ov::intel_myriad::hddl::device_id {"HDDL_DEVICE_ID"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<uint32> of device ids.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gac560203cf781593c05025723d3d5451c:
.. index:: pair: variable; device_subclass

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<int>, PropertyMutability::RO> ov::intel_myriad::hddl::device_subclass {"HDDL_DEVICE_SUBCLASS"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<int> of device subclasses.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga0259592ec2148de4810110831b0f8b6f:
.. index:: pair: variable; device_memory_total

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> ov::intel_myriad::hddl::device_memory_total {     "HDDL_DEVICE_MEMORY_TOTAL"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<uint32> of device total memory.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga3458dd969123814b14c9e890ee24e4fc:
.. index:: pair: variable; device_memory_used

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<unsigned int>, PropertyMutability::RO> ov::intel_myriad::hddl::device_memory_used {     "HDDL_DEVICE_MEMORY_USED"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<uint32> of device used memory.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga2efc734e51f387bbfc338e919a51c805:
.. index:: pair: variable; device_utilization

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<float>, PropertyMutability::RO> ov::intel_myriad::hddl::device_utilization {"HDDL_DEVICE_UTILIZATION"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<float> of device utilization.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gafea8b6c0cf6c262ec49d6d18a4c93658:
.. index:: pair: variable; stream_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> ov::intel_myriad::hddl::stream_id {"HDDL_STREAM_ID"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<std::string> of stream ids.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gabd3a69621f032384ec51362f0aff60fc:
.. index:: pair: variable; device_tag

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<std::string>, PropertyMutability::RO> ov::intel_myriad::hddl::device_tag {"HDDL_DEVICE_TAG"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<std::string> of device tags.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga96d3511530edce78a2a4cceaf1e9f81d:
.. index:: pair: variable; group_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::vector<int>, PropertyMutability::RO> ov::intel_myriad::hddl::group_id {"HDDL_GROUP_ID"}

:ref:`Property <doxid-classov_1_1_property>` to get a std::vector<int> of group ids.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga186c1f3f7544108ff70e8c610238b8e9:
.. index:: pair: variable; device_group_using_num

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> ov::intel_myriad::hddl::device_group_using_num {"HDDL_DEVICE_GROUP_USING_NUM"}

:ref:`Property <doxid-classov_1_1_property>` to get a int number of device be using for group.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gab63aacf49ad9858d0949922f00031191:
.. index:: pair: variable; device_total_num

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<int, PropertyMutability::RO> ov::intel_myriad::hddl::device_total_num {"HDDL_DEVICE_TOTAL_NUM"}

:ref:`Property <doxid-classov_1_1_property>` to get a int number of total device.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga84172e57b3d168c126b039830406be21:
.. index:: pair: variable; graph_tag

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::graph_tag {"HDDL_GRAPH_TAG"}

[Only for HDDLPlugin] Type: Arbitrary non-empty string. If empty (""), equals no set, default: ""; This option allows to specify the number of MYX devices used for inference a specific Executable network. Note: Only one network would be allocated to one device. The number of devices for the tag is specified in the hddl_service.config file. Example: "service_settings": { "graph_tag_map": { "tagA":3 } } It means that an executable network marked with tagA will be executed on 3 devices

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga591d5aa119bb7307c8251f1f971a4df1:
.. index:: pair: variable; set_stream_id

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::set_stream_id {"HDDL_SET_STREAM_ID"}

[Only for HDDLPlugin] Type: Arbitrary non-empty string. If empty (""), equals no set, default: ""; This config makes the executable networks to be allocated on one certain device (instead of multiple devices). And all inference through this executable network, will be done on this device. Note: Only one network would be allocated to one device. The number of devices which will be used for stream-affinity must be specified in hddl_service.config file. Example: "service_settings": { "stream_device_number":5 } It means that 5 device will be used for stream-affinity

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga9ae718698f02a76ebb88cb6f4e5513c6:
.. index:: pair: variable; set_device_tag

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::set_device_tag {"HDDL_SET_DEVICE_TAG"}

[Only for HDDLPlugin] Type: Arbitrary non-empty string. If empty (""), equals no set, default: ""; This config allows user to control device flexibly. This config gives a "tag" for a certain device while allocating a network to it. Afterward, user can allocating/deallocating networks to this device with this "tag". Devices used for such use case is controlled by a so-called "Bypass Scheduler" in HDDL backend, and the number of such device need to be specified in hddl_service.config file. Example: "service_settings": { "bypass_device_number": 5 } It means that 5 device will be used for Bypass scheduler.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga268df1558aba168766995fdf764d5db2:
.. index:: pair: variable; bind_device

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::bind_device {"HDDL_BIND_DEVICE"}

[Only for HDDLPlugin] Type: "bool", default is "false". This config is a sub-config of DEVICE_TAG, and only available when "DEVICE_TAG" is set. After a user load a network, the user got a handle for the network. If "YES", the network allocated is bind to the device (with the specified "DEVICE_TAG"), which means all afterwards inference through this network handle will be executed on this device only. If "NO", the network allocated is not bind to the device (with the specified "DEVICE_TAG"). If the same network is allocated on multiple other devices (also set BIND_DEVICE to "False"), then inference through any handle of these networks may be executed on any of these devices those have the network loaded.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gab920a771ac462a7e0290834231ecb90f:
.. index:: pair: variable; runtime_priority

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::runtime_priority {"HDDL_RUNTIME_PRIORITY"}

[Only for HDDLPlugin] Type: A signed int wrapped in a string, default is "0". This config is a sub-config of DEVICE_TAG, and only available when "DEVICE_TAG" is set and "BIND_DEVICE" is "False". When there are multiple devices running a certain network (a same network running on multiple devices in Bypass Scheduler), the device with a larger number has a higher priority, and more inference tasks will be fed to it with priority.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1gaeaee6296c19e498f97866806536dc7a7:
.. index:: pair: variable; use_sgad

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::use_sgad {"HDDL_USE_SGAD"}

[Only for HDDLPlugin] Type: "bool", default is "false". SGAD is short for "Single Graph All Device". With this scheduler, once application allocates 1 network, all devices (managed by SGAD scheduler) will be loaded with this graph. The number of network that can be loaded to one device can exceed one. Once application deallocates 1 network from device, all devices will unload the network from them.

.. _doxid-group__ov__runtime__hddl__prop__cpp__api_1ga11893faf0c25782e86653e0e10ae6d17:
.. index:: pair: variable; group_device

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> ov::intel_myriad::hddl::group_device {"HDDL_GROUP_DEVICE"}

[Only for HDDLPlugin] Type: A signed int wrapped in a string, default is "0". This config gives a "group id" for a certain device when this device has been reserved for certain client, client can use this device grouped by calling this group id while other client can't use this device Each device has their own group id. Device in one group shares same group id.

