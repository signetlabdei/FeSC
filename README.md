# FeSC

This repo will contain the Matlab code that implements an architecture for Feature Selection with Consensus (FeSC).

The architecture clusters features using two (or more) clustering algorithms, and combine the output clusters computing the consensus among the algorithms, selecting those features for which the algorithms were in agreement.
The selected features are used to select part of the input data, which are than classified through SVM. 
Performance evaluation is done with 5-folds cross-validation and estimated in terms of classification accuracy.

## References
- G. Cisotto, M. Capuzzo, A. V. Guglielmi, and A. Zanella, “Feature selection for gesture recognition in Internet-
of-Things for healthcare”, International Conference on Communications (ICC), 7-11 June, 2020, Dublin, Ireland. Pre-published in ArXiV: http://arxiv.org/abs/2005.11031
