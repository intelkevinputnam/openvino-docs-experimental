.. index:: pair: enum; CellType
.. _doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3:

enum InferenceEngine::RNNCellBase::CellType
===========================================

Overview
~~~~~~~~

Direct type of recurrent cell (including subtypes) Description of particular cell semantics is in :ref:`LSTMCell <doxid-class_inference_engine_1_1_l_s_t_m_cell>`, :ref:`GRUCell <doxid-class_inference_engine_1_1_g_r_u_cell>`, :ref:`RNNCell <doxid-class_inference_engine_1_1_r_n_n_cell>`. :ref:`More...<details-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>

	enum CellType
	{
	    :ref:`LSTM<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a910000de786e7fcdc257fbd01a0559a8>`,
	    :ref:`GRU<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a1e137b059dc56f4e464fd78e6b5588b1>`,
	    :ref:`RNN<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a2085e85695ce4f41c62f5a198f4f397e>`,
	    :ref:`GRU_LBR<doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3acfc6783005836eaaaa5e6a9d7d282785>`,
	};

.. _details-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Direct type of recurrent cell (including subtypes) Description of particular cell semantics is in :ref:`LSTMCell <doxid-class_inference_engine_1_1_l_s_t_m_cell>`, :ref:`GRUCell <doxid-class_inference_engine_1_1_g_r_u_cell>`, :ref:`RNNCell <doxid-class_inference_engine_1_1_r_n_n_cell>`.

Enum Values
-----------

.. _doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a910000de786e7fcdc257fbd01a0559a8:
.. index:: pair: enumvalue; LSTM

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LSTM

Original LSTM cell

.. _doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a1e137b059dc56f4e464fd78e6b5588b1:
.. index:: pair: enumvalue; GRU

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GRU

Original GRU cell

.. _doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3a2085e85695ce4f41c62f5a198f4f397e:
.. index:: pair: enumvalue; RNN

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RNN

Original RNN cell

.. _doxid-class_inference_engine_1_1_r_n_n_cell_base_1aa0c9020aaea4ab61d36b9ef112207ca3acfc6783005836eaaaa5e6a9d7d282785:
.. index:: pair: enumvalue; GRU_LBR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GRU_LBR

GRU cell modification. "Linear before reset"

