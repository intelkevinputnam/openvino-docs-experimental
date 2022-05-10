.. index:: pair: class; InferenceEngine::LayerNameLess
.. _doxid-class_inference_engine_1_1_layer_name_less:

class InferenceEngine::LayerNameLess
====================================



to allow storing of LayersSP in collections ordered by names


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <graph_tools.hpp>
	
	class LayerNameLess
	{
	public:
		// methods
	
		bool :target:`operator ()<doxid-class_inference_engine_1_1_layer_name_less_1adda63f5477fc8fba5228c5d28dcae6e3>` (const :ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`& lhs, const :ref:`CNNLayerPtr<doxid-namespace_inference_engine_1af972e334feb2788341e38ac3e6103e60>`& rhs) const;
	};

