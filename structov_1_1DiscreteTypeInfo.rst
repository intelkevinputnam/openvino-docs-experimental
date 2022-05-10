.. index:: pair: struct; ov::DiscreteTypeInfo
.. _doxid-structov_1_1_discrete_type_info:

struct ov::DiscreteTypeInfo
===========================



Overview
~~~~~~~~

Type information for a type system without inheritance; instances have exactly one type not related to any other type. :ref:`More...<details-structov_1_1_discrete_type_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <type.hpp>
	
	struct DiscreteTypeInfo
	{
		// fields
	
		const char \* :target:`name<doxid-structov_1_1_discrete_type_info_1a79f8162ebea17fe26076868b9dd0272f>`;
		uint64_t :target:`version<doxid-structov_1_1_discrete_type_info_1abb086a96cddbf9dfc52664d64ce60b81>`;
		const char \* :target:`version_id<doxid-structov_1_1_discrete_type_info_1ac7d9aa05482a7dd8ff5754d744707286>`;
		const DiscreteTypeInfo \* :target:`parent<doxid-structov_1_1_discrete_type_info_1a04c236feb5e2ff42481469e9bc053761>`;

		// construction
	
		:target:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info_1ae1e95daf45decf140cc509722c1c391c>`();
		:target:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info_1af5e2595da9b9ab7a330c01d06f5fced2>`(const DiscreteTypeInfo&);
		:target:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info_1a571d713d6058f1b2fa093cd126966362>`(DiscreteTypeInfo&&);
	
		:target:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info_1ab663ecf9d8c9818e7b881f5a25dc2dde>`(
			const char \* _name,
			const char \* _version_id,
			const DiscreteTypeInfo \* _parent = nullptr
			);
	
		:target:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info_1ac17477f531a561eedbe11fa0299ca805>`(
			const char \* _name,
			uint64_t _version,
			const DiscreteTypeInfo \* _parent = nullptr
			);
	
		:target:`DiscreteTypeInfo<doxid-structov_1_1_discrete_type_info_1a19a0b10e54f7b161c8ab1357ca1750e8>`(
			const char \* _name,
			uint64_t _version,
			const char \* _version_id,
			const DiscreteTypeInfo \* _parent = nullptr
			);

		// methods
	
		DiscreteTypeInfo& :target:`operator =<doxid-structov_1_1_discrete_type_info_1a45d156912d49cf5ac361b9f546d1e903>` (const DiscreteTypeInfo&);
		:ref:`OPENVINO_SUPPRESS_DEPRECATED_END<doxid-openvino_2core_2deprecated_8hpp_1ac8c3082fae0849f6d58b442d540b5767>` bool :target:`is_castable<doxid-structov_1_1_discrete_type_info_1a83fdbd602ecb416ab4cca3adac14ab64>`(const DiscreteTypeInfo& target_type) const;
		std::string :target:`get_version<doxid-structov_1_1_discrete_type_info_1a2d01b15fbd2f1d3dd8e2a6620611bccf>`() const;
		bool :target:`operator <<doxid-structov_1_1_discrete_type_info_1a3eec35d280c5da58882d188a0b57e449>` (const DiscreteTypeInfo& b) const;
		bool :target:`operator <=<doxid-structov_1_1_discrete_type_info_1a9eb55c31e9841b4774af23b2a969004f>` (const DiscreteTypeInfo& b) const;
		bool :target:`operator ><doxid-structov_1_1_discrete_type_info_1ac002ea1276b311c9ac834ea6f20b800c>` (const DiscreteTypeInfo& b) const;
		bool :target:`operator >=<doxid-structov_1_1_discrete_type_info_1a736f4940b4876b81dc6dc3b82fa165d9>` (const DiscreteTypeInfo& b) const;
		bool :target:`operator ==<doxid-structov_1_1_discrete_type_info_1a19ea80168752af3fcb077c4ce2cdc0ce>` (const DiscreteTypeInfo& b) const;
		bool :target:`operator !=<doxid-structov_1_1_discrete_type_info_1a357f3529438258ff362f02ed332330f2>` (const DiscreteTypeInfo& b) const;
		:target:`operator std::string<doxid-structov_1_1_discrete_type_info_1ab7e5dd855ad9ec03a3f1450860c93398>` () const;
		size_t :target:`hash<doxid-structov_1_1_discrete_type_info_1a18b9faee9d109fbad39f8f17d097d78d>`() const;
		size_t :target:`hash<doxid-structov_1_1_discrete_type_info_1afab34d4c67546a7a8343c6caa37da7fb>`();
	};
.. _details-structov_1_1_discrete_type_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Type information for a type system without inheritance; instances have exactly one type not related to any other type.

Supports three functions, :ref:`ov::is_type\<Type> <doxid-namespaceov_1a419fbed7ac66870aeb53ceda545ed3e9>`, :ref:`ov::as_type\<Type> <doxid-namespaceov_1aa67d0d3a45c34768e631cb1826fd13c9>`, and :ref:`ov::as_type_ptr\<Type> <doxid-namespaceov_1a3ac8bf7de248c459f19154912f9b216f>` for type-safe dynamic conversions via static_cast/static_ptr_cast without using C++ RTTI. Type must have a static type_info member and a virtual get_type_info() member that returns a reference to its type_info member.


