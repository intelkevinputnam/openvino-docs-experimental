.. index:: pair: class; ov::frontend::FrontEndManager
.. _doxid-classov_1_1frontend_1_1_front_end_manager:

class ov::frontend::FrontEndManager
===================================



Overview
~~~~~~~~

Frontend management class, loads available frontend plugins on construction Allows load of frontends for particular framework, register new and list available frontends This is a main frontend entry point for client applications. :ref:`More...<details-classov_1_1frontend_1_1_front_end_manager>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <manager.hpp>
	
	class FrontEndManager
	{
	public:
		// construction
	
		:ref:`FrontEndManager<doxid-classov_1_1frontend_1_1_front_end_manager_1a4ae2f62d331c3143a403774627b4b65e>`();
		:ref:`FrontEndManager<doxid-classov_1_1frontend_1_1_front_end_manager_1a1012f93d7717d96ab12d0d5675ab7023>`(FrontEndManager&&);

		// methods
	
		FrontEndManager& :ref:`operator =<doxid-classov_1_1frontend_1_1_front_end_manager_1a8fea6bc576c973b18e1b6db56f4c9f90>` (FrontEndManager&&);
		:ref:`FrontEnd::Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>` :ref:`load_by_framework<doxid-classov_1_1frontend_1_1_front_end_manager_1ab079dc1ae1d6bf9cc27f56e683e5a328>`(const std::string& framework);
	
		template <typename... Types>
		:ref:`FrontEnd::Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>` :ref:`load_by_model<doxid-classov_1_1frontend_1_1_front_end_manager_1addb6ad60a29ed43c2e7fd2b8c46cab72>`(const Types&... vars);
	
		std::vector<std::string> :ref:`get_available_front_ends<doxid-classov_1_1frontend_1_1_front_end_manager_1aa552205c95783eeb244423c449a5e52a>`();
		void :ref:`register_front_end<doxid-classov_1_1frontend_1_1_front_end_manager_1af9dbe8136142e711ca0585b9d24f6259>`(const std::string& name, :ref:`FrontEndFactory<doxid-namespaceov_1_1frontend_1ac5dc4ee362133b5e540e65cb606567f0>` creator);
		:ref:`FRONTEND_API<doxid-frontends_2common_2include_2openvino_2frontend_2visibility_8hpp_1acfd11755e29560fd36ce5369ba155288>` :ref:`FrontEnd::Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>` :target:`load_by_model<doxid-classov_1_1frontend_1_1_front_end_manager_1a7c94dc7f7b13be31bcc6501cfa8293a1>`(const std::vector<:ref:`ov::Any<doxid-classov_1_1_any>`>& variants);
	};
.. _details-classov_1_1frontend_1_1_front_end_manager:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Frontend management class, loads available frontend plugins on construction Allows load of frontends for particular framework, register new and list available frontends This is a main frontend entry point for client applications.

Construction
------------

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1a4ae2f62d331c3143a403774627b4b65e:
.. index:: pair: function; FrontEndManager

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FrontEndManager()

Default constructor. Searches and loads of available frontends.

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1a1012f93d7717d96ab12d0d5675ab7023:
.. index:: pair: function; FrontEndManager

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FrontEndManager(FrontEndManager&&)

Default move constructor.

Methods
-------

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1a8fea6bc576c973b18e1b6db56f4c9f90:
.. index:: pair: function; operator=

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FrontEndManager& operator = (FrontEndManager&&)

Default move assignment operator.

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1ab079dc1ae1d6bf9cc27f56e683e5a328:
.. index:: pair: function; load_by_framework

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`FrontEnd::Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>` load_by_framework(const std::string& framework)

Loads frontend by name of framework and capabilities.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- framework

		- Framework name. Throws exception if name is not in list of available frontends



.. rubric:: Returns:

Frontend interface for further loading of models

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1addb6ad60a29ed43c2e7fd2b8c46cab72:
.. index:: pair: function; load_by_model

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Types>
	:ref:`FrontEnd::Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>` load_by_model(const Types&... vars)

Loads frontend by model fragments described by each :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` documentation. Selects and loads appropriate frontend depending on model file extension and other file info (header)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vars

		- :ref:`Any <doxid-classov_1_1_any>` number of parameters of any type. What kind of parameters are accepted is determined by each :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` individually, typically it is std::string containing path to the model file. For more information please refer to specific :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` documentation.



.. rubric:: Returns:

Frontend interface for further loading of model. Returns 'nullptr' if no suitable frontend is found

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1aa552205c95783eeb244423c449a5e52a:
.. index:: pair: function; get_available_front_ends

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> get_available_front_ends()

Gets list of registered frontends. :ref:`Any <doxid-classov_1_1_any>` not loaded frontends will be loaded by this call.

.. _doxid-classov_1_1frontend_1_1_front_end_manager_1af9dbe8136142e711ca0585b9d24f6259:
.. index:: pair: function; register_front_end

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void register_front_end(const std::string& name, :ref:`FrontEndFactory<doxid-namespaceov_1_1frontend_1ac5dc4ee362133b5e540e65cb606567f0>` creator)

Register frontend with name and factory creation method.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Name of front end

	*
		- creator

		- Creation factory callback. Will be called when frontend is about to be created


