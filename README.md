# GraphShap
Motif-based Explanations for Black-box Graph Classifiers

Most of the methods for explaining black-box classifiers  (e.g., on tabular data, images, or time series) rely on measuring the impact of removing sets of features from a model, thus forcing the explanation language to match the classifier input space. However, when dealing with graph data, in which the basic features are the edges, this seems not appropriate. In this paper we argue that (i) a good explanation method for graph classification should be fully agnostic with respect to the internal representation used by the black-box; and (ii) a good explanation language for graph classification tasks should be represented by higher order structures, such as motifs. The need to decouple the input space of the classifier from the explanation space (motifs) is thus the main challenge towards developing actionable explanations for a graph classification task. We introduce GraphShap, a Shapley-based approach able to provide motif-based explanations for black-box graph classifiers, assuming no knowledge whatsoever about the model or its training data: the only requirement is that the black-box can be queried at will. Our experiments on synthetic data with artificially injected motifs and on real-world brain networks confirm that GraphShap produces meaningful and compact explanations.

The code in this repository allows to re-obtain all results and plots from the paper.

PDF exports of the two notebooks have been added for read-only convenience.
