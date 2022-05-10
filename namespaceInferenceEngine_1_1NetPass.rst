.. index:: pair: namespace; InferenceEngine::NetPass
.. _doxid-namespace_inference_engine_1_1_net_pass:

namespace InferenceEngine::NetPass
==================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace NetPass {

	// global functions

	bool :ref:`CombineRNNSeq<doxid-namespace_inference_engine_1_1_net_pass_1a9d8d73f4802e65a88a071ab9ab6fb30c>`(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net);
	bool :target:`CombineRNNSeq<doxid-namespace_inference_engine_1_1_net_pass_1afdaf01de908c14f8fd0fceb58c19752b>`(:ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>`& net);
	std::vector<:ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`> :ref:`TIBodySortTopologically<doxid-namespace_inference_engine_1_1_net_pass_1a9235c33d2e2d4e2755b49c033b08d9bd>`(const :ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>`& body);
	bool :ref:`HasInternalSubnet<doxid-namespace_inference_engine_1_1_net_pass_1a278478ca4398734eef41eb9a478dfc62>`(const :ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`& layer);
	details::CNNSubnet :ref:`GetInternalSubnet<doxid-namespace_inference_engine_1_1_net_pass_1a9213452a8807b27e8650f8a537e7d84b>`(const :ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`& layer);
	bool :ref:`UnrollTI<doxid-namespace_inference_engine_1_1_net_pass_1adcb808bbd2ff9707d03eceef2d01b0ac>`(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net);
	bool :ref:`UnrollRNN_if<doxid-namespace_inference_engine_1_1_net_pass_1a2ac256a93533c09c0ccbe1bb4a270ab5>`(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net, std::function<bool(const :ref:`RNNCellBase<doxid-class_inference_engine_1_1_r_n_n_cell_base>`&)> pred);

	:ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>` :ref:`CopyTIBody<doxid-namespace_inference_engine_1_1_net_pass_1a8dd5172f0f06e5f862dc4891c5a6f615>`(
		const :ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>`& body,
		std::string suffix = std::string()
		);

	bool :target:`UnrollRNN_if<doxid-namespace_inference_engine_1_1_net_pass_1aab9b92b45e87515474a1f1ad53d3a46c>`(
		:ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>`& net,
		std::function<bool(const :ref:`RNNCellBase<doxid-class_inference_engine_1_1_r_n_n_cell_base>`&)> pred
		);

	void :ref:`ConvertPrecision<doxid-namespace_inference_engine_1_1_net_pass_1acc5608a61279c68b0cdbd5e0ce4bca3f>`(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` from, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` to);
	void :target:`ConvertIOPrecision<doxid-namespace_inference_engine_1_1_net_pass_1a8a11c0a658a9881741e469abf86fc12a>`(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` from, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` to);

	} // namespace NetPass
.. _details-namespace_inference_engine_1_1_net_pass:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. _doxid-namespace_inference_engine_1_1_net_pass_1a9d8d73f4802e65a88a071ab9ab6fb30c:
.. index:: pair: function; CombineRNNSeq

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool CombineRNNSeq(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net)

Try to detect LSTM Sequence pattern inside TI and convert it



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- net

		- network to modify



.. rubric:: Returns:

true if all Tensor iterator was converted

.. _doxid-namespace_inference_engine_1_1_net_pass_1a9235c33d2e2d4e2755b49c033b08d9bd:
.. index:: pair: function; TIBodySortTopologically

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`> TIBodySortTopologically(const :ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>`& body)

Returns a vector of the topologically sorted layers from the passed TI layer body.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- body

		- TI body



.. rubric:: Returns:

vector of layer objects

.. _doxid-namespace_inference_engine_1_1_net_pass_1a278478ca4398734eef41eb9a478dfc62:
.. index:: pair: function; HasInternalSubnet

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool HasInternalSubnet(const :ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`& layer)

Check if provided layer contains internal attribute like subnet/subgraph



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layer

		- to check



.. rubric:: Returns:

true if layer has subnet

.. _doxid-namespace_inference_engine_1_1_net_pass_1a9213452a8807b27e8650f8a537e7d84b:
.. index:: pair: function; GetInternalSubnet

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	details::CNNSubnet GetInternalSubnet(const :ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`& layer)

Extract internal subnet from layer

All internal layers are returned by reference. Any modification further subnet modification will has affect on original layer state.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- layer

		- to proceed



.. rubric:: Returns:

internal subnet

.. _doxid-namespace_inference_engine_1_1_net_pass_1adcb808bbd2ff9707d03eceef2d01b0ac:
.. index:: pair: function; UnrollTI

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool UnrollTI(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net)

Unroll all present Tensor Iterators



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- net

		- network to modify



.. rubric:: Returns:

true if all Tensor iterator was unrolled successfully

.. _doxid-namespace_inference_engine_1_1_net_pass_1a2ac256a93533c09c0ccbe1bb4a270ab5:
.. index:: pair: function; UnrollRNN_if

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool UnrollRNN_if(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net, std::function<bool(const :ref:`RNNCellBase<doxid-class_inference_engine_1_1_r_n_n_cell_base>`&)> pred)

Unroll all RNN specific layers by predicate

Will be applied to all RNNSeq and :ref:`RNNCell <doxid-class_inference_engine_1_1_r_n_n_cell>` layers



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- net

		- network to modify

	*
		- pred

		- predicate to mark layer to unroll



.. rubric:: Returns:

true if all RNN layers was unrolled successfully

.. _doxid-namespace_inference_engine_1_1_net_pass_1a8dd5172f0f06e5f862dc4891c5a6f615:
.. index:: pair: function; CopyTIBody

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>` CopyTIBody(
		const :ref:`TensorIterator::Body<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_body>`& body,
		std::string suffix = std::string()
		)

Construct a copy of provided subnet. Will change names by adding suffix if it was provided.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- subnet

		- to copy from

	*
		- suffix

		- is optional attribute. Will be added into name of each layer/data object if provided



.. rubric:: Returns:

subnet copy. Each layer/data object is newly created. Const blob objects is inherited from original subnet.

.. _doxid-namespace_inference_engine_1_1_net_pass_1acc5608a61279c68b0cdbd5e0ce4bca3f:
.. index:: pair: function; ConvertPrecision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void ConvertPrecision(:ref:`CNNNetwork<doxid-class_inference_engine_1_1_c_n_n_network>`& net, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` from, :ref:`Precision<doxid-class_inference_engine_1_1_precision>` to)

:ref:`Precision <doxid-class_inference_engine_1_1_precision>` conversion pass

Will perform conversion of all presented tensors with specified precision including const blobs and intermediate tensors. It doesn't check layer semantic. It may break correctness of topology.

It also remove redundant convert layers if they will appear.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- net

		- is network to apply conversion

	*
		- from

		- precision of tensors required conversion

	*
		- to

		- resulting precision of tensors

