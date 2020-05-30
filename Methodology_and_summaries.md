# Methodology

Concepts:
1) Cost-sensitive:  Cost sensitive learning assigns diﬀerent penalties for the misclassiﬁcation of diﬀerent classes so that more penalties will be given if points in minority classes are misclassiﬁed to majority classes
2)Resampling based learning methods are to oversample the minority and undersample the majority, which can be further divided into random oversampling/undersampling , synthetic oversampling/undersampling and other variants, e.g. data cleaning approaches.


# Summaries

1) Model-Based Oversampling for Imbalanced Sequence Classification
- based in the 'generative' models of sequences.In particular, a recurrent neural network was employed to learn the generative mechanics for sequences as representations for the corresponding sequences. These generative models are then utilized to form a kernel to capture the similarity between diﬀerent sequences

-Resampling based learning methods are to oversample the minority and undersample the majority, which can be further divided into random oversampling/undersampling, synthetic oversampling/undersampling and other variants, e.g. data cleaning approaches .

- SMOTE,BorderSMOTE, ADASYN do not match the temporal dynamics of sequences.

-  In this paper proposes an algorithm that generates new synthetic data in a model-spanned representation space. In particular, they ﬁrst learn representations for sequences to take advantage of the sequential order information using a special kind of recurrent neural network (RNN). Then the sequence representations are utilized to compute a kernel to preserve the similarity constraints. The representations and kernel parameter are tuned iteratively for better representation and discrimination. Finally, in the learned kernel feature space, oversampling is performed

- Algorithm: 1 ) Use the CRJ network to fit models for sequences in T(training set)
2) Compte empirical kernel acc. eq3
3) Tune networkparameters acc. eq5
4) Tune Kernel parameter according to eq11

2) Integrated Oversampling (INOS) for Imbalanced Time Series Clasification
- Introduced an enhanced structure preserving oversampling (ESPO) technique and synergistically combine it with interpolation-based oversampling methods. ESPO 
- Two objectives : i) preserve the regularized eigen covariance structure which can be estimated using the limited positive time series samples 
ii) the other is to be able to provide adequate emphasis on the key minority samples with remaining oversampling capacity.
