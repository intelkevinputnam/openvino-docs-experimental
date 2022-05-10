.. index:: pair: class; ov::frontend::ProgressReporterExtension
.. _doxid-classov_1_1frontend_1_1_progress_reporter_extension:

class ov::frontend::ProgressReporterExtension
=============================================



Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <progress_reporter.hpp>
	
	class ProgressReporterExtension: public :ref:`ov::Extension<doxid-classov_1_1_extension>`
	{
	public:
		// typedefs
	
		typedef std::function<void(float, unsigned int, unsigned int)> :ref:`progress_notifier_callback<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a63e7403cde10ea92b14c9220a9f629c4>`;

		// construction
	
		:ref:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1aa9cd3aac120431b314233e50bcf7b2f8>`();
		:target:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a0929618a0ebc584618a87857246f3cfd>`(const :ref:`progress_notifier_callback<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a63e7403cde10ea92b14c9220a9f629c4>`& callback);
		:target:`ProgressReporterExtension<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1aea9df5d5f42f1a99125bfe0d51a8a460>`(:ref:`progress_notifier_callback<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a63e7403cde10ea92b14c9220a9f629c4>`&& callback);

		// methods
	
		void :ref:`report_progress<doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a4de56e2e7e3719d306ece00289369e0c>`(
			float progress,
			unsigned int total_steps,
			unsigned int completed_steps
			) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef std::shared_ptr<:ref:`Extension<doxid-classov_1_1_extension>`> :ref:`Ptr<doxid-classov_1_1_extension_1a1454e93b5f448c6b94d88a6515f135c5>`;

.. _details-classov_1_1frontend_1_1_progress_reporter_extension:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Typedefs
--------

.. _doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a63e7403cde10ea92b14c9220a9f629c4:
.. index:: pair: typedef; progress_notifier_callback

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<void(float, unsigned int, unsigned int)> progress_notifier_callback

A progress reporting callback signature. A FunctionObject that matches this signature should be passed to the constructor of this extension. The extension will then invoke this as a callback each time the progress needs to be reported. The callback itself is responsible for consuming the reported values.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- progress

		- A float value in the range [0.0, 1.0] indicating the total progress of an operation.

	*
		- total_steps

		- The total number of steps that a given instance of this extension is tracking

	*
		- completed_completed

		- The current number of completed steps (out of the total number of steps to take)

Construction
------------

.. _doxid-classov_1_1frontend_1_1_progress_reporter_extension_1aa9cd3aac120431b314233e50bcf7b2f8:
.. index:: pair: function; ProgressReporterExtension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ProgressReporterExtension()

The default constructor which creates a reporter that doesn't report progress.

Methods
-------

.. _doxid-classov_1_1frontend_1_1_progress_reporter_extension_1a4de56e2e7e3719d306ece00289369e0c:
.. index:: pair: function; report_progress

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void report_progress(
		float progress,
		unsigned int total_steps,
		unsigned int completed_steps
		) const

The main method of this extension used to report the progress. This method forwards its arguments to the callback stored in this class.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- progress

		- A float value in the range [0.0, 1.0] indicating the total progress of an operation.

	*
		- total_steps

		- The total number of steps that a given instance of this extension is tracking

	*
		- completed_steps

		- The current number of completed steps (out of the total number of steps to take)


