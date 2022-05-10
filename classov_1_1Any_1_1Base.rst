.. index:: pair: class; ov::Any::Base
.. _doxid-classov_1_1_any_1_1_base:

class ov::Any::Base
===================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class Base: public std::enable_shared_from_this< Base >
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Base> :target:`Ptr<doxid-classov_1_1_any_1_1_base_1a28a10be34cb0d747b7c918c8c6297566>`;

		// methods
	
		void :target:`type_check<doxid-classov_1_1_any_1_1_base_1a8758ada553cb49fc31cce118c6c5824b>`(const std::type_info&) const;
		virtual const std::type_info& :target:`type_info<doxid-classov_1_1_any_1_1_base_1a20af16417797017296af1d382baa7291>`() const = 0;
		virtual std::vector<std::type_index> :target:`base_type_info<doxid-classov_1_1_any_1_1_base_1a19890cce151db67735d71e88ffd1474e>`() const = 0;
		virtual const void \* :target:`addressof<doxid-classov_1_1_any_1_1_base_1aebd85cb306161e65ebde611e3569cd8e>`() const = 0;
		void \* :target:`addressof<doxid-classov_1_1_any_1_1_base_1aaa9b2a5329af08ec872f30a0b17abdc8>`();
		virtual Base::Ptr :target:`copy<doxid-classov_1_1_any_1_1_base_1aa3072482779a6ce0f61ab46252e94ee1>`() const = 0;
		virtual bool :target:`equal<doxid-classov_1_1_any_1_1_base_1a9d87ef70fc66d04ddf90218c4299b887>`(const Base& rhs) const = 0;
		virtual void :target:`print<doxid-classov_1_1_any_1_1_base_1a4fe74264240c294ecfb15f9cb5aeec6c>`(std::ostream& os) const = 0;
		virtual void :target:`read<doxid-classov_1_1_any_1_1_base_1af7bd5e5db20a8ae54626571092afb63e>`(std::istream& os) = 0;
		void :target:`read_to<doxid-classov_1_1_any_1_1_base_1a8dc7b6b53f88f863ed8191587d62fe5d>`(Base& other) const;
		virtual const :ref:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info>`& :target:`get_type_info<doxid-classov_1_1_any_1_1_base_1aae05a68f42120633b42eb180d4e7b900>`() const = 0;
		virtual std::shared_ptr<:ref:`RuntimeAttribute<doxid-classov_1_1_runtime_attribute>`> :target:`as_runtime_attribute<doxid-classov_1_1_any_1_1_base_1aaaf7fbe4f23422f0a59c23556ea8a09e>`() const;
		virtual bool :target:`is_copyable<doxid-classov_1_1_any_1_1_base_1ac2c59e9241dd578e4ab040300dd93094>`() const;
		virtual :ref:`Any<doxid-classov_1_1_any>` :target:`init<doxid-classov_1_1_any_1_1_base_1a83312d93bea28023929725e28cdaebc5>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
		virtual :ref:`Any<doxid-classov_1_1_any>` :target:`merge<doxid-classov_1_1_any_1_1_base_1a930d535955687080160848e06baf05ed>`(const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& nodes);
		virtual std::string :target:`to_string<doxid-classov_1_1_any_1_1_base_1a295404013d6987611e6de60362c1d5d1>`();
		virtual bool :target:`visit_attributes<doxid-classov_1_1_any_1_1_base_1a80d3d4f02c94f86f0771357d19f25b89>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&);
		bool :target:`visit_attributes<doxid-classov_1_1_any_1_1_base_1a63f9749557a5d65f5184a080bf28734a>`(:ref:`AttributeVisitor<doxid-classov_1_1_attribute_visitor>`&) const;
		std::string :target:`to_string<doxid-classov_1_1_any_1_1_base_1a142961ab6b834c2ba8ba5cd97200a3c4>`() const;
		bool :target:`is<doxid-classov_1_1_any_1_1_base_1a799a34120425ce95bb559e7d08f22bed>`(const std::type_info& other) const;
	
		template <class T>
		bool :target:`is<doxid-classov_1_1_any_1_1_base_1a797558103954ca0102a0338a85468b6c>`() const;
	
		template <class T>
		T& :target:`as<doxid-classov_1_1_any_1_1_base_1a94e2f55a397ede8b859bb6edf2878f41>`();
	
		template <class T>
		const T& :target:`as<doxid-classov_1_1_any_1_1_base_1ae74ce79da6160cc541029eab49626081>`() const;

	protected:
	};

