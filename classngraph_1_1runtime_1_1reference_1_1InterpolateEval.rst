.. index:: pair: class; ngraph::runtime::reference::InterpolateEval
.. _doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval:

class ngraph::runtime::reference::InterpolateEval
=================================================



Overview
~~~~~~~~

Class to perform interpolation calculation. :ref:`More...<details-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <interpolate.hpp>
	
	template <typename T>
	class InterpolateEval
	{
	public:
		// construction
	
		:target:`InterpolateEval<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_1a78aa8a08ad3f3f82c5cd1c3d6bc310c0>`();
		:ref:`InterpolateEval<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_1a2cdcd496f60363f3547453663e319e83>`(const :ref:`op::v4::Interpolate::InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs>`& attrs);

		// methods
	
		void :ref:`operator ()<doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_1a5bda4a8eb2f66d4b2d9d3036694b6d5e>` (
			const T \* input_data,
			const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
			const std::vector<float>& scales,
			const std::vector<int64_t>& axes,
			T \* out,
			const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape
			);
	};
.. _details-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class to perform interpolation calculation.

Construction
------------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_1a2cdcd496f60363f3547453663e319e83:
.. index:: pair: function; InterpolateEval

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	InterpolateEval(const :ref:`op::v4::Interpolate::InterpolateAttrs<doxid-structov_1_1op_1_1v4_1_1_interpolate_1_1_interpolate_attrs>`& attrs)

Constructs interpolation calculation using Interpolate attributes.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- attrs

		- Interpolate-4 attributes.

Methods
-------

.. _doxid-classngraph_1_1runtime_1_1reference_1_1_interpolate_eval_1a5bda4a8eb2f66d4b2d9d3036694b6d5e:
.. index:: pair: function; operator()

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void operator () (
		const T \* input_data,
		const :ref:`Shape<doxid-classov_1_1_shape>`& input_data_shape,
		const std::vector<float>& scales,
		const std::vector<int64_t>& axes,
		T \* out,
		const :ref:`Shape<doxid-classov_1_1_shape>`& out_shape
		)

Performing interpolation calculation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- input_data

		- pointer to input data

	*
		- input_data_shape

		- shape of the input data

	*
		- scales

		- scale factors for each interpolated axis

	*
		- axes

		- axes to interpolate

	*
		- out

		- pointer to memory block for output data

	*
		- out_shape

		- shape of output data


