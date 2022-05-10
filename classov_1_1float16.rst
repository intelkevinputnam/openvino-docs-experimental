.. index:: pair: class; ov::float16
.. _doxid-classov_1_1float16:

class ov::float16
=================

.. toctree::
	:hidden:

	F32 <unionov_1_1float16_1_1F32.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <float16.hpp>
	
	class float16
	{
	public:
		// unions
	
		union :ref:`F32<doxid-unionov_1_1float16_1_1_f32>`;

		// fields
	
		static constexpr uint32_t :target:`frac_size<doxid-classov_1_1float16_1a3babdcb9de060d22bfe1dff9f01ec763>` = 10;
		static constexpr uint32_t :target:`exp_size<doxid-classov_1_1float16_1a711fc5729181571ea922bbde78b5de0b>` = 5;
		static constexpr uint32_t :target:`exp_bias<doxid-classov_1_1float16_1a33e2e5a6fa801ccde1f98552f7c11394>` = 15;

		// construction
	
		:target:`float16<doxid-classov_1_1float16_1afde571d3fc3111713105e3e0c798d789>`();
		:target:`float16<doxid-classov_1_1float16_1af68701ac2c6f68e18275670ad05824c4>`(uint32_t sign, uint32_t biased_exponent, uint32_t fraction);
		:target:`float16<doxid-classov_1_1float16_1a9c1fbd15b432dd3f7f27d2a33ecded6c>`(float value);
	
		template <typename I>
		:target:`float16<doxid-classov_1_1float16_1aa0fa10721f3c91c3aff1ae06ed52e1fe>`(I value);

		// methods
	
		std::string :target:`to_string<doxid-classov_1_1float16_1a6172f7e83d6c987cd92b02700d4ab800>`() const;
		size_t :target:`size<doxid-classov_1_1float16_1a09e215ed0b1a36e9bdc50eb54cd10d98>`() const;
	
		template <typename T>
		bool :target:`operator ==<doxid-classov_1_1float16_1a170eb6a455ea2a5aec290472ed908f5c>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator !=<doxid-classov_1_1float16_1a62d7bc598c91aeab3537ddd7ff4f7a96>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator <<doxid-classov_1_1float16_1aff79094f27d8b4bb86be444a1828f37b>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator <=<doxid-classov_1_1float16_1afaeeef9c64f65e1b4d2313e48addbd41>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator ><doxid-classov_1_1float16_1aa7d77a66d77f4c034ace1ba89fe34521>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator >=<doxid-classov_1_1float16_1a23fab4ed46c1184affd481f15003c7b3>` (const T& other) const;
	
		template <typename T>
		float16 :target:`operator +<doxid-classov_1_1float16_1a0b4efe52a9128ce6931a8496bf37c092>` (const T& other) const;
	
		template <typename T>
		float16 :target:`operator +=<doxid-classov_1_1float16_1a92817564aead0e8934ea842bf33016ba>` (const T& other);
	
		template <typename T>
		float16 :target:`operator -<doxid-classov_1_1float16_1a005f4bb0c63922a32882977e586b9363>` (const T& other) const;
	
		template <typename T>
		float16 :target:`operator -=<doxid-classov_1_1float16_1acf3c1a55c87fd6189e8e4c17a55cca58>` (const T& other);
	
		template <typename T>
		float16 :target:`operator\*<doxid-classov_1_1float16_1a7bca2682cbb6f440751e2363d98715c4>` (const T& other) const;
	
		template <typename T>
		float16 :target:`operator\*=<doxid-classov_1_1float16_1a44a20bc6eba55df76f720ae342a270d5>` (const T& other);
	
		template <typename T>
		float16 :target:`operator/<doxid-classov_1_1float16_1a56741d5b88e2ef09938ad407b2fe0180>` (const T& other) const;
	
		template <typename T>
		float16 :target:`operator/=<doxid-classov_1_1float16_1a460fb8654fcc0f09c2a60df8478ef83c>` (const T& other);
	
		:target:`operator float<doxid-classov_1_1float16_1a7df887043613f8942392373d63dfad20>` () const;
		uint16_t :target:`to_bits<doxid-classov_1_1float16_1a5aea9c28853a59072d59cc5aff2f563c>`() const;
		static constexpr float16 :target:`from_bits<doxid-classov_1_1float16_1aa3ee051b6a90a1fb1ac2e8d71b42ca01>`(uint16_t bits);
	};

