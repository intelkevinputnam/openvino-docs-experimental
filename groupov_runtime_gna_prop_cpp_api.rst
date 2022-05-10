.. index:: pair: group; Intel GNA specific properties
.. _doxid-group__ov__runtime__gna__prop__cpp__api:

Intel GNA specific properties
=============================

.. toctree::
	:hidden:

	ExecutionMode <enumov_1_1intel_gna_1_1ExecutionMode.rst>
	HWGeneration <enumov_1_1intel_gna_1_1HWGeneration.rst>
	PWLDesignAlgorithm <enumov_1_1intel_gna_1_1PWLDesignAlgorithm.rst>

Overview
~~~~~~~~

Set of Intel GNA specific properties. :ref:`More...<details-group__ov__runtime__gna__prop__cpp__api>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// enums

	enum :ref:`ov::intel_gna::ExecutionMode<doxid-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499>`;
	enum :ref:`ov::intel_gna::HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`;
	enum :ref:`ov::intel_gna::PWLDesignAlgorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1gadff8cc42104b8f3a8a4c50c08a45f6a3>`;

	// global variables

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> :ref:`ov::intel_gna::library_full_version<doxid-group__ov__runtime__gna__prop__cpp__api_1gae3d6b5080a37a65548ed411d3f6b00ca>` {"GNA_LIBRARY_FULL_VERSION"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<std::string, float>> :ref:`ov::intel_gna::scale_factors_per_input<doxid-group__ov__runtime__gna__prop__cpp__api_1gaf72daf77f0c085f54b0a84f77c3d7734>` {"GNA_SCALE_FACTOR_PER_INPUT"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> :ref:`ov::intel_gna::firmware_model_image_path<doxid-group__ov__runtime__gna__prop__cpp__api_1gafe83f57de302a35fa0d94563fab01e2d>` {"GNA_FIRMWARE_MODEL_IMAGE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ExecutionMode<doxid-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499>`> :ref:`ov::intel_gna::execution_mode<doxid-group__ov__runtime__gna__prop__cpp__api_1ga68ea397901af8f965863fbe599535341>` {"GNA_DEVICE_MODE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`> :ref:`ov::intel_gna::execution_target<doxid-group__ov__runtime__gna__prop__cpp__api_1ga4ecfa3938d07be52618f606bb54ac429>` {"GNA_HW_EXECUTION_TARGET"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`> :ref:`ov::intel_gna::compile_target<doxid-group__ov__runtime__gna__prop__cpp__api_1gad9a766500212ccb6826b47aedde9e825>` {"GNA_HW_COMPILE_TARGET"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> :ref:`ov::intel_gna::memory_reuse<doxid-group__ov__runtime__gna__prop__cpp__api_1ga23eede6f1972f66534651d7946963953>` {"GNA_COMPACT_MODE"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`PWLDesignAlgorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1gadff8cc42104b8f3a8a4c50c08a45f6a3>`> :ref:`ov::intel_gna::pwl_design_algorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1ga4b02b547bf360236e72ab5aa9c8d1d44>` {"GNA_PWL_DESIGN_ALGORITHM"};
	static constexpr :ref:`Property<doxid-classov_1_1_property>`<float> :ref:`ov::intel_gna::pwl_max_error_percent<doxid-group__ov__runtime__gna__prop__cpp__api_1gaaf0afe1c01700ad7eed94783910c27fa>` {"GNA_PWL_MAX_ERROR_PERCENT"};

.. _details-group__ov__runtime__gna__prop__cpp__api:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Set of Intel GNA specific properties.

Global Variables
----------------

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1gae3d6b5080a37a65548ed411d3f6b00ca:
.. index:: pair: variable; library_full_version

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string, PropertyMutability::RO> ov::intel_gna::library_full_version {"GNA_LIBRARY_FULL_VERSION"}

:ref:`Property <doxid-classov_1_1_property>` to get an std::string of GNA Library version, usually in the form <API_REVISION>.<RELEASE_LINE>.<RELEASE>.<BUILD>

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1gaf72daf77f0c085f54b0a84f77c3d7734:
.. index:: pair: variable; scale_factors_per_input

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::map<std::string, float>> ov::intel_gna::scale_factors_per_input {"GNA_SCALE_FACTOR_PER_INPUT"}

Scale factor provided by the user to use static quantization. This option should be used with floating point value serialized to string with . (dot) as a decimal separator.

In the case of multiple inputs, individual scale factors can be provided using the map where key is layer name and value is scale factor Example:

.. ref-code-block:: cpp

	:ref:`ov::Core <doxid-classov_1_1_core>` core;
	auto :ref:`model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>` = core.:ref:`read_model <doxid-classov_1_1_core_1a3cca31e2bb5d569330daa8041e01f6f1>`(model_path);
	std::map<std::string, float> scale_factors;
	for (auto& input : :ref:`model <doxid-group__ov__runtime__cpp__prop__api_1ga461856fdfb6d7533dc53355aec9e9fad>`->inputs()) {
	    scale_factors[input.get_any_name()] = 1.0f;
	}
	core.:ref:`set_property <doxid-classov_1_1_core_1aa953cb0a1601dbc9a34ef6ba82b8476e>`("GNA", :ref:`ov::intel_gna::scale_factors_per_input <doxid-group__ov__runtime__gna__prop__cpp__api_1gaf72daf77f0c085f54b0a84f77c3d7734>`(scale_factors));

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1gafe83f57de302a35fa0d94563fab01e2d:
.. index:: pair: variable; firmware_model_image_path

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<std::string> ov::intel_gna::firmware_model_image_path {"GNA_FIRMWARE_MODEL_IMAGE"}

if turned on, dump GNA firmware model into specified file

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ga68ea397901af8f965863fbe599535341:
.. index:: pair: variable; execution_mode

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`ExecutionMode<doxid-group__ov__runtime__gna__prop__cpp__api_1gab1ef047d51bcaf91e5d2bbb1fd535499>`> ov::intel_gna::execution_mode {"GNA_DEVICE_MODE"}

GNA proc_type setting that should be one of AUTO, HW, GNA_HW_WITH_SW_FBACK, GNA_SW_EXACT or SW_FP32.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ga4ecfa3938d07be52618f606bb54ac429:
.. index:: pair: variable; execution_target

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`> ov::intel_gna::execution_target {"GNA_HW_EXECUTION_TARGET"}

The option to override the GNA HW execution target. May be one of GNA_2_0, GNA_3_0. By default (in case of no value set) the behavior depends on GNA HW availability: If GNA HW is present, use the option corresponding to this HW. If HW is not present, use the option corresponding to the latest fully supported GNA HW generation. A fully supported GNA HW generation means it must be supported by both the OV GNA Plugin and the core GNA Library. Currently, the latest supported GNA HW generation corresponds to GNA_3_0.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1gad9a766500212ccb6826b47aedde9e825:
.. index:: pair: variable; compile_target

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`HWGeneration<doxid-group__ov__runtime__gna__prop__cpp__api_1ga9d0c1cacd84e38e561fa71c6a818fc90>`> ov::intel_gna::compile_target {"GNA_HW_COMPILE_TARGET"}

The option to override the GNA HW compile target. May be one of GNA_2_0, GNA_3_0. By default the same as execution_target.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ga23eede6f1972f66534651d7946963953:
.. index:: pair: variable; memory_reuse

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<bool> ov::intel_gna::memory_reuse {"GNA_COMPACT_MODE"}

if enabled produced minimum memory footprint for compiled model in GNA memory, default value is true

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1ga4b02b547bf360236e72ab5aa9c8d1d44:
.. index:: pair: variable; pwl_design_algorithm

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<:ref:`PWLDesignAlgorithm<doxid-group__ov__runtime__gna__prop__cpp__api_1gadff8cc42104b8f3a8a4c50c08a45f6a3>`> ov::intel_gna::pwl_design_algorithm {"GNA_PWL_DESIGN_ALGORITHM"}

The option to set PWL design algorithm. By default the optimized algorithm called "Recursive Descent Algorithm for Finding
the Optimal Minimax Piecewise Linear Approximation of Convex Functions" is used. If value is UNIFORM_DISTRIBUTION then simple uniform distribution is used to create PWL approximation of activation functions. Uniform distribution usually gives poor approximation with the same number of segments.

.. _doxid-group__ov__runtime__gna__prop__cpp__api_1gaaf0afe1c01700ad7eed94783910c27fa:
.. index:: pair: variable; pwl_max_error_percent

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static constexpr :ref:`Property<doxid-classov_1_1_property>`<float> ov::intel_gna::pwl_max_error_percent {"GNA_PWL_MAX_ERROR_PERCENT"}

The option to allow to specify the maximum error percent that the optimized algorithm finding will be used to find PWL functions. By default (in case of NO value set), 1.0 value is used.

