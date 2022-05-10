.. index:: pair: interface; InferenceEngine::ILayerExecImpl
.. _doxid-class_inference_engine_1_1_i_layer_exec_impl:

interface InferenceEngine::ILayerExecImpl
=========================================



Overview
~~~~~~~~

This class provides interface for the implementation with the custom execution code. :ref:`More...<details-class_inference_engine_1_1_i_layer_exec_impl>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_iextension.h>
	
	template ILayerExecImpl: public :ref:`InferenceEngine::ILayerImpl<doxid-class_inference_engine_1_1_i_layer_impl>`
	{
		// typedefs
	
		typedef std::shared_ptr<ILayerExecImpl> :ref:`Ptr<doxid-class_inference_engine_1_1_i_layer_exec_impl_1a3b25cdf779880a91b9577466952208dd>`;

		// methods
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`getSupportedConfigurations<doxid-class_inference_engine_1_1_i_layer_exec_impl_1a245f69f994c7351d269c45ca2114890b>`(
			std::vector<:ref:`LayerConfig<doxid-struct_inference_engine_1_1_layer_config>`>& conf,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`init<doxid-class_inference_engine_1_1_i_layer_exec_impl_1af22bf65cae9c3082d212e4d120dbfb0b>`(:ref:`LayerConfig<doxid-struct_inference_engine_1_1_layer_config>`& config, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0;
	
		virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` :ref:`execute<doxid-class_inference_engine_1_1_i_layer_exec_impl_1a7d6ae7ed16c37d42532ee40e7082fc29>`(
			std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& inputs,
			std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& outputs,
			:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
			) = 0;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`ILayerImpl<doxid-class_inference_engine_1_1_i_layer_impl>`> :ref:`Ptr<doxid-class_inference_engine_1_1_i_layer_impl_1a83cfc1d50968aa3dbdd05fac0a55c28d>`;

.. _details-class_inference_engine_1_1_i_layer_exec_impl:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class provides interface for the implementation with the custom execution code.

Typedefs
--------

.. _doxid-class_inference_engine_1_1_i_layer_exec_impl_1a3b25cdf779880a91b9577466952208dd:
.. index:: pair: typedef; Ptr

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::shared_ptr<ILayerExecImpl> Ptr

A shared pointer to the :ref:`ILayerExecImpl <doxid-class_inference_engine_1_1_i_layer_exec_impl>` interface.

Methods
-------

.. _doxid-class_inference_engine_1_1_i_layer_exec_impl_1a245f69f994c7351d269c45ca2114890b:
.. index:: pair: function; getSupportedConfigurations

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` getSupportedConfigurations(
		std::vector<:ref:`LayerConfig<doxid-struct_inference_engine_1_1_layer_config>`>& conf,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Gets all supported configurations for the current layer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- conf

		- Vector with supported configurations

	*
		- resp

		- Response descriptor



.. rubric:: Returns:

Status code

.. _doxid-class_inference_engine_1_1_i_layer_exec_impl_1af22bf65cae9c3082d212e4d120dbfb0b:
.. index:: pair: function; init

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` init(:ref:`LayerConfig<doxid-struct_inference_engine_1_1_layer_config>`& config, :ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp) = 0

Initializes the implementation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- config

		- Selected supported configuration

	*
		- resp

		- Response descriptor



.. rubric:: Returns:

Status code

.. _doxid-class_inference_engine_1_1_i_layer_exec_impl_1a7d6ae7ed16c37d42532ee40e7082fc29:
.. index:: pair: function; execute

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`StatusCode<doxid-namespace_inference_engine_1a2ce897aa6a353c071958fe379f5d6421>` execute(
		std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& inputs,
		std::vector<:ref:`Blob::Ptr<doxid-class_inference_engine_1_1_blob_1abb6c4f89181e2dd6d8a29ada2dfb4060>`>& outputs,
		:ref:`ResponseDesc<doxid-struct_inference_engine_1_1_response_desc>` \* resp
		) = 0

Execute method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- inputs

		- Vector of blobs with input memory

	*
		- outputs

		- Vector of blobs with output memory

	*
		- resp

		- Response descriptor



.. rubric:: Returns:

Status code


