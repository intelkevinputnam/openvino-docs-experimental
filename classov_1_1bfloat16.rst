.. index:: pair: class; ov::bfloat16
.. _doxid-classov_1_1bfloat16:

class ov::bfloat16
==================

.. toctree::
	:hidden:

	F32 <unionov_1_1bfloat16_1_1F32.rst>




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <bfloat16.hpp>
	
	class bfloat16
	{
	public:
		// unions
	
		union :ref:`F32<doxid-unionov_1_1bfloat16_1_1_f32>`;

		// construction
	
		:target:`bfloat16<doxid-classov_1_1bfloat16_1aa19f971bbfebb617a57c94315d6f22ff>`();
		:target:`bfloat16<doxid-classov_1_1bfloat16_1aa176113dc30ffce9b536cb056a4b752b>`(float value);
	
		template <typename I>
		:target:`bfloat16<doxid-classov_1_1bfloat16_1a815e3123437635e3a56129c3fc0d6529>`(I value);

		// methods
	
		std::string :target:`to_string<doxid-classov_1_1bfloat16_1a7ea28c6352466d31a6a6baf67d02c987>`() const;
		size_t :target:`size<doxid-classov_1_1bfloat16_1a2048584ec114db01e412480b5250687d>`() const;
	
		template <typename T>
		bool :target:`operator ==<doxid-classov_1_1bfloat16_1abe2e793e92d809a678bcd3e98d293da3>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator !=<doxid-classov_1_1bfloat16_1a131d44232476433f4b4f33703c1cbb3a>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator <<doxid-classov_1_1bfloat16_1a80f0854eeda5bdde3d7ea3d4aa877a2f>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator <=<doxid-classov_1_1bfloat16_1a21b186f034883e363ee22f8775142375>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator ><doxid-classov_1_1bfloat16_1a9fcd24c947e23aa01240f17644478426>` (const T& other) const;
	
		template <typename T>
		bool :target:`operator >=<doxid-classov_1_1bfloat16_1ac6de0b3a71af807fcc187a6388f8b6c4>` (const T& other) const;
	
		template <typename T>
		bfloat16 :target:`operator +<doxid-classov_1_1bfloat16_1accf98335c469f6cad35b1eb7513bb2de>` (const T& other) const;
	
		template <typename T>
		bfloat16 :target:`operator +=<doxid-classov_1_1bfloat16_1aae560ca417c9cfac662375a2eac2dc14>` (const T& other);
	
		template <typename T>
		bfloat16 :target:`operator -<doxid-classov_1_1bfloat16_1a703250e0e4af9c1bc91dfa5288086aac>` (const T& other) const;
	
		template <typename T>
		bfloat16 :target:`operator -=<doxid-classov_1_1bfloat16_1a15ec0328c4ee9f489d2b40b4aabccd4a>` (const T& other);
	
		template <typename T>
		bfloat16 :target:`operator\*<doxid-classov_1_1bfloat16_1abeae58e2d904327208b15fcf61c5f295>` (const T& other) const;
	
		template <typename T>
		bfloat16 :target:`operator\*=<doxid-classov_1_1bfloat16_1a50797df2536b5edf707c62f2b4c2da77>` (const T& other);
	
		template <typename T>
		bfloat16 :target:`operator/<doxid-classov_1_1bfloat16_1ac2384de98f309c983aca6c33ec2feed2>` (const T& other) const;
	
		template <typename T>
		bfloat16 :target:`operator/=<doxid-classov_1_1bfloat16_1af23d841e328984e8a5a481e10c43526e>` (const T& other);
	
		:target:`operator float<doxid-classov_1_1bfloat16_1af3a87699114214e164f7250da40aad20>` () const;
		uint16_t :target:`to_bits<doxid-classov_1_1bfloat16_1a0997f12b812cf3eb211a04fd126b9756>`() const;
		static std::vector<float> :target:`to_float_vector<doxid-classov_1_1bfloat16_1a3bad54a84e5492e4e63b6f636b3beb18>`(const std::vector<bfloat16>&);
		static std::vector<bfloat16> :target:`from_float_vector<doxid-classov_1_1bfloat16_1a788daaea85bdb099a38b776145ccaedf>`(const std::vector<float>&);
		static constexpr bfloat16 :target:`from_bits<doxid-classov_1_1bfloat16_1a56a83cf6a12277703d32122efa99bee1>`(uint16_t bits);
		static uint16_t :target:`round_to_nearest_even<doxid-classov_1_1bfloat16_1a8506913fc55cff55acb1e7f175da566f>`(float x);
		static uint16_t :target:`round_to_nearest<doxid-classov_1_1bfloat16_1ad04d72f0bdc458644b4f4bbfff60ce04>`(float x);
		static uint16_t :target:`truncate<doxid-classov_1_1bfloat16_1a5a8802725da7d29b58066d845ddc49f1>`(float x);
	};

