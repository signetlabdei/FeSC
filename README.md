# FeSC

This repo will contain the Matlab code that implements an architecture for Feature Selection with Consensus (FeSC).

The architecture clusters features using a nested cross-validation (CV) scheme.
Inside the inner CV, two (or more) clustering algorithms are employed to clusterize features, and their output is combined through consensus evaluation, to retain only the features for which the algorithms were in agreement.
The selected features are used to select part of the input data, which are than classified through SVM. 
Performance evaluation is done with 5-folds cross-validation and estimated in terms of classification accuracy. The selection of features achieving the best accurcay is selected.
This is done for each iteration of the outer-CV loop, obtaining, therefore, one optimal selection of feature for each iteration. Then, the best among them is selected. 
Finally, this selection of features is applied to the whole training set and an SVM is trained. The SVM model is then used to classify the test set.

The clustering algorithms employed are
- GC Spectral clustering
- Hierarchical clustering

A more detailed description of the ncv-FeSC algorithm is given in the paper linked below.

## References
- G. Cisotto, M. Capuzzo, A. V. Guglielmi, and A. Zanella, “Feature selection for gesture recognition in Internet-
of-Things for healthcare”, International Conference on Communications (ICC), 7-11 June, 2020, Dublin, Ireland. Pre-published in ArXiV: http://arxiv.org/abs/2005.11031
