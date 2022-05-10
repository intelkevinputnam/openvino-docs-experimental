.. index:: pair: struct; ov::op::v5::Loop::SpecialBodyPorts
.. _doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports:

struct ov::op::v5::Loop::SpecialBodyPorts
=========================================



Allows to define the purpose of inputs/outputs in the body.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <loop.hpp>
	
	struct SpecialBodyPorts
	{
		// fields
	
		int64_t :target:`current_iteration_input_idx<doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports_1a361bb6cb434fe9840d9349bc3d5345d3>` = -1;
		int64_t :target:`body_condition_output_idx<doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports_1a82151a739b95004805c5069202e6151a>` = -1;

		// construction
	
		:target:`SpecialBodyPorts<doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports_1aea6f90f5dd396c44fbdb915f11b11953>`();
	
		:target:`SpecialBodyPorts<doxid-structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports_1ac15f096551e9ed887c9a566c65ae16d7>`(
			int64_t in_current_iteration_input_idx,
			int64_t in_body_condition_output_idx
			);
	};

