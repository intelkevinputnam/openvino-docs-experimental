.. index:: pair: struct; InferenceEngine::TensorIterator::PortMap
.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map:

struct InferenceEngine::TensorIterator::PortMap
===============================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>
	
	struct PortMap
	{
		// fields
	
		int :ref:`from<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a55dcb90f4fd951b4d8ee57d32b85042f>`;
		int :ref:`to<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a6c4c0cb8316811c0c34d2b065a6f7666>`;
		int :ref:`axis<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1ab6d4dc7895f72a97dedb8709b77e8f28>`;
		int :ref:`stride<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a7e9fd0dd49c6af7712a1fc56062b753b>`;
		int :ref:`start<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a4b2c93d61957af4a7f690dbf4469fc4e>`;
		int :ref:`end<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a103144439f1023eee4dcd90217cbbf85>`;
		int :ref:`part_size<doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1ab769848d4e018f8899d2f4326b15e268>`;
	};
.. _details-struct_inference_engine_1_1_tensor_iterator_1_1_port_map:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Fields
------

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a55dcb90f4fd951b4d8ee57d32b85042f:
.. index:: pair: variable; from

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int from

Index of exteral data from ins/outs fields of :ref:`CNNLayer <doxid-class_inference_engine_1_1_c_n_n_layer>`

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a6c4c0cb8316811c0c34d2b065a6f7666:
.. index:: pair: variable; to

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int to

Index of internal data in iterator body

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1ab6d4dc7895f72a97dedb8709b77e8f28:
.. index:: pair: variable; axis

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int axis

Axis to iterate throught

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a7e9fd0dd49c6af7712a1fc56062b753b:
.. index:: pair: variable; stride

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int stride

Stride to iterate throught

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a4b2c93d61957af4a7f690dbf4469fc4e:
.. index:: pair: variable; start

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int start

Start index of iteration range

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1a103144439f1023eee4dcd90217cbbf85:
.. index:: pair: variable; end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int end

Last index of iteration range

.. _doxid-struct_inference_engine_1_1_tensor_iterator_1_1_port_map_1ab769848d4e018f8899d2f4326b15e268:
.. index:: pair: variable; part_size

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int part_size

Part size which will be transfered to body subnetwork


