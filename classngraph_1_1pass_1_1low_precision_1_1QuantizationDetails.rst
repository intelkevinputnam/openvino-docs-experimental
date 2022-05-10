.. index:: pair: class; ngraph::pass::low_precision::QuantizationDetails
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details:

class ngraph::pass::low_precision::QuantizationDetails
======================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <quantization_details.hpp>
	
	class QuantizationDetails
	{
	public:
		// fields
	
		const size_t :target:`levels<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a4268cb68f91abb2b43d6c9873488616e>`;
		const std::vector<float> :target:`inputLowValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a6b2dda3b2351ce234cda2ddfc22669e8>`;
		const std::vector<float> :target:`inputHighValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a2b19dbc5f1d250cf43725e8b8da1949d>`;
		const std::vector<float> :target:`outputLowValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1ab576f016be92fe63f6f2105926c27e21>`;
		const std::vector<float> :target:`outputHighValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1ab6552d9799d384acbd3f00ecc9bc1f69>`;

		// construction
	
		:target:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a603b366ef6dd854f7ccec8c7aae21596>`();
		:target:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1ab6f9ddbe66ccc62d2aae0d7554ccc0e6>`(const QuantizationDetails& quantizationDetails);
	
		:target:`QuantizationDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a25009e21c4a8ee43b6a2115aea777164>`(
			const size_t levels,
			const std::vector<float>& inputLowValues,
			const std::vector<float>& inputHighValues,
			const std::vector<float>& outputLowValues,
			const std::vector<float>& outputHighValues
			);

		// methods
	
		bool :target:`hasNegativeOutput<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a474aa68ead5b8e53cf8d84775a0f15a5>`() const;
		float :target:`maxOutput<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1ab773d3a15e0febc6f6048422e89a90db>`(const size_t channel) const;
		float :target:`maxInput<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a5ccb4cc75b5e46b48f7a4df63b95dc48>`(const size_t channel) const;
		float :target:`getInputLowValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a92af8d4c58c0b32dbd0892a135465b76>`(const size_t channel) const;
		float :target:`getInputHighValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a31d2647954848fd1eb6d726036331371>`(const size_t channel) const;
		float :target:`getOutputLowValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a2f1c14ccb28e326eac17da7d6318b6cd>`(const size_t channel) const;
		float :target:`getOutputHighValue<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a2b25d87090a1fbbb05984c2706f0764d>`(const size_t channel) const;
		bool :target:`empty<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a90faf7ed32c800727d01bf5252a80bdf>`() const;
	
		static bool :target:`outputLayoutIsSupported<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a6be85add753ef35269d26b49abb974e4>`(
			std::shared_ptr<opset1::FakeQuantize> quantize,
			bool isConvertExpected = false
			);
	
		static void :target:`getInputIntervals<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1aec1ce4a6e1bdb27805a9c38d02104275>`(
			std::shared_ptr<opset1::FakeQuantize> quantize,
			std::vector<float>& inputLowValues,
			std::vector<float>& inputHighValues
			);
	
		static void :target:`getOutputIntervals<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a9d035abad6ff32b782f4e285ef12caa0>`(
			std::shared_ptr<opset1::FakeQuantize> quantize,
			std::vector<float>& outputLowValues,
			std::vector<float>& outputHighValues
			);
	
		static QuantizationDetails :target:`getDetails<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1a95c195808850421e7dfca2ae47a2800e>`(std::shared_ptr<opset1::FakeQuantize>);
		static bool :target:`isSupportedLevel<doxid-classngraph_1_1pass_1_1low__precision_1_1_quantization_details_1aec0fa82673eacbd1ccde6d8f1c383d9c>`(const size_t level);
	};

