.. index:: pair: enum; ExecutionMode
.. _doxid-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499:

enum ov::intel_gna::ExecutionMode
=================================

Overview
~~~~~~~~

Enum to define software acceleration mode. :ref:`More...<details-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499>`

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <properties.hpp>

	enum ExecutionMode
	{
	    :ref:`AUTO<doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499ae1f2d5134ed2543d38a0de9751cf75d9>`             = 0,
	    :ref:`HW<doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499a4bd2241a3a809d3cc2bb28e951cc183a>`               = 1,
	    :ref:`HW_WITH_SW_FBACK<doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499a5628dcdf14e39ece06c6ed5297b2a823>` =         2,
	    :ref:`SW_EXACT<doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499acae42957c2ecdda981ee942aada307ec>`         = 3,
	    :ref:`SW_FP32<doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499a8ea28d5d5fdd438f63c14d2f4167ddb2>`          = 4,
	};

.. _details-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Enum to define software acceleration mode.

Enum Values
-----------

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499ae1f2d5134ed2543d38a0de9751cf75d9:
.. index:: pair: enumvalue; AUTO

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	AUTO

Uses Intel GNA if available, otherwise uses software execution mode on CPU.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499a4bd2241a3a809d3cc2bb28e951cc183a:
.. index:: pair: enumvalue; HW

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HW

Uses Intel GNA if available, otherwise raises an error.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499a5628dcdf14e39ece06c6ed5297b2a823:
.. index:: pair: enumvalue; HW_WITH_SW_FBACK

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HW_WITH_SW_FBACK

Uses Intel GNA if available, otherwise raises an error. If the hardware queue is not empty, automatically falls back to CPU in the bit-exact mode.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499acae42957c2ecdda981ee942aada307ec:
.. index:: pair: enumvalue; SW_EXACT

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SW_EXACT

Executes the GNA-compiled graph on CPU performing calculations in the same precision as the Intel GNA in the bit-exact mode.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ggab1ef047d51bcaf91e5d2bbb1fd535499a8ea28d5d5fdd438f63c14d2f4167ddb2:
.. index:: pair: enumvalue; SW_FP32

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SW_FP32

Executes the GNA-compiled graph on CPU but substitutes parameters and calculations from low precision to floating point

