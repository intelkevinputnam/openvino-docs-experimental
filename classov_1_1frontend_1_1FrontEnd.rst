.. index:: pair: class; ov::frontend::FrontEnd
.. _doxid-classov_1_1frontend_1_1_front_end:

class ov::frontend::FrontEnd
============================



Overview
~~~~~~~~

An interface for identifying a frontend for a particular framework. Provides an ability to load and convert of input model. :ref:`More...<details-classov_1_1frontend_1_1_front_end>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <frontend.hpp>
	
	class FrontEnd
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<FrontEnd> :target:`Ptr<doxid-classov_1_1frontend_1_1_front_end_1af08fa70977c5ba7d9b9a41f23aaf792d>`;

		// construction
	
		:ref:`FrontEnd<doxid-classov_1_1frontend_1_1_front_end_1a20591a02dbe0f1e220d9c3a66d12ed8d>`();
		:target:`FrontEnd<doxid-classov_1_1frontend_1_1_front_end_1a78220b7ca4caaa55a76c7c53a1f0b4c5>`(const FrontEnd&);
		:target:`FrontEnd<doxid-classov_1_1frontend_1_1_front_end_1af7fd1c5681663a55e8dab267a2ff1b24>`(FrontEnd&&);

		// methods
	
		FrontEnd& :target:`operator =<doxid-classov_1_1frontend_1_1_front_end_1a63238be5eeb7f49a95b24a5d7d72aed3>` (const FrontEnd&);
		FrontEnd& :target:`operator =<doxid-classov_1_1frontend_1_1_front_end_1a1d320e28b80be810e203ca858ada5fc8>` (FrontEnd&&);
	
		template <typename... Types>
		bool :ref:`supported<doxid-classov_1_1frontend_1_1_front_end_1adfeebe8e859068995fdf7f5646cd6ca6>`(const Types&... vars) const;
	
		template <typename... Types>
		:ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>` :ref:`load<doxid-classov_1_1frontend_1_1_front_end_1a3cdf022bd820be68f2cf8536b431222b>`(const Types&... vars) const;
	
		:ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>` :target:`load<doxid-classov_1_1frontend_1_1_front_end_1a653821b9a52e924a41b89a28284d69fe>`(const :ref:`ov::AnyVector<doxid-namespaceov_1a730f82cac7504a622d0d3c27d547a2c7>`& vars) const;
		virtual std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> :ref:`convert<doxid-classov_1_1frontend_1_1_front_end_1a95614f78f8143dfc764a5e614dfb224a>`(const :ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`& model) const;
		virtual void :ref:`convert<doxid-classov_1_1frontend_1_1_front_end_1a02517ed9bb9c8227dc8c8c94a2249269>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& partially_converted) const;
		virtual std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> :ref:`convert_partially<doxid-classov_1_1frontend_1_1_front_end_1a16a5bd59e2fe57bba2dc5b7f995d9fc6>`(const :ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`& model) const;
		virtual std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> :ref:`decode<doxid-classov_1_1frontend_1_1_front_end_1aa584111cc5e96999cf356a5ae65cc22c>`(const :ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`& model) const;
		virtual void :ref:`normalize<doxid-classov_1_1frontend_1_1_front_end_1a3bb2ab3c395b4a76476f8af0c55d2a5b>`(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& model) const;
		virtual std::string :ref:`get_name<doxid-classov_1_1frontend_1_1_front_end_1a969a49f1b555efada7d497ed8c6bf4b1>`() const;
		virtual void :ref:`add_extension<doxid-classov_1_1frontend_1_1_front_end_1aa37591d4b10d02b7f31d0468c1365f22>`(const std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>& extension);
		void :ref:`add_extension<doxid-classov_1_1frontend_1_1_front_end_1ae763d4fc7f6c316582e7d1d074759520>`(const std::vector<std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>>& extensions);
		void :ref:`add_extension<doxid-classov_1_1frontend_1_1_front_end_1a16b60ef3b1dcdfd4a5f2dbbda6a1f819>`(const std::string& library_path);
	
		template <
			class T,
			typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
			>
		void :ref:`add_extension<doxid-classov_1_1frontend_1_1_front_end_1a76185d2ad8e9301f127640774fdde18d>`(const T& extension);
	
		template <
			class T,
			class... Targs,
			typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
			>
		void :ref:`add_extension<doxid-classov_1_1frontend_1_1_front_end_1a564ce147806ea05920fec970effbe726>`(
			const T& extension,
			Targs... args
			);
	
		bool :target:`supported<doxid-classov_1_1frontend_1_1_front_end_1aaf16e03c08a2d4c05612285c48f0564a>`(const std::vector<:ref:`ov::Any<doxid-classov_1_1_any>`>& variants) const;
	};
.. _details-classov_1_1frontend_1_1_front_end:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

An interface for identifying a frontend for a particular framework. Provides an ability to load and convert of input model.

Construction
------------

.. _doxid-classov_1_1frontend_1_1_front_end_1a20591a02dbe0f1e220d9c3a66d12ed8d:
.. index:: pair: function; FrontEnd

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FrontEnd()

Default constructor.

Methods
-------

.. _doxid-classov_1_1frontend_1_1_front_end_1adfeebe8e859068995fdf7f5646cd6ca6:
.. index:: pair: function; supported

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Types>
	bool supported(const Types&... vars) const

Validates if :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` can recognize model with parameters specified. Same parameters should be used to load model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vars

		- :ref:`Any <doxid-classov_1_1_any>` number of parameters of any type. What kind of parameters are accepted is determined by each :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` individually, typically it is std::string containing path to the model file. For more information please refer to specific :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` documentation.



.. rubric:: Returns:

true if model recognized, false - otherwise.

.. _doxid-classov_1_1frontend_1_1_front_end_1a3cdf022bd820be68f2cf8536b431222b:
.. index:: pair: function; load

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename... Types>
	:ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>` load(const Types&... vars) const

Loads an input model by any specified arguments. Each :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` separately defines what arguments it can accept.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vars

		- :ref:`Any <doxid-classov_1_1_any>` number of parameters of any type. What kind of parameters are accepted is determined by each :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` individually, typically it is std::string containing path to the model file. For more information please refer to specific :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>` documentation.



.. rubric:: Returns:

Loaded input model.

.. _doxid-classov_1_1frontend_1_1_front_end_1a95614f78f8143dfc764a5e614dfb224a:
.. index:: pair: function; convert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> convert(const :ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`& model) const

Completely convert and normalize entire :ref:`Model <doxid-classov_1_1_model>`, throws if it is not possible.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- :ref:`Input <doxid-classov_1_1_input>` model



.. rubric:: Returns:

fully converted OV :ref:`Model <doxid-classov_1_1_model>`

.. _doxid-classov_1_1frontend_1_1_front_end_1a02517ed9bb9c8227dc8c8c94a2249269:
.. index:: pair: function; convert

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void convert(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& partially_converted) const

Completely convert the remaining, not converted part of a :ref:`Model <doxid-classov_1_1_model>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- partiallyConverted

		- partially converted OV :ref:`Model <doxid-classov_1_1_model>`

.. _doxid-classov_1_1frontend_1_1_front_end_1a16a5bd59e2fe57bba2dc5b7f995d9fc6:
.. index:: pair: function; convert_partially

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> convert_partially(const :ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`& model) const

Convert only those parts of the model that can be converted leaving others as-is. Converted parts are not normalized by additional transformations; normalize :ref:`Model <doxid-classov_1_1_model>` or another form of convert :ref:`Model <doxid-classov_1_1_model>` should be called to finalize the conversion process.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- :ref:`Input <doxid-classov_1_1_input>` model



.. rubric:: Returns:

partially converted OV :ref:`Model <doxid-classov_1_1_model>`

.. _doxid-classov_1_1frontend_1_1_front_end_1aa584111cc5e96999cf356a5ae65cc22c:
.. index:: pair: function; decode

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`> decode(const :ref:`InputModel::Ptr<doxid-classov_1_1frontend_1_1_input_model_1a384879771dc22a100d918d4ee612e194>`& model) const

Convert operations with one-to-one mapping with decoding nodes. Each decoding node is an OV node representing a single FW operation node with all attributes represented in FW-independent way.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- model

		- :ref:`Input <doxid-classov_1_1_input>` model



.. rubric:: Returns:

OV :ref:`Model <doxid-classov_1_1_model>` after decoding

.. _doxid-classov_1_1frontend_1_1_front_end_1a3bb2ab3c395b4a76476f8af0c55d2a5b:
.. index:: pair: function; normalize

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void normalize(const std::shared_ptr<:ref:`ov::Model<doxid-classov_1_1_model>`>& model) const

Runs normalization passes on :ref:`Model <doxid-classov_1_1_model>` that was loaded with partial conversion.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`Model <doxid-classov_1_1_model>`

		- partially converted OV :ref:`Model <doxid-classov_1_1_model>`

.. _doxid-classov_1_1frontend_1_1_front_end_1a969a49f1b555efada7d497ed8c6bf4b1:
.. index:: pair: function; get_name

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string get_name() const

Gets name of this :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>`. Can be used by clients if frontend is selected automatically by :ref:`FrontEndManager::load_by_model <doxid-classov_1_1frontend_1_1_front_end_manager_1addb6ad60a29ed43c2e7fd2b8c46cab72>`.



.. rubric:: Returns:

Current frontend name. Empty string if not implemented

.. _doxid-classov_1_1frontend_1_1_front_end_1aa37591d4b10d02b7f31d0468c1365f22:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void add_extension(const std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>& extension)

Register base extension in the :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- base extension

.. _doxid-classov_1_1frontend_1_1_front_end_1ae763d4fc7f6c316582e7d1d074759520:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_extension(const std::vector<std::shared_ptr<:ref:`ov::Extension<doxid-classov_1_1_extension>`>>& extensions)

Register base extensions in the :ref:`FrontEnd <doxid-classov_1_1frontend_1_1_front_end>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extensions

		- vector of extensions

.. _doxid-classov_1_1frontend_1_1_front_end_1a16b60ef3b1dcdfd4a5f2dbbda6a1f819:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_extension(const std::string& library_path)

Registers extension.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- library_path

		- path to library with :ref:`ov::Extension <doxid-classov_1_1_extension>`

.. _doxid-classov_1_1frontend_1_1_front_end_1a76185d2ad8e9301f127640774fdde18d:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
		>
	void add_extension(const T& extension)

Registers extension.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- :ref:`Extension <doxid-classov_1_1_extension>` class which is inherited from :ref:`ov::BaseOpExtension <doxid-classov_1_1_base_op_extension>` class

.. _doxid-classov_1_1frontend_1_1_front_end_1a564ce147806ea05920fec970effbe726:
.. index:: pair: function; add_extension

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <
		class T,
		class... Targs,
		typename std::enable_if<std::is_base_of<ov::Extension, T>::value, bool>::type = true
		>
	void add_extension(
		const T& extension,
		Targs... args
		)

Registers extensions.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- extension

		- :ref:`Extension <doxid-classov_1_1_extension>` class which is inherited from :ref:`ov::Extension <doxid-classov_1_1_extension>` class


