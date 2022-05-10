.. index:: pair: class; ov::intel_gpu::ocl::ClImage2DTensor
.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor:

class ov::intel_gpu::ocl::ClImage2DTensor
=========================================



Overview
~~~~~~~~

This class represents an abstraction for GPU plugin remote tensor which can be shared with user-supplied OpenCL 2D Image. The plugin object derived from this class can be obtained with :ref:`ClContext::create_tensor() <doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1ac1735cf031cfde65e2ced782b21cc256>` call. :ref:`More...<details-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ocl.hpp>
	
	class ClImage2DTensor: public :ref:`ov::RemoteTensor<doxid-classov_1_1_remote_tensor>`
	{
	public:
		// methods
	
		static void :ref:`type_check<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1a7fd0b5937795885dd74e93542536041c>`(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
		cl_mem :ref:`get<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1a8ed30d7e79bdd57f8a99aefff6a677a8>`();
		:ref:`operator cl_mem<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1af31cb6f2f13ce797c03283d32ad5851a>` ();
		:ref:`operator cl::Image2D<doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1a2dcf188200399c1eb57bce4c10eec251>` ();
	};

	// direct descendants

	class :ref:`D3DSurface2DTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor>`;
	class :ref:`VASurfaceTensor<doxid-classov_1_1intel__gpu_1_1ocl_1_1_v_a_surface_tensor>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		:ref:`Tensor<doxid-classov_1_1_tensor>`& :ref:`operator =<doxid-classov_1_1_tensor_1a83b0b800c932eca2a5e9d42dfdae655c>` (const :ref:`Tensor<doxid-classov_1_1_tensor>`& other);
		:ref:`Tensor<doxid-classov_1_1_tensor>`& :ref:`operator =<doxid-classov_1_1_tensor_1a3cf1d342fa056b59fd5bc38964d54575>` (:ref:`Tensor<doxid-classov_1_1_tensor>`&& other);
		void :ref:`set_shape<doxid-classov_1_1_tensor_1a7a513a53ac7221d1a52006c34bce6c18>`(const :ref:`ov::Shape<doxid-classov_1_1_shape>`& shape);
		:ref:`element::Type<doxid-classov_1_1element_1_1_type>` :ref:`get_element_type<doxid-classov_1_1_tensor_1a7b00f757407bfee07d831647f15b1686>`() const;
		:ref:`Shape<doxid-classov_1_1_shape>` :ref:`get_shape<doxid-classov_1_1_tensor_1a706163e01fb555eb9ccdfb5204cf7834>`() const;
		size_t :ref:`get_size<doxid-classov_1_1_tensor_1a26dfed6a65b46d9a25562e811912f09d>`() const;
		size_t :ref:`get_byte_size<doxid-classov_1_1_tensor_1ae540fcafc1e9dc9181e86a1ec2682935>`() const;
		:ref:`Strides<doxid-classov_1_1_strides>` :ref:`get_strides<doxid-classov_1_1_tensor_1a610491239de68e700c7c3579479b6692>`() const;
		void \* :ref:`data<doxid-classov_1_1_tensor_1ac1b8835f54d67d92969d7979e666e2a8>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>` type = {}) const;
	
		template <typename T, typename datatype = typename std::decay<T>::type>
		T \* :ref:`data<doxid-classov_1_1_tensor_1ae73e29ecaf40339a7b4f6b65cdde0736>`() const;
	
		bool :ref:`operator !<doxid-classov_1_1_tensor_1aa65688ce884468fdd9bd9cc24dda907a>` () const;
		:ref:`operator bool<doxid-classov_1_1_tensor_1a7ac03a96d3eeca3f057307bccb095df5>` () const;
	
		template <typename T>
		std::enable_if<std::is_base_of<:ref:`Tensor<doxid-classov_1_1_tensor>`, T>::value, bool>::type :ref:`is<doxid-classov_1_1_tensor_1a287c90f6c44793fd411e26490786c83d>`() const;
	
		template <typename T>
		const std::enable_if<std::is_base_of<:ref:`Tensor<doxid-classov_1_1_tensor>`, T>::value, T>::type :ref:`as<doxid-classov_1_1_tensor_1a345f8ade85da6fe30bcf8a3ae15a4bca>`() const;
	
		static void :ref:`type_check<doxid-classov_1_1_tensor_1a8beef8846cacaa542e3b51c061d50e42>`(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor);
	
		static void :ref:`type_check<doxid-classov_1_1_remote_tensor_1a5fd48aa60181ecea3e19e5e1629a660d>`(
			const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor,
			const std::map<std::string, std::vector<std::string>>& type_info = {}
			);
	
		void \* :ref:`data<doxid-classov_1_1_remote_tensor_1a84a2a19a0db87daf881eb5525767dc8c>`(const :ref:`element::Type<doxid-classov_1_1element_1_1_type>`);
	
		template <typename T>
		T \* :ref:`data<doxid-classov_1_1_remote_tensor_1a8f2c25380dc70bf6d90bab6ecb2757e1>`();
	
		:ref:`ov::AnyMap<doxid-namespaceov_1a51d339c5ba0d88c4a1397c791430af88>` :ref:`get_params<doxid-classov_1_1_remote_tensor_1aecdf1dc2e396c38b58a45b6d0202a0b3>`() const;

.. _details-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class represents an abstraction for GPU plugin remote tensor which can be shared with user-supplied OpenCL 2D Image. The plugin object derived from this class can be obtained with :ref:`ClContext::create_tensor() <doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context_1ac1735cf031cfde65e2ced782b21cc256>` call.

User can obtain OpenCL image handle from this class.

Methods
-------

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1a7fd0b5937795885dd74e93542536041c:
.. index:: pair: function; type_check

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void type_check(const :ref:`Tensor<doxid-classov_1_1_tensor>`& tensor)

Checks that type defined runtime parameters are presented in remote object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- tensor

		- a tensor to check

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1a8ed30d7e79bdd57f8a99aefff6a677a8:
.. index:: pair: function; get

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	cl_mem get()

Returns the underlying OpenCL memory object handle.



.. rubric:: Returns:

underlying OpenCL memory object handle

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1af31cb6f2f13ce797c03283d32ad5851a:
.. index:: pair: function; operator cl_mem

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator cl_mem ()

OpenCL memory handle conversion operator.



.. rubric:: Returns:

``cl_mem``

.. _doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor_1a2dcf188200399c1eb57bce4c10eec251:
.. index:: pair: function; operator cl::Image2D

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	operator cl::Image2D ()

Standard Khronos cl::Image2D wrapper conversion operator for the :ref:`ClContext <doxid-classov_1_1intel__gpu_1_1ocl_1_1_cl_context>` object.



.. rubric:: Returns:

``cl::Image2D`` object


