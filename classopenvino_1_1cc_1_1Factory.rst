.. index:: pair: class; openvino::cc::Factory
.. _doxid-classopenvino_1_1cc_1_1_factory:

class openvino::cc::Factory
===========================






.. index:: pair: class; openvino::cc::Factory<Key, T(Args...)>
.. _doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4:

class openvino::cc::Factory<Key, T(Args...)>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. toctree::
	:hidden:

	Factory <structopenvino_1_1cc_1_1Factory_1_1Factory.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <factory.h>
	
	template <typename Key, typename T, typename... Args>
	class Factory<Key, T(Args...)>
	{
	public:
		// typedefs
	
		typedef std::function<T(Args...)> :target:`builder_t<doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1a02dd52fce82d5b667b7503e9eada805b>`;

		// structs
	
		template <typename K>
		struct :ref:`Factory<Key, T(Args...)><doxid-structopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1_1_enum_class_hash>`;

		// construction
	
		:target:`Factory<doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1adde8cb85def522b7f1c48d24bfac5097>`(const std::string& name);

		// methods
	
		template <typename Impl>
		void :target:`registerImpl<doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1ab9c7fabbd33c73e50891740e46258c67>`(const Key& key);
	
		T :target:`createImpl<doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1ada85044308e5b0068e1a56ccd12a6bfe>`(const Key& key, Args... args);
	
		template <typename Fn>
		void :target:`foreach<doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1a9236130e8b2851e9b72e5cfbefaafd99>`(Fn fn) const;
	
		size_t :target:`size<doxid-classopenvino_1_1cc_1_1_factory_3_01_key_00_01_t_07_args_8_8_8_08_4_1a8f66b58fd9bd5a7df260efe2171ea03c>`() const;
	};

