.. index:: pair: enum; levels
.. _doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950d:

enum ngraph::pass::low_precision::levels
========================================



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <layer_transformation.hpp>

	enum levels
	{
	    :target:`int4<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da8c688c73219b09838a67bd8286375458>`               = 16,
	    :target:`int4_narrow_range<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da1be813d1cc0f1e55b8b38dedc7fdd34b>`  = 15,
	    :target:`int8<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da7c28a536d4380ba409ec9b76bbcc8394>`               = 256,
	    :target:`int8_narrow_range<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da14e0dd141af5ef959d6ff9ec98c6b12f>`  = 255,
	    :target:`int16<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da81c72c01fa1f4e71b8df0fb64fbec719>`              = 65536,
	    :target:`int16_narrow_range<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da09f93d8b417daba8be6c2d14a5c41d50>` = 65535,
	    :target:`int32<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da67079b0dd13afe2704d076826fcdac43>`              = size_t(4294967296),
	    :target:`int32_narrow_range<doxid-namespacengraph_1_1pass_1_1low__precision_1a67a8738db238c117213c348a4c5f950da2d28ab60af2c80e55be58d36b8ae895f>` = 4294967295,
	};

