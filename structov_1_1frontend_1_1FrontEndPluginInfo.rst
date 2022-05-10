.. index:: pair: struct; ov::frontend::FrontEndPluginInfo
.. _doxid-structov_1_1frontend_1_1_front_end_plugin_info:

struct ov::frontend::FrontEndPluginInfo
=======================================



Each frontend plugin is responsible to export GetFrontEndData function returning heap-allocated pointer to this structure. Will be used by :ref:`FrontEndManager <doxid-classov_1_1frontend_1_1_front_end_manager>` during loading of plugins.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <manager.hpp>
	
	struct FrontEndPluginInfo
	{
		// fields
	
		std::string :target:`m_name<doxid-structov_1_1frontend_1_1_front_end_plugin_info_1a0cdf945cec201e6d56743980c52c80c1>`;
		:ref:`FrontEndFactory<doxid-namespaceov_1_1frontend_1ac5dc4ee362133b5e540e65cb606567f0>` :target:`m_creator<doxid-structov_1_1frontend_1_1_front_end_plugin_info_1a359db5a13d2b3ce140a5052c15dc2446>`;
	};

