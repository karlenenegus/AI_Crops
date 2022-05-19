# AI & Crop Improvement

## AI
- Types:
  - Rule Based: User-defined rules; uses rules as knowledge representation; simplest form of AI
    - Decision Trees (when conditionals are user specified)
      - some don't consider rules-based decision trees to be AI since users specify all the if...else conditionals
    - Probability Modeling?
      - Bayesian networks?
    - Pathfinding algorithms
  - Learning Base: System-defined rules; learning systems create their own models
    - Machine Learning
      - Unsupervised
        - Clustering
          - K-Means Clustering
          - Principle Component Analysis
        - Association
          - ...
      - Supervised
        - Regression (continuous output)
          - Linear regression
            - rrBLUP (linear mixed model)
            - GBLUP (linear mixed model)
          - Decision Trees (regression trees)
          - Random Forest (from regression trees)
          - Baysian regression models
            - BayesA
            - BayesB
            - BayesC
            - BayesCπ
          - reproducing kernels Hilbert spaces regression (RKHS)
          - support vector machine (SVM) regression
        - Classification (discreet output)
          - Logistic Regression
          - Support vector machine (SVM) classification
          - Decision Trees (conditional trees)
          - Random Forest (from conditional trees)
      - Reinforcement

Neural networks are often considered supervised machine learning. Deep learning often uses both supervised and unsupervised learning. Reinforcement algorithms almost always uses deep learning (layers)
- Neural networks
  - Number of layers:
    - Deep: neural networks have multiple hidden layers
    - Non-deep neural networks (shallow neural networks): only have one hidden layer (plus input and output layers)
  - Layer types:
      - pooling layer: apply a given function; do not have capacity to learning
      - convolutional layer: has parameters to learn; updates weights
  - Output type:
    - Deterministic: outputs only most likely class
    - Probabilistic(stochastic): outputs probabilities for each class; provides representation of uncertainty
  - Model adaptivity [(ref)](https://ieeexplore.ieee.org/abstract/document/180705)
    - Static
    - Dynamic
      - Feedforward: input signals are fed unidirectionally to output
        - Examples: MLPs and radial basis functions
      - Output Feedback: output signals are fed back to a previous layer
        - Examples of single layer, dynamic feedback network are Elman & Hopfield networks) [(ref)](https://subscription.packtpub.com/book/big_data_and_business_intelligence/9781788397872/1/ch01lvl1sec21/feed-forward-and-feedback-networks)
      - State Feedback: state-response pairs

Perspectives:
- feedback
  - supervised: explicit feedback (feedback is specified in the input data)
  - unsupervised: no feedback
  - reinforcement: implicit feedback (feedback is specified via output data)
- output
  - deterministic: outputs only most likely class
  - probabilistic: outputs probabilities for each class; provides representation of uncertainty
- input
  - supervised: explicit input(state)-response pairs
  - unsupervised: inputs lack specified responses
    - under the perspective of 'input' reinforcement learning becomes a type of unsupervised learning since reinforcement learning does not require input-output pairs
- patterns


Other
[Types of Neural Networks](https://www.mygreatlearning.com/blog/types-of-neural-networks/)
[Data Mining Text](https://link.springer.com/book/10.1007/978-0-387-36795-8?page=1&oscar-books=true#toc)
[Probabilistic Machine Learning Text](https://probml.github.io/pml-book/book1.html)

### [Rutkoski et al. 2011](https://link.springer.com/article/10.1007/s10681-010-0301-1)

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

### [Jung et al 2021](https://www.sciencedirect.com/science/article/pii/S0958166920301257?via%3Dihub)

- Network types

    - Artificial neural networks (ANN), convolution neural networks (CNN), deep convolution neural networks (DCNN), deep neural network (DNN), fully convolutional network (FCN), region-convolutional neural network (R-CNN)

- Artificial Intelligence (AI) is recently gaining significant attention within agriculture disciplines because of its potential to leverage big data

### [Harfouche et al. 2019](https://www.sciencedirect.com/science/article/pii/S0167779919301143?via%3Dihub)

Current implementations of AI

Neural networks (NNs)

Extreme gradient boosting

Deep learning (DL)

Phenomics (imaging)+ ML/DL

### [Tong & Nikoloski 2021](https://www.sciencedirect.com/science/article/pii/S0176161720302443?via%3Dihub)

- all genomic selection approaches rely on learning a mathematical relation between genotypic and phenotypic data that is later used for prediction.
  - By this definition, genomic selection approaches are part of supervised machine learning (aim to develop and analyze the performance of models using a set of training data)
- Types of Machine Learning
  - Unsupervised
    - identifies patterns in data without human supervision
    - relationships are established  in absence of input-response pairs
    - Ex: ordinary least squares regression
  - Supervised
    - requires input-response pairs (also called labeled training data)
    - uses training data to create learning model that maps inputs to responses
    - Ex: deep learning/artificial neural networks
  - Reinforcement
    - relies on feedback on model performance from dynamic environment while continuously improving the model building by maximizing the rewards
    - limited biological examples, recently DeepMind
- Genomic Selection Classification Criteria
    1. Statistical/machine learning techniques
      - regression
      - classification
      - deep learning

Multi-trait analysis methodologically similar to multi-environment trait analysis
Linear vs non-linear


Questions:
- are most regression based genomic selection models deterministic or probabilistic?
  - regression models output a single phenotypic value (class) which is Deterministic
  - probabilistic regression models do exist
  - uncertainty can arise from linear regression via
    - aleatoric uncertainty
      - uncertainty arising from data
    - epistemic uncertainty
      - uncertainty arising from regression model


### [(Bzdok et al. 2018)](https://www.nature.com/articles/nmeth.4642)

***Statistical methods***: focuses on inference
  - achieved through creation and fitting of a project specific model

| | Environment | Environment |
|----------------------|----|----|
|**Genotype (known)**  | 1  | 2  |
|**Genotype (unknown)**| 3  | 4  |

Only concerned with box 1

Provides quantitative measure of confidence in relationship describing true effects

***Machine Learning***: concentrates on prediction
- good for "wide data" (where # of inputs exceeds # of subjects)

As the complexity of the relationship captured by a statistical model increases & statistical inferences become less precise,  the boundary between statistical & machine learning approaches becomes less distinct

---
Notes: Statistics aims to provide interpretation, some machine learning model are uninterpretable (neural networks) and only provide predictions

### [Chapter 1 - (Montesinos Lopez et al. 2022)](https://link.springer.com/chapter/10.1007/978-3-030-89010-0_1)

The main characteristics of the training set are (a) it combines molecular (independent variables) and phenotypic (dependent variables) and (b) it contains enough observations (lines) and predictors (molecular data) to be able to train a statistical machine learning model with high generalized power to predict new lines.

The main characteristics of the testing set is that it contains genotypic data (markers) for a sample of observations (lines) and the goal is to predict the phenotypic or breeding values of lines that have been genotyped but not phenotyped.

GS has great potential for quickly improving complex traits with low heritability, as well as significantly reducing the cost of line and hybrid development.

Statistical machine learning tools often only approximate solutions to real-world problems by evaluating probabilistic distributions.

The creation of models using probability distributions and indicators (like confidence intervals) to evaluate the performance of predictions is a field of statistical machine learning.

Artificial Intelligence is the field of science that creates machines or devices that can mimic intelligent behaviors.

Statistical machine learning is a branch of AI that applies statistical methods to identify patterns in data using computers while also giving the computers the ability to learn without being explicitly programmed.

Statistical machine learning allows learning the relationship between two types of information, then one part of the information (input) can be used to predict the information lacking (output) in the other using the learned relationship.

GS implementation is challenging, since the quality of the data (phenotypic and genotypic) needs to be improved.

Statistical machine learning tools have the power to help increase the potential of GS if more powerful statistical machine learning methods are developed, if the existing methods can deal with larger data sets, and if these methods can be automatized to perform the prediction process with only a limited knowledge of the subject.

GS data are hampered by issues such as multicollinearity among markers (adjacent markers are highly correlated) and by a problem that consists of having a small number of observations and a large number of independent variables (commonly known as "large *p* and small *n*")(wide-data) which poses a statistical challenge.

Statistical machine learning methods continue to have difficulty carrying their experiences from one set of circumstances to another - this is known as transfer learning

**A model is a simplified description using mathematical tools of the processes we think that give rise to the observations in a set of data.** Statistical (or stochastic) models try to approximate exact solutions by evaluating probabilistic distributions. A statistical model is expressed by an equation composed of a *systematic* (deterministic) and a *random part*.

Writing a completely deterministic model is rarely possible because we'd need to know the mechanism that gives rise to the uniqueness of each individual. Instead we use probability distributions to characterize the observations measured in the individuals.

Statistical models can be described as:
$y_i = f(x_i) + \epsilon _i$, for $i = 1, 2, ..., n$

$f(x_i)$ is the systematic part of the model because it is *determined* by the explanatory variables (predictors)

$\epsilon_i$ is the error term which is independent of $x_i$ and has mean of zero

The set of approaches for estimating $f$ is called statistical learning.

There is no universally superior $f$ that can be used for all processes and because there is evidence that a set of assumptions that works well in one domain may work poorly in another - this is called the *no free lunch theorem*

When scientists are interested n understanding the relationship between each individual predictor (marker) and the response variable, what they really want is a model for inference

The type of statistical machine learning models used for testing causal hypothesis are usually association-based models applied to observational data. For example, regression models are one-type of association-based models used for testing causal hypotheses

**Statistical machine learning models**
- parametric: predictors take predetermined forms with the response; function that describes the relationship between the response and the explanatory variables is known
- semiparametric: part of the predictors do not take predetermined forms while the other part takes known forms with the response
- nonparametric: none of the predictors take predetermined forms with the response but are constructed according to information derived from data; these models require larger samples than parametric statistical machine learning models because the ddata must supply the model structure as well as the model estimates

**Model effects**
- fixed effects:  parameters associated with an entire population or with certain levels of experimental factors of interest
- random effects: individual experimental units are drawn at random from a population
- mixed-effects model: better suited to describe relationships between a response variable and some co-variates in data that are grouped according to one or more classification factors.

models with at least two sources of random variation are called hierarchical models or multilevel models

**Data types**

when ordinal data can be coded as numbers as in the case of stages of drought resistance from 1 to 5, we cannot say that a plant in stage 4 has drought resistance twice as strong as the resistance of a plant in stage 2. In ordinal data the differences between categories does not make sense. It is incorrect to present, for example, the average stage of drought resistance in a group of plants

**Types of learning**

*Supervised learning*: process of learning a function that maps an input to an output based on teaching the statistical machine learning method with input-output airs. The training data consist of pairs of objects: one component of the pair is the input data (predictors = explanatory variable = input) and the other, the desirable results (response variable = dependent variable = output)

*Unsupervised learning*: when you only have input (predictors = independent variables) and no previous knowledge of corresponding labeled outputs or response variables. The network uses training patterns to discover emerging collective properties and organizes the data into clusters. In unsupervised learning, there is no correct answer (output = response variable = dependent variable) and there is no teacher. For this reason, we are not interested in prediction since we do not have and associated response variable.

*Semi-supervised learning*: problems that have a large amount of input data available but only some of the data are labeled.


### Chapter 5 - Linear mixed models

Linear mixed models are flexible extensions of linear models in which fixed and random effects enter linearly into the model. Useful to model repeated, longitudinal, or clustered observations, in which random effects are introduced to help capture correlation or/and random variation among observations in the same group of individuals

There's an increasing number of applications of this model in genomic selection for plant and animal breeding, where molecular markers obtained by genotyping-by-sequencing or other technologies are used to predict breeding values  for non-phenotyped lines to select candidate lines prior to phenotypic evaluation.
### Read:  

Heffner et al 2009

Jannink et al 2010 : methods for genomic prediction

### Thoughts:
Review: Plant Breeding to Genomic Prediction

Methods:
[(Sandhu et al. 2021)](https://acsess.onlinelibrary.wiley.com/doi/10.1002/tpg2.20119)
[(Tong et al. 2021)](https://www.sciencedirect.com/science/article/pii/S0176161720302443?via%3Dihub)
- Regression
  - Linear mixed models
    - rrBLUP
  - GBLUP
  - Bayes A, B, C, Cpi
  - LASSO
  - elastic net
  - Baysian ridge regression
  - Baysian LASSO
  - Reproducing kernels Hilbert spaces regression
  - Random forest
  - Support vector machines
- Classification
  - Random forest
  - SVM
  - Sparse partial least squares discriminant analysis*
  - Probabilistic neural network
  - Rank*
- Neural Networks
  - Multilayer perceptron
  - Deep learning
  - Convolutional neural network
  - Multi-trait deep learning
  - Multivariate poisson deep learning
  - probabilistic neural network
  - radial basis function neural network (SVM use radial basis functions?)


### Outline
