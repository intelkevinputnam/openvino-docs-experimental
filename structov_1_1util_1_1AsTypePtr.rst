.. index:: pair: struct; ov::util::AsTypePtr
.. _doxid-structov_1_1util_1_1_as_type_ptr:

struct ov::util::AsTypePtr
==========================






.. index:: pair: struct; ov::util::AsTypePtr<std::shared_ptr<In>>
.. _doxid-structov_1_1util_1_1_as_type_ptr_3_01std_1_1shared__ptr_3_01_in_01_4_01_4:

struct ov::util::AsTypePtr<std::shared_ptr<In>>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



Casts a std::shared_ptr<Value> to a std::shared_ptr<Type> if it is of type Type, nullptr otherwise


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <type.hpp>
	
	template <typename In>
	struct AsTypePtr<std::shared_ptr<In>>
	{
		// methods
	
		template <typename Type>
		static std::shared_ptr<Type> :target:`call<doxid-structov_1_1util_1_1_as_type_ptr_3_01std_1_1shared__ptr_3_01_in_01_4_01_4_1a12ffa5b2a8e7a689f056b68f1d6438b4>`(const std::shared_ptr<In>& value);
	};

