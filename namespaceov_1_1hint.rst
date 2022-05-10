.. index:: pair: namespace; ov::hint
.. _doxid-namespaceov_1_1hint:

namespace ov::hint
==================

.. toctree::
	:hidden:

Namespace with hint properties.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace hint {

	// enums

	enum :ref:`PerformanceMode<doxid-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73>`;
	enum :ref:`Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`element::Type<doxid-classov_1_1element_1_1_type>`, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`inference_precision<doxid-group__ov__runtime__cpp__prop__api_1gad605a888f3c9b7598ab55023fbf44240>` {"INFERENCE_PRECISION_HINT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`Priority<doxid-group__ov__runtime__cpp__prop__api_1ga3e74923a1ee02f6f5067a368418f0442>`> :ref:`model_priority<doxid-group__ov__runtime__cpp__prop__api_1ga3663a3976ff7c4bdc3ccdb9ce44945ce>` {"MODEL_PRIORITY"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`PerformanceMode<doxid-group__ov__runtime__cpp__prop__api_1ga032aa530efa40760b79af14913d48d73>`> :ref:`performance_mode<doxid-group__ov__runtime__cpp__prop__api_1ga2691fe27acc8aa1d1700ad40b6da3ba2>` {"PERFORMANCE_HINT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>> :ref:`model<doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` {"MODEL_PTR"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool, :ref:`PropertyMutability::RW<doxid-namespaceov_1aa7f23cdb5187727acc9a4aa3814f6c47af5b15f58cabad73d1bf2de7bcb89db6c>`> :ref:`allow_auto_batching<doxid-group__ov__runtime__cpp__prop__api_1ga445a111e7219955c585eb418d2f4f80d>` {"ALLOW_AUTO_BATCHING"};

	} // namespace hint
