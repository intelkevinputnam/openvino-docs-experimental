.. index:: pair: class; ov::Busy
.. _doxid-classov_1_1_busy:

class ov::Busy
==============



Thrown in case of calling the :ref:`InferRequest <doxid-classov_1_1_infer_request>` methods while the request is busy with compute operation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <exception.hpp>
	
	class Busy: public :ref:`ov::Exception<doxid-classov_1_1_exception>`
	{
	};

