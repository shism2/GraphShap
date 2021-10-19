# GraphShap
Motif-based Explanations for Black-box Graph Classifiers

Most methods for explaining black-box classifiers  (e.g., on tabular data, images, or time series) rely on measuring the impact that the removal/perturbation of features has on the model output. This forces the explanation language to match the classifier features space. However, when dealing with graph data, in which the basic features correspond essentially to the adjacency information describing the graph structure (i.e., the edges), this matching between features space and explanation language might not be appropriate. In this regard, we argue that (i) a good explanation method for graph classification should be fully agnostic with respect to the internal representation used by the black-box; and (ii) a good explanation language for graph classification tasks should be represented by higher-order structures, such as motifs. The need to decouple the feature space (edges) from the explanation space (motifs) is thus a major challenge towards developing actionable explanations for graph classification tasks.

In this paper we introduce GraphShap, a Shapley-based approach able to provide motif-based explanations for black-box graph classifiers, assuming no knowledge whatsoever about the model or its training data: the only requirement is that the black-box can be queried at will. For the sake of computational efficiency we explore a progressive approximation strategy and show how a simple kernel can efficiently approximate explanation scores, thus allowing GraphShap to scale on scenarios with a large explanation space (i.e., large number of motifs).

We devise a synthetic dataset generator with artificially injected motifs in order to empirically compare different masking approaches 
and to demonstrate that the proposed kernel is able to approximate the exact Shapley values with a computational complexity that is linear with respect to the number of explained features. Furthermore, we introduce additional auxiliary components such as a custom graph convolutional layer and algorithms for motif mining and ranking.

Finally, we test GraphShap on a real-world brain-network dataset consisting of patients affected by Autism Spectrum Disorder and a control group. Our experiments highlight how the classification provided by a black-box model can be effectively explained by few connectomics patterns.


The code in this repository allows to re-obtain all results and plots from the paper.
