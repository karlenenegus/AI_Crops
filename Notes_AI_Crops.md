# AI & Crop Improvement

## AI

- Types:
  - Rule Based: User-defined rules; uses rules as knowledge representation
    - Decision Trees
    - Probability Modeling?
      - Bayesian networks?
    - Pathfinding algorithms
  - Learning Base: System-defined rules; learning systems create their own models
    - Machine learning
      - unsupervised
      - supervised
      - reinforcement

Deterministic vs Probabilistic
- Deterministic: outputs only most likely class
- Probabilistic: outputs probabilities for each class; provides representation of uncertainty

[Rutkoski et al. 2011](https://link.springer.com/article/10.1007/s10681-010-0301-1)

- GEBV accuracies can be used to calculate response from selection (R) where R = irσA with r=accuracy, i = selection intensity, and (sigma)A = square root of the additive genetic variance (Falconer and Mackay 1996, p189)  

- If linkage disequilibrium decay is more rapid in the selection candidate's population than in the training population, accuracies would decline because markers could segregate from the QTL they estimate in the training population

- When the population under selection was one generation removed from the training population, a greater number of replications of each training individual instead of a greater number of genotypes led to higher accuracies. This is due to the improved prediction of the genetic relationship between training and selecting candidates. When the population under selection was four generations removed from the training population, more genotypes rather than replicates in the training population increased GEBV accuracies because in this scenario the model relies more on estimation of marker effects due to linkage disequilibrium with QTL

  - Agrees with the trend of increased estimation of QTL effects from increased genotypes over increased replicates (Knapp and Bridges 1990)

- Ridge regression best linear unbiased prediction (RR-BLUP) simultaneously estimates all marker effects but assumes that markers are random effects with a common variance and shrinks all marker effects equally toward zero.

- Bayesian estimation methods were proposed to address the common variance assumption

  - Bayes-A: the prior distribution uses an inverted chi-squared distribution adjusted to match the mean and variances of the marker effects by adjusting the degrees of freedom and scalar parameters

  - In Bayes-B the prior distribution allows marker effects to equal zero and uses an inverted chi-squared distribution for marker effects greater than zero.

    - This adjustment yields a more realistic prior distribution because many markers are expected to have no effect on the trait of interest

- Accuracy of methods depends on strength of marker effects

  - When markers are in high linkage disequilibrium with few large-effect QTL capturing most of the genetic variance – Bayesian methods are most accurate

  - When many markers have small effects – RR-BLUP method is most accurate (Zhong et al. 2009)

Summary: Genomic selection can more effectively identify selection candidates for traits controlled by many small effect loci than MAS. MAS is more limited to identifying large effect loci which limits its use for improvement of multigenic traits. Genomic selection is used to train and validate a prediction model, use the model to predict breeding values of selection candidates, and make selections based on the predicted values. Genomic selection utilizes genome wide marker data to estimate and predict the total additive genetic variance. To apply genomic selection to populations far removed from the training population generation, sufficient linkage disequilibrium needs to exist between the markers and QTL for the predictive accuracy to be preserved. Additionally for long-term model accuracy, training populations must include appropriate germplasm selections to represent a broad range of families upon which GS may be made.    	 

[Jung et al 2021](https://www.sciencedirect.com/science/article/pii/S0958166920301257?via%3Dihub)

- Network types

    - Artificial neural networks (ANN), convolution neural networks (CNN), deep convolution neural networks (DCNN), deep neural network (DNN), fully convolutional network (FCN), region-convolutional neural network (R-CNN)

- Artificial Intelligence (AI) is recently gaining significant attention within agriculture disciplines because of its potential to leverage big data

[Harfouche et al. 2019](https://www.sciencedirect.com/science/article/pii/S0167779919301143?via%3Dihub)

Current implementations of AI

Neural networks (NNs)

Extreme gradient boosting

Deep learning (DL)

Phenomics (imaging)+ ML/DL

[Tong & Nikoloski 2021](https://www.sciencedirect.com/science/article/pii/S0176161720302443?via%3Dihub)



### Read:  

Heffner et al 2009

Jannink et al 2010 : methods for genomic prediction
