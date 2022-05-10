.. index:: pair: class; ngraph::pass::low_precision::NetworkHelper
.. _doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper:

class ngraph::pass::low_precision::NetworkHelper
================================================

.. toctree::
	:hidden:

	InsertDequantizationResult <classngraph_1_1pass_1_1low_precision_1_1NetworkHelper_1_1InsertDequantizationResult.rst>

:ref:`NetworkHelper <doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper>` class encapsulates manipulations with nGraph function.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <network_helper.hpp>
	
	class NetworkHelper
	{
	public:
		// classes
	
		class :ref:`InsertDequantizationResult<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result>`;

		// methods
	
		static bool :target:`is_castable_to_one_of<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ae0d09dc2b06b5c5ba9ffafcca5e08d58>`(
			:ref:`NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>` type,
			const std::unordered_set<:ref:`NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>`>& types
			);
	
		static std::vector<:ref:`Input<doxid-classov_1_1_input>`<:ref:`Node<doxid-classov_1_1_node>`>> :target:`consumer_inputs<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a702a9fbb2e71adb8bda6d197b753cbdf>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		static std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :target:`consumers<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1aafd698a07b3e8215fc131feaab18a841>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		static bool :target:`isConstantPath<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ab4eb6fec9693e994463999aa2b88145d>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& op);
	
		template <typename OperationType>
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`setOutDataPrecisionForTypeRelaxed<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a6888f0d53b36133f124de4ca3f77407d>`(
			std::shared_ptr<OperationType> operation,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& precision
			);
	
		template <typename OperationType>
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`setOutDataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1afeec64a9ffe8830a279e6c2061e99fc1>`(
			std::shared_ptr<OperationType> operation,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`& precision
			);
	
		static std::shared_ptr<opset1::Constant> :target:`foldDequantizationConstant<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a19314448e0b0a7b4055d13503a599e48>`(
			const std::shared_ptr<opset1::Constant>& foldingConstant,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& operation,
			const size_t outIdx = 0
			);
	
		static size_t :target:`getOutputChannelsCount<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a42fa67599033efff28622606bdb62fd0>`(
			std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`> layer,
			bool isOnWeights = false
			);
	
		static std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :target:`getParentsRecursivelyExceptTypes<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ab8acbcdb069987d19f57db85245612e8>`(
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer,
			const std::unordered_set<:ref:`NodeTypeInfo<doxid-classngraph_1a8f207b9a789594d326c5adbfc49ccc71>`>& exceptionLayerTypes = {},
			const int portIndex = -1
			);
	
		static size_t :target:`getInputChannelsCount<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1add5c0dd91d6bd39700f84b4a3f5e3c1b>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer);
		static size_t :target:`getGroupsCount<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a6734e393dcb30f5c695258ea49d4074c>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> layer);
		static void :target:`removeLayer<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1aa130979bb3167a0f0a23d242749dc5f5>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
	
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`swapMultiplyAndAdd<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a69aa52c4bd913bd00af4b3908436cfa5>`(
			std::shared_ptr<opset1::Add> addAfterMultiply,
			const int multiplyBranch
			);
	
		static void :target:`copyInfo<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a42f5c0b18d4c5c446143fb2d41013aaf>`(
			const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& sources,
			const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& targets,
			bool overrideName = true
			);
	
		static void :target:`copyInfo<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a7e4046bbb3d2426e4524328abb97769e>`(
			const std::vector<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>>& sources,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& target,
			bool overrideName = true
			);
	
		static void :target:`copyInfo<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a2b9b83f5ecd522572de2d3f61fe824b3>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& source,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& target,
			bool overrideName = true
			);
	
		static bool :target:`isScalarLike<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a3bf04c7045a9e9835a626a8939518d00>`(std::shared_ptr<opset1::Constant> constant);
		static bool :target:`isZero<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a557526a09597b0764f7de4818584ec81>`(std::shared_ptr<opset1::Constant> constant);
		static std::shared_ptr<opset1::Constant> :target:`toScalar<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a82b41d1e1485ab258d8e808994aa46e1>`(std::shared_ptr<opset1::Constant> constant);
	
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`getConstantInput<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a6e24c70a2411187146ae7cdfda854d6a>`(
			const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node,
			const bool convertIsExpected = false
			);
	
		static std::vector<size_t> :target:`updateReshapeValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a5c3d91e0c549225d221853e41bfb0c25>`(
			const :ref:`Shape<doxid-classov_1_1_shape>`& elementwiseConstantShape,
			const :ref:`Shape<doxid-classov_1_1_shape>`& elementwiseShape,
			const std::vector<size_t>& reshapeValues
			);
	
		static std::shared_ptr<ngraph::opset1::Multiply> :target:`optimizeMultipliesAfter<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a30966c10747d0f9194349b5ca5d090ba>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> multiply);
	
		static std::shared_ptr<opset1::Constant> :target:`round<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a5b8194daa318207e8c598789aaa26e6c>`(
			std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node,
			:ref:`element::Type<doxid-classov_1_1element_1_1_type>` target_type
			);
	
		static std::shared_ptr<opset1::FakeQuantize> :target:`composeFakeQuantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a4e5881bb76d1878324f157717f46cf01>`(
			const std::shared_ptr<opset1::FakeQuantize>& fq,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static std::tuple<std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>, std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>> :target:`decomposeFakeQuantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a378608fce035e81d2d30ba10253c1ede>`(
			std::shared_ptr<opset1::FakeQuantize> fq,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision,
			const float min,
			const float max,
			const bool hasZeroPoint,
			const bool updatePrecision,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` deqPrecision = element::f32,
			const size_t outChannelsShapeIndex = 0
			);
	
		static std::shared_ptr<opset1::FakeQuantize> :target:`updateFakeQuantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a4a65ba330ee05ba20edcdd2a5dd8af69>`(
			std::shared_ptr<opset1::FakeQuantize> fq,
			:ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision,
			float min,
			float max,
			const bool replace = true
			);
	
		static :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` :target:`makeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a8473e5c757ffc0df4e99832a7feef2c6>`(
			const float dequantizationMul,
			const float dequantizationSub,
			const :ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>` originalPrecision,
			const :ref:`ngraph::PartialShape<doxid-classov_1_1_partial_shape>`& dataNodeOutputShape,
			:ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` deqPrecision = element::f32,
			std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> input = nullptr
			);
	
		static :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` :target:`createDequantizationFromFakeQuantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a00ebce26b04f14cc5f6320d61d54274e>`(
			std::shared_ptr<opset1::FakeQuantize> fq,
			:ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision,
			float min,
			float max,
			const bool hasZeroPoint,
			const bool updatePrecision,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` deqPrecision = element::f32
			);
	
		static bool :target:`areQuantizeAndDequantizeSupportedForSubtract<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1acaa693323231737064c9d7d6e3a25b89>`(
			const std::shared_ptr<const :ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static bool :target:`areQuantizeAndDequantizeSupportedForMultiply<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ae0dfcb088b4a5659a946b56e171ae2d7>`(
			const std::shared_ptr<const :ref:`ngraph::Node<doxid-classov_1_1_node>`>& node,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& _defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static bool :target:`isQuantizeSupported<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ae7135afe102a13e55e8f5c127c3788b0>`(const std::shared_ptr<opset1::FakeQuantize>& fakeQuantize);
	
		static :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` :target:`getDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1afa7f688b000e2533731deef01f767157>`(
			const std::shared_ptr<const :ref:`Node<doxid-classov_1_1_node>`>& node,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`> _defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`,
			const size_t parentIndex = 0ul,
			const bool inPlace = false
			);
	
		static :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` :target:`getDequantizationBelow<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a66377e160ee554d01eb7b6ce72b96415>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
			const bool convertIsMandatory = false
			);
	
		static :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` :target:`normalizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a6f04fcabb60a06f0f2fb6f755b0470c0>`(:ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` dequantization);
	
		static std::shared_ptr<opset1::Constant> :target:`normalizeDequantizationShape<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a3d4a8de6da3facd0bace4a69a6949945>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& eltwise,
			const bool convertIsExpected = false
			);
	
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`optimizeSubtract<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a32af186e5d008bef4334319c9113afb8>`(std::shared_ptr<opset1::Subtract> add);
	
		static :ref:`InsertDequantizationResult<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result>` :target:`moveDequantizationAfter<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a611c837a001d9f963a8ea605a03c2ce7>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& operation,
			const :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>`& dequantization,
			const bool updatePrecision,
			const bool moveSubtract,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static :ref:`InsertDequantizationResult<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1_1_insert_dequantization_result>` :target:`moveDequantizationBefore<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a4b6ba4e093d229bb53acf421af0d7b15>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& operation,
			const :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>`& dequantization,
			const bool updatePrecision,
			const bool moveSubtract
			);
	
		static std::vector<std::vector<std::shared_ptr<ngraph::opset1::Constant>>> :target:`splitConstantsBeforeConcat<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1aafdb5b43f57e156d0531723c4bf3fa62>`(
			const std::shared_ptr<:ref:`ov::Node<doxid-classov_1_1_node>`> concat,
			const std::vector<std::shared_ptr<opset1::Constant>> currConstants
			);
	
		static bool :target:`checkConstantValuePrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a9a12da84c58f36e33216572df189fecc>`(
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` expectedPrecision,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& constant
			);
	
		static size_t :target:`getChildInputIndex<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1af60dfe2c1d2d8a94c5e5c2d969c63b7e>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& parent,
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& child
			);
	
		static size_t :target:`getParentOutputIndex<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a7f4a178c1caaa5b2eadc8725ee4db7cd>`(
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& parent,
			const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& child
			);
	
		static :ref:`FakeQuantizeDequantizationValues<doxid-namespacengraph_1_1pass_1_1low__precision_1aca276710287c1a293770619348ca5054>` :target:`createEmptyValues<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a5b2ae483dbceba9d9f86c71b6f1f6df5>`(
			const :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>`& dequantization,
			const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` precision
			);
	
		static bool :target:`isZeroConst<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a48e239d5d5d3e02e1fdabe88c37f2460>`(const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node);
	
		static bool :target:`checkZeroPoint<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a6a6671be46bca5150f3db94b73644541>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
			const :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`& dataPrecision = :ref:`DataPrecision<doxid-classngraph_1_1pass_1_1low__precision_1_1_data_precision>`()
			);
	
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`toScalarIfPossible<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ab075ed99a3cd1bcdbd777603033a496f>`(std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> node);
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`fold_fake_quantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1aaf72291d4eada5e73ac9dd13f854d8c5>`(const std::shared_ptr<opset1::FakeQuantize>& fq);
	
		static std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`> :target:`fold_fake_quantize<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a6708a40ccfd6d00c9d891425b47345e6>`(
			const std::shared_ptr<opset1::FakeQuantize>& fq,
			const bool roundValues,
			int outChannelsShapeIndex = 0
			);
	
		static :ref:`FakeQuantizeDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_fake_quantize_dequantization>` :target:`foldDequantization<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a168fda17ca945abb939fa76adb9cb2cc>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& node,
			const size_t branchIndex,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`,
			const bool inPlace = false
			);
	
		static std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> :target:`separateInStandaloneBranch<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ae8e8e68eb56b1435b9f8eaee45c558c5>`(
			std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`> node,
			const std::vector<:ref:`ngraph::element::Type<doxid-classov_1_1element_1_1_type>`>& defaultPrecisions = :ref:`precision_set::int8_support<doxid-namespacengraph_1_1pass_1_1low__precision_1_1precision__set_1aadf8375a12f123670991b043f50a94e5>`
			);
	
		static std::shared_ptr<opset1::FakeQuantize> :target:`fuseConvert<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a66f59edc5d96ac5d53def5ce4adb8f3c>`(const std::shared_ptr<opset1::FakeQuantize>& fakeQuantize);
	
		static std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`> :target:`precisionIntersection<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a33fecde05d2ac427ded5b5c61766e438>`(
			const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& v1,
			const std::vector<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`>& v2
			);
	
		static bool :target:`isPrecisionPreserved<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1aceac67b80b726054fd8917239b7c36f9>`(const std::shared_ptr<:ref:`ngraph::Node<doxid-classov_1_1_node>`>& node);
	
		static void :target:`insertDequantizationAfter<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1ab73371dbe56b6d94c7a1a050e21c38d9>`(
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& originalNode,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& dequantization,
			const std::shared_ptr<:ref:`Node<doxid-classov_1_1_node>`>& newNode
			);
	
		template <typename SharedAttribute>
		static void :target:`reassign<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a0248ff11c9903f99e6c2f141277ae9d9>`(
			const std::shared_ptr<typename :ref:`SharedAttribute::SharedValueAttribute::SharedValue<doxid-struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value>`>& sharedValue,
			const std::vector<std::weak_ptr<typename :ref:`SharedAttribute::SharedValueAttribute<doxid-class_shared_attribute_1_1_shared_value_attribute>`>>& attributes
			);
	
		static size_t :target:`calculateLevels<doxid-classngraph_1_1pass_1_1low__precision_1_1_network_helper_1a22d411bc509617d56881df76588b6a0f>`(
			const float dataPrecisionMin,
			const float dataPrecisionMax,
			const float combinedIntervalLow,
			const float combinedIntervalHigh,
			const float minIntervalLow,
			const float minIntervalHigh,
			float& dequantizationMul,
			float& dequantizationSub,
			float& updatedOutputLowValue,
			float& updatedOutputHighValue
			);
	};

