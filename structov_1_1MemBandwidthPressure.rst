.. index:: pair: struct; ov::MemBandwidthPressure
.. _doxid-structov_1_1_mem_bandwidth_pressure:

struct ov::MemBandwidthPressure
===============================






.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <performance_heuristics.hpp>
	
	struct MemBandwidthPressure
	{
		// fields
	
		float :target:`max_mem_tolerance<doxid-structov_1_1_mem_bandwidth_pressure_1a00d7f353feda3767a8dc585960e9bf50>` = :ref:`UNKNOWN<doxid-structov_1_1_mem_bandwidth_pressure_1afad35953b515f47a75bb8257a5f51ebb>`;
		float :target:`ratio_compute_convs<doxid-structov_1_1_mem_bandwidth_pressure_1a80e54dd62c8a4c4828f92b3f8ffc0e63>` = 0;
		float :target:`ratio_mem_limited_convs<doxid-structov_1_1_mem_bandwidth_pressure_1add8f16c0996ba45c868fa9ced8fa1683>` = 0;
		float :target:`ratio_compute_deconvs<doxid-structov_1_1_mem_bandwidth_pressure_1a49db740b2ce38c6f48a459b1d8aae3d5>` = 0;
		static constexpr float :target:`UNKNOWN<doxid-structov_1_1_mem_bandwidth_pressure_1afad35953b515f47a75bb8257a5f51ebb>` = FLT_MAX;
		static constexpr float :target:`ALL<doxid-structov_1_1_mem_bandwidth_pressure_1a90db072790d1a6c0c2e74f36d8b17713>` = 1.0f;
		static constexpr float :target:`NONE<doxid-structov_1_1_mem_bandwidth_pressure_1a1cece9f294d94d26bf49c6934a1db21b>` = 0.0f;
		static constexpr float :target:`LIMITED<doxid-structov_1_1_mem_bandwidth_pressure_1aaecf28fe40418116e7f80c50dbb27f35>` = 0.5f;
	};

