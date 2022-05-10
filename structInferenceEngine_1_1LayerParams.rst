.. index:: pair: struct; InferenceEngine::LayerParams
.. _doxid-struct_inference_engine_1_1_layer_params:

struct InferenceEngine::LayerParams
===================================



Overview
~~~~~~~~

Deprecated Migrate to IR v10 and work with :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` directly. :ref:`More...<details-struct_inference_engine_1_1_layer_params>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	struct LayerParams
	{
		// fields
	
		std::string :ref:`name<doxid-struct_inference_engine_1_1_layer_params_1af1df6d7abe75229d793eca546f075c66>`;
		std::string :ref:`type<doxid-struct_inference_engine_1_1_layer_params_1a9540b56f6830cdf1a269c112284fb098>`;
		:ref:`Precision<doxid-class_inference_engine_1_1_precision>` :ref:`precision<doxid-struct_inference_engine_1_1_layer_params_1aad7058b36874adbc0cc2a1ca1c0965c6>`;

		// construction
	
		:ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params_1af8ca6b9f92a164a871b6025dd1ed1442>`();
		:ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params_1a9f9ca5259c927dd71110351f587609e9>`(const LayerParams& other);
	
		:ref:`LayerParams<doxid-struct_inference_engine_1_1_layer_params_1a42d2eb7da311042c8d60b7b282bf57b6>`(
			const std::string& name,
			const std::string& type,
			:ref:`Precision<doxid-class_inference_engine_1_1_precision>` precision
			);

		// methods
	
		LayerParams& :ref:`operator =<doxid-struct_inference_engine_1_1_layer_params_1a57e3756da9c77445c523a19049fa261b>` (const LayerParams& other);
	};
.. _details-struct_inference_engine_1_1_layer_params:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Deprecated Migrate to IR v10 and work with :ref:`ngraph::Function <doxid-classngraph_1a14d7fe7c605267b52c145579e12d2a5f>` directly. The method will be removed in 2021.1

Fields
------

.. _doxid-struct_inference_engine_1_1_layer_params_1af1df6d7abe75229d793eca546f075c66:
.. index:: pair: variable; name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string name

Layer name.

.. _doxid-struct_inference_engine_1_1_layer_params_1a9540b56f6830cdf1a269c112284fb098:
.. index:: pair: variable; type

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string type

Layer type.

.. _doxid-struct_inference_engine_1_1_layer_params_1aad7058b36874adbc0cc2a1ca1c0965c6:
.. index:: pair: variable; precision

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Precision<doxid-class_inference_engine_1_1_precision>` precision

Layer precision.

Construction
------------

.. _doxid-struct_inference_engine_1_1_layer_params_1af8ca6b9f92a164a871b6025dd1ed1442:
.. index:: pair: function; LayerParams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LayerParams()

A default constructor.

.. _doxid-struct_inference_engine_1_1_layer_params_1a9f9ca5259c927dd71110351f587609e9:
.. index:: pair: function; LayerParams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LayerParams(const LayerParams& other)

A copy constructor.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- An object to copy.

.. _doxid-struct_inference_engine_1_1_layer_params_1a42d2eb7da311042c8d60b7b282bf57b6:
.. index:: pair: function; LayerParams

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LayerParams(
		const std::string& name,
		const std::string& type,
		:ref:`Precision<doxid-class_inference_engine_1_1_precision>` precision
		)

A constructor with parameters.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- A layer name.

	*
		- type

		- A layer type.

	*
		- precision

		- A layer precision.

Methods
-------

.. _doxid-struct_inference_engine_1_1_layer_params_1a57e3756da9c77445c523a19049fa261b:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LayerParams& operator = (const LayerParams& other)

A copy assignment operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- other

		- An object to copy



.. rubric:: Returns:

A value


