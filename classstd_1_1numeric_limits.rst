.. index:: pair: class; std::numeric_limits<ov::bfloat16>
.. _doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4:

class std::numeric_limits<ov::bfloat16>
=======================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <bfloat16.hpp>
	
	template <>
	class numeric_limits<ov::bfloat16>
	{
	public:
		// fields
	
		static constexpr bool :target:`is_specialized<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a27a6ba9e4e51ac69abff314c39955ab8>` = true;
		static constexpr int :target:`digits<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1aaaaf510b64dfd6c9b3d07ee652d0d0c0>` = 7;
		static constexpr int :target:`digits10<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ab863b3c902f70633c71667bed90bfe42>` = 2;
		static constexpr bool :target:`is_signed<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a437c557a2955d16b9af9972cdbfd1371>` = true;
		static constexpr bool :target:`is_integer<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1aa7da2a38a003fd56aa88dafbba53bced>` = false;
		static constexpr bool :target:`is_exact<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a4677d9296f74eede10b7645fc287c68d>` = false;
		static constexpr int :target:`radix<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a8b7a8dce66ad723c916429b0964ea3de>` = 2;
		static constexpr int :target:`min_exponent<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1afab1a017773c1f84bdf39416e9f9402c>` = -125;
		static constexpr int :target:`min_exponent10<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ac6b032d47f9b946066e900118ebff42f>` = -37;
		static constexpr int :target:`max_exponent<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a9ccd60868f3d9cf156c13afcdf6ce477>` = 128;
		static constexpr int :target:`max_exponent10<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ae14f875a886efae1f2b77aa307cee783>` = 38;
		static constexpr bool :target:`has_infinity<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ae54c7f7c9cf5f978248bc53f38709084>` = true;
		static constexpr bool :target:`has_quiet_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1aaad57761c287be9abe77160d20834c99>` = true;
		static constexpr bool :target:`has_signaling_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1abf5f76ebf1aa6f221fd938b5facac138>` = true;
		static constexpr float_denorm_style :target:`has_denorm<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a23519c05c091c11ba800abc2958a04d0>` = denorm_absent;
		static constexpr bool :target:`has_denorm_loss<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a02d3a90e829f2262a407fd3d5fb10d8a>` = false;
		static constexpr bool :target:`is_iec559<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ae17fe2bea55c86ece12eef2b850db758>` = false;
		static constexpr bool :target:`is_bounded<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a85a1522752e7a23781e22fc18fa53bbf>` = false;
		static constexpr bool :target:`is_modulo<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ab8ec99fc21ac47c82a9a1ba088f26707>` = false;
		static constexpr bool :target:`traps<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1addee708a27d9bade3d8935b2611b7803>` = false;
		static constexpr bool :target:`tinyness_before<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a4713b83f4318dfa146d8ce186424ec8a>` = false;
		static constexpr float_round_style :target:`round_style<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a45d4c18027008db446f810a12c7142cf>` = round_to_nearest;

		// methods
	
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`min<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a623ce73626bc6c4acaabaf843a3b6ada>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`max<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a2fbe92d0b0fa9d22a35194181b20e389>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`lowest<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a80324e10f613d5520c3750a09b94d6a4>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`epsilon<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a7f8ca8119397d6a35c0a27914f1e2a27>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`round_error<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1ae6dcedff4a005301c2b7ff931b8226f0>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`infinity<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a5cfbe0d8588ddf272d5e76cb9bc3f548>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`quiet_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a62671965cbdd9fa5740d1ff306f34010>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`signaling_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1af1de8d5515e13cf9d654c7374634dda1>`();
		static constexpr :ref:`ov::bfloat16<doxid-classov_1_1bfloat16>` :target:`denorm_min<doxid-classstd_1_1numeric__limits_3_01ov_1_1bfloat16_01_4_1a7a16464e8ef3069f9761d52b8cec1f28>`();
	};

.. index:: pair: class; std::numeric_limits<ov::float16>
.. _doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4:

class std::numeric_limits<ov::float16>
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <float16.hpp>
	
	template <>
	class numeric_limits<ov::float16>
	{
	public:
		// fields
	
		static constexpr bool :target:`is_specialized<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a19008d985342e41ce329c614cf2254ad>` = true;
		static constexpr int :target:`digits<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1aac983629aec9c6b1966bbe57527052c8>` = 11;
		static constexpr int :target:`digits10<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1ac2449e2356d781def3564a77f4df14d8>` = 3;
		static constexpr bool :target:`is_signed<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1aeb3dce756c4a59e789c6eb0086dce580>` = true;
		static constexpr bool :target:`is_integer<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a6cc3b8b1b0c0c006762ac27d356227b1>` = false;
		static constexpr bool :target:`is_exact<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a23d441f916da8a0eae789ddf4bf392e7>` = false;
		static constexpr int :target:`radix<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a48b20f67bbc1c0adff559881f6059099>` = 2;
		static constexpr int :target:`min_exponent<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a0f591c095eb8c08abef69ed7af05f967>` = -13;
		static constexpr int :target:`min_exponent10<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a527d49d0ad7e0e62f205ffa5ca80b6e9>` = -4;
		static constexpr int :target:`max_exponent<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1abfbd72c0b122fc43b304fce891adc4e9>` = 16;
		static constexpr int :target:`max_exponent10<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1aeb04794cc39bfd13cea932ee3c4bb250>` = 4;
		static constexpr bool :target:`has_infinity<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a4269dd13227f34f08c9824b3b9e9121a>` = true;
		static constexpr bool :target:`has_quiet_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a20fe2e4bc56cc8c114152f1d1c77187f>` = true;
		static constexpr bool :target:`has_signaling_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a1681db92af6a031035cdc7c5e1b656e7>` = true;
		static constexpr float_denorm_style :target:`has_denorm<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a8af27f105cb7aad7820dccf2ecb1e723>` = denorm_absent;
		static constexpr bool :target:`has_denorm_loss<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a58b73ccabf674f3b2afb84080a29fbbc>` = false;
		static constexpr bool :target:`is_iec559<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a9c0f6ba06813a02a3020e6df9333b843>` = false;
		static constexpr bool :target:`is_bounded<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1ababca7f4667238a43c560b7e2c4623d0>` = false;
		static constexpr bool :target:`is_modulo<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1afa9d88c8600cd73c8ac97c84877345e0>` = false;
		static constexpr bool :target:`traps<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1ab95fbcbc827068636d26365f3d72d999>` = false;
		static constexpr bool :target:`tinyness_before<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a60f345a3fe62bb7db9bd15e12bca20a4>` = false;
		static constexpr float_round_style :target:`round_style<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1ad54685b549becae1eb8c6d3703570c1f>` = round_to_nearest;

		// methods
	
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`min<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a87b03df9590bdc28aeb389183e041cad>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`max<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a51ba555082d354789d6177bf18b110d2>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`lowest<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a537701e67fa7beb52dd51dc8ffadf98d>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`epsilon<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1ac8eac949a23dcdf8518b8ef0bb38e052>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`round_error<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1ad19dc4feda0c2eff214ee5f000c1a61e>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`infinity<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1afffc4ea73550bf5fe3acd14dbd7b7c20>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`quiet_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a7d88940a5577be4e0b2f9cd343ed9652>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`signaling_NaN<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a86a33f118c0b53eb0da4223d4d485c78>`();
		static constexpr :ref:`ov::float16<doxid-classov_1_1float16>` :target:`denorm_min<doxid-classstd_1_1numeric__limits_3_01ov_1_1float16_01_4_1a5757ed3ee87b19bdac4f7bd120afb1ab>`();
	};

