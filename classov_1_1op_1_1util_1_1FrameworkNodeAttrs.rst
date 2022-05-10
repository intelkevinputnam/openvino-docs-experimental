.. index:: pair: class; ov::op::util::FrameworkNodeAttrs
.. _doxid-classov_1_1op_1_1util_1_1_framework_node_attrs:

class ov::op::util::FrameworkNodeAttrs
======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <framework_node.hpp>
	
	class FrameworkNodeAttrs
	{
	public:
		// typedefs
	
		typedef std::unordered_map<std::string, std::string> :target:`attrs_t<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a5938401dd8418a52a2317d95348c811e>`;

		// methods
	
		void :target:`set_opset_name<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1ac10b5f933c2a05047a96dd7cb2d17694>`(const std::string& opset_name);
		void :target:`set_type_name<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a04051527c9025557743bc6a1c58da99f>`(const std::string& type_name);
		const std::string& :target:`get_opset_name<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a8a5eea64558877121438a0e0399685ed>`() const;
		const std::string& :target:`get_type_name<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a9b4d9fd1939bf07e631545e6187a8641>`() const;
		attrs_t::iterator :target:`begin<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1af02af58f88ee3775c5f765a05f405350>`();
		attrs_t::iterator :target:`end<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a45ac1a3f33a7d4c08ba9fd54ebe71d57>`();
		attrs_t::const_iterator :target:`begin<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1ae1fda3679f5f0f87021e83bf0497e2f7>`() const;
		attrs_t::const_iterator :target:`end<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a262b3f1db72fe08f2347f866343da9c4>`() const;
		std::string& :target:`operator []<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a574cd557f38fc3a517353b60849e2392>` (const std::string& key);
		std::string :target:`at<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1a7ae88608267d86b6455e3ace399249a3>`(const std::string& key) const;
		bool :target:`operator ==<doxid-classov_1_1op_1_1util_1_1_framework_node_attrs_1ab87648d6caf97fd7e997cfbfc2bcac25>` (const FrameworkNodeAttrs& other) const;
	};

