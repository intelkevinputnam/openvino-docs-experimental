.. index:: pair: namespace; ov::intel_gna
.. _doxid-namespaceov_1_1intel__gna:

namespace ov::intel_gna
=======================

.. toctree::
	:hidden:

Namespace with Intel GNA specific properties.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace intel_gna {

	// enums

	enum :ref:`ExecutionMode<doxid-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499>`;
	enum :ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`;
	enum :ref:`PWLDesignAlgorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1gadff8cc42104b8f3a8a4c50c08a45f6a3>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`library_full_version<doxid-group__ov__runtime__gna__prop__cpp__api_1gae3d6b5080a37a65548ed411d3f6b00ca>` {"GNA_LIBRARY_FULL_VERSION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<std::string, float>> :ref:`scale_factors_per_input<doxid-group__ov__runtime__gna__prop__cpp__api_1gaf72daf77f0c085f54b0a84f77c3d7734>` {"GNA_SCALE_FACTOR_PER_INPUT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> :ref:`firmware_model_image_path<doxid-group__ov__runtime__gna__prop__cpp__api_1gafe83f57de302a35fa0d94563fab01e2d>` {"GNA_FIRMWARE_MODEL_IMAGE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ExecutionMode<doxid-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499>`> :ref:`execution_mode<doxid-group__ov__runtime__gna__prop__cpp__api_1ga68ea397901af8f965863fbe599535341>` {"GNA_DEVICE_MODE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`> :ref:`execution_target<doxid-group__ov__runtime__gna__prop__cpp__api_1ga4ecfa3938d07be52618f606bb54ac429>` {"GNA_HW_EXECUTION_TARGET"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`> :ref:`compile_target<doxid-group__ov__runtime__gna__prop__cpp__api_1gad9a766500212ccb6826b47aedde9e825>` {"GNA_HW_COMPILE_TARGET"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> :ref:`memory_reuse<doxid-group__ov__runtime__gna__prop__cpp__api_1ga23eede6f1972f66534651d7946963953>` {"GNA_COMPACT_MODE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`PWLDesignAlgorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1gadff8cc42104b8f3a8a4c50c08a45f6a3>`> :ref:`pwl_design_algorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1ga4b02b547bf360236e72ab5aa9c8d1d44>` {"GNA_PWL_DESIGN_ALGORITHM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<float> :ref:`pwl_max_error_percent<doxid-group__ov__runtime__gna__prop__cpp__api_1gaaf0afe1c01700ad7eed94783910c27fa>` {"GNA_PWL_MAX_ERROR_PERCENT"};

	} // namespace intel_gna
