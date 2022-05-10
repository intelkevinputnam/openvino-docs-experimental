.. index:: pair: struct; ov::Any::Impl<T, typename std::enable_if<!std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type>
.. _doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734:

struct ov::Any::Impl<T, typename std::enable_if<!std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type>
=========================================================================================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <class T>
	struct Impl<T, typename std::enable_if<!std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type>: public ov::Any::Base
	{
		// fields
	
		T :target:`value<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a0024a394544c8dc88b43f7c4e89999e1>`;

		// construction
	
		template <typename... Args>
		:target:`Impl<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1afec28bffaf38fbf0640871774addc909>`(Args&&... args);

		// methods
	
		:target:`OPENVINO_RTTI<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1ad66db639c6d8a0709ee99067f2e1d089>`(typeid(T).name());
		const std::type_info& :target:`type_info<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a8d1ffda33be3e444d591bb26be49f7ec>`() const;
		const void \* :target:`addressof<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a3115d9094b523d84d524eb67fceb09e3>`() const;
		Base::Ptr :target:`copy<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a0da36d18c3c349dcd835a788891ff785>`() const;
		std::vector<std::type_index> :target:`base_type_info<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a85e4b1a6bae1c78c293e62a730befa1b>`() const;
		bool :target:`equal<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a8d3b3cce57decaa67b55f690f1521e15>`(const Base& rhs) const;
		void :target:`print<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a77105845f9e36a993da5bf3316c896f2>`(std::ostream& os) const;
		void :target:`read<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_9std_1_1is__convertible_3_083409bd45442b6084ae9ed049ebc3734_1a57dd16227f303045e84a414036788f45>`(std::istream& is);
	};

.. index:: pair: struct; ov::Any::Impl<T, typename std::enable_if<std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type>
.. _doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1:

struct ov::Any::Impl<T, typename std::enable_if<std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	template <class T>
	struct Impl<T, typename std::enable_if<std::is_convertible<T, std::shared_ptr<RuntimeAttribute>>::value>::type>: public ov::Any::Base
	{
		// fields
	
		T :target:`runtime_attribute<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1aca1379c2e6c296e290c0b3d0ea64bb40>`;

		// construction
	
		:target:`Impl<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a7716682c0b3e980acdb99a6a6c71ed19>`(const T& runtime_attribute);

		// methods
	
		const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a688ca394c06c3a46153c84901d367430>`() const;
		std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :target:`as_runtime_attribute<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1acc36455ad6d55268ebf98df57272c09d>`() const;
		bool :target:`is_copyable<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a8870485c4a269033ce9320629403aa6e>`() const;
		:ref:`Any<doxid-classov_1_1_any>` :target:`init<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a5887af1798dce6211bb2aac142a93212>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
		:ref:`Any<doxid-classov_1_1_any>` :target:`merge<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1aa0cdff1a0203bca1575629e053a0c4bb>`(const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& nodes);
		std::string :target:`to_string<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1acee9265d17142b27912152c1ca90f5d3>`();
		bool :target:`visit_attributes<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a40bf498a6ae62cf725ce734656023b0c>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`& visitor);
		const std::type_info& :target:`type_info<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a2d2080f4c897a3d464f0e9fdec175f75>`() const;
		std::vector<std::type_index> :target:`base_type_info<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a725a7080efdd72edf7789bdc827d786f>`() const;
		const void \* :target:`addressof<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a958cb3f1dad2abf79e15a43b25a7331a>`() const;
		Base::Ptr :target:`copy<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a8b3033447510b8ab81a0c1445a0a7575>`() const;
		bool :target:`equal<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1ac9f405e01c0926790aceb9d821d3cb77>`(const Base& rhs) const;
		void :target:`print<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a0d5fb122ffdb99ef9ad81e6a56074455>`(std::ostream& os) const;
		void :target:`read<doxid-structov_1_1_any_1_1_impl_3_01_t_00_01typename_01std_1_1enable__if_3_01std_1_1is__convertible_3_84b6d20fb2b04dc7a31242da3ec425a1_1a774c01c8213ce4c81079f3bc73d73b82>`(std::istream&);
	};

.. index:: pair: struct; ov::Any::Impl
.. _doxid-structov_1_1_any_1_1_impl:

struct ov::Any::Impl
^^^^^^^^^^^^^^^^^^^^






