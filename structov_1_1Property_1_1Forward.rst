.. index:: pair: struct; ov::Property::Forward
.. _doxid-structov_1_1_property_1_1_forward:

struct ov::Property::Forward
============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <typename V>
	struct Forward
	{
		// fields
	
		V&& :target:`value<doxid-structov_1_1_property_1_1_forward_1abc21c69afaa9c2494675b6414f31dae6>`;

		// methods
	
		template <
			typename U,
			typename std::enable_if<!std::is_same<typename std::decay<U>::type, std::string>::value&&!std::is_convertible<V, std::string>::value, bool>::type = true
			>
		:target:`operator U<doxid-structov_1_1_property_1_1_forward_1ad6cf3b5131d18cbbd93c6a39fe0d78ff>` ();
	};

