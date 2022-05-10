.. index:: pair: class; ngraph::pass::low_precision::FakeQuantizeDequantization
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization:

class ngraph::pass::low_precision::FakeQuantizeDequantization
=============================================================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <fake_quantize_dequantization.hpp>
	
	class FakeQuantizeDequantization
	{
	public:
		// fields
	
		:ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`> :target:`data<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a50bbd9173f66e85d51d13829f0dc6bea>`;
		std::shared_ptr<opset1::Convert> :target:`convert<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1aea4ffb1d75a84b64ee9ff587956735fc>`;
		std::shared_ptr<opset1::Subtract> :target:`subtract<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a20dd9125cfd076039f3b6143472f92d9>`;
		std::shared_ptr<ngraph::opset1::Convert> :target:`subtractConvert<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a9784a16ce9d165a8f25b7295c30c3896>`;
		std::shared_ptr<ngraph::opset1::Constant> :target:`subtractConstant<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1afe259a426faf075888b113ae36bd2ab7>`;
		std::shared_ptr<opset1::Multiply> :target:`multiply<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1aa359190b6e00cc62affff4bb68058dec>`;
		std::shared_ptr<ngraph::opset1::Constant> :target:`multiplyConstant<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1ad63610137e9cc544149c4988013b34da>`;

		// construction
	
		:target:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a6dfdad1be6c6962e216c6ea0c12b744e>`();
	
		:target:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1af40b0b2090691dfe48380238f55a6dd8>`(
			const :ref:`Output<doxid-classov_1_1_output>`<:ref:`Node<doxid-classov_1_1_node>`>& data,
			const std::shared_ptr<ngraph::opset1::Convert>& convert,
			const std::shared_ptr<ngraph::opset1::Subtract>& subtract,
			const std::shared_ptr<ngraph::opset1::Convert>& subtractConvert,
			const std::shared_ptr<ngraph::opset1::Constant>& subtractConstant,
			const std::shared_ptr<ngraph::opset1::Multiply>& multiply,
			const std::shared_ptr<ngraph::opset1::Constant>& multiplyConstant
			);

		// methods
	
		bool :target:`empty<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a5595de4301a13c63915d80af34b8d96e>`() const;
		bool :target:`multiplyHasZeroOrDenormal<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a1f499285c5ad5c3c3d7794ce9f9d7c04>`() const;
		bool :target:`isShared<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a141a775a22f07a06b2ba61df6c40c515>`() const;
		bool :target:`isLowPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a483a3dae3a92bb78cae458b595e0767e>`() const;
		std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`copyWithNewInput<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a35833ebbe457335dd510d895c3cf79fa>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& input) const;
		static bool :target:`checkElementwise<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a5ac083975840ab210d1e9e86315f49ce>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& elementwise);
		static bool :target:`checkShape<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1a4a3b8f8a546b2cd6f8550bd8e199de87>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& elementwise);
	
		static int :target:`fillDequantizationParams<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1aaa520c00a44be1de27c44400439c52da>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& elementwise,
			std::shared_ptr<ngraph::opset1::Convert>& convert,
			std::shared_ptr<ngraph::opset1::Constant>& constant
			);
	
		static int :target:`fillDequantizationParams<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization_1adfe88fd2772c25c9de6880a7ffc97bba>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& elementwise,
			std::shared_ptr<ngraph::opset1::Constant>& constant
			);
	};

