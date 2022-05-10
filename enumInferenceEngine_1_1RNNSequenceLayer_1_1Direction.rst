.. index:: pair: enum; Direction
.. _doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12ab:

enum InferenceEngine::RNNSequenceLayer::Direction
=================================================

Overview
~~~~~~~~

Direction of iteration through sequence dimension. :ref:`More...<details-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12ab>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ie_layers.h>

	enum Direction
	{
	    :ref:`FWD<doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12abac742554fe3954954cb7900cdce2b0f76>`,
	    :ref:`BWD<doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12abafe1c34556b3dd0a5d278808e681bc8d8>`,
	    :ref:`BDR<doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12aba7030a3fe9a397c08caf5dd6d7388f198>`,
	};

.. _details-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12ab:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Direction of iteration through sequence dimension.

Enum Values
-----------

.. _doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12abac742554fe3954954cb7900cdce2b0f76:
.. index:: pair: enumvalue; FWD

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FWD

Forward mode. Iterate starts from index 0 with step 1.

.. _doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12abafe1c34556b3dd0a5d278808e681bc8d8:
.. index:: pair: enumvalue; BWD

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BWD

Backward mode. Iterate starts from last index with step -1.

.. _doxid-class_inference_engine_1_1_r_n_n_sequence_layer_1a6e831e42636d72cb8b8d1c03dfae12aba7030a3fe9a397c08caf5dd6d7388f198:
.. index:: pair: enumvalue; BDR

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BDR

Bidirectional mode. First is forward pass, second is backward.

