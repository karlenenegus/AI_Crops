---
title: "AI and Crop Improvement"
author:
- name: Karlene Negus
  affiliation: Iowa State University
  email: knegus@iastate.edu
date: June 2022
abstract: "Lorem ipsum dolor sit amet."
bibliography: "../../Grad_ISU/library.bib"
link-citations: true
link-bibliography: true
geometry: margin = 1in
urlcolor: "red"
toc: true
csl: "./csl/theoretical-and-applied-genetics.csl"
...

<!---
# Example Section

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua

In-text reference to Fig. {@fig:phybreed1}.

![Caption.](../Images/PhysiologicalBreeding.jpg){#fig:phybreed1}

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua citation [@Duvick2005]. See sec. @sec:example-section
-->
# Crop Improvement

To achieve a rate of yield increase that keeps pace with the growing world population, new approaches to crop improvement will be required.

## Modern Crop Improvement

Conventional breeding took advantage of traditional phenotyping methods to inform crossing and selection.

Prior issues facing crop improvement research revolved around data accumulation. Genotyping methods prior to NGS were laborious and limited quantities of genotypes were achievable. Traditional phenotyping methods are time intensive and sometimes limited by the expertise of evaluators. Envirotyping was difficult to achieve with useful levels of resolution. The post-NGS sequencing technology era has made sequencing whole genomes a feasible genotyping approach. image-based phenotyping and other high throughput techniques generate terabytes of data every growing season. Remote sensing technologies have made observing envirotypes within a single field possible.

<!--- phenotyping + selection + genotyping -->
With the increase in genetic technology availability and decrease in cost during the (1980s-2000s), targeted improvements through approaches such as marker assisted selection became feasible. Genetic improvement was seen as the new way forward in contrast to the plateauing gains made from cultural practices. Genetic data became abundant in the next-generation sequencing era. Earlier QTL studies have identified many loci with large contributions to highly heritable traits. Traits with unresolved genetic architecture, result from the contributions of many, small effect loci. QTL studies in such traits require extensive phenotyping and are often not stable across environment.

<!--- phenotyping + selection + genotyping = resulting problems -->



<!---In recent years focus has returned to approaching crop improvement from all angles. An example of a breeding approach that integrates many different types of data is physiological breeding. Reynolds and Langridge [-@Reynolds2016] break physiological breeding into 6 parts - crops design, genetic resource exploration, phenotyping, genetic analysis, hybridization and progeny selection, and genetic gain evaluation via multi-location testing. This framework helps describe the purpose of obtaining genomic, phenomic and enviromic data during the current breeding cycle and why dissection of traits, genetically and physiologically, is important for -->


Modern crop improvement has the advantage and challenge of access to large genomic, phenomic and enviromic data sets<!--- genomic, phenomic and enviromic should have been defined in earlier section --> to inform breeding and selection decisions. A single population can now produce dramatically more data then was cumulatively obtained in the breeding process in previous decades. The prior issues of genotyping and phenotyping bottlenecks have been largely overcome with higher levels of automation achieved through approaches like GBS NGS sequencing technologies <!--- more specific -->, HTP, and remote sensing <!--- These should have been mentioned previously -->. However, these solutions and the accompanying "big data" also lend new issues to the field of crop improvement. Fully exploiting "-omic" data in an efficient manor is difficult with prior approaches<!--like...-->. There is now a need for new methods of analysis which effective and efficient in order to continue bridging the gap between observed genotypes and observed phenotypes. AI has the potential to provide diverse solutions to these ends.

# AI

Artificial intelligence (AI) is concerned with the process of designing computers that can think and act humanly and rationally [@Russsel2009]. In recent years, AI has been increasingly explored as a means to analyze big data most popularly through machine learning (ML) approaches. However in addition to ML, AI encompasses a number of diverse sub-fields which can can be generally categorized as symbolic or sub-symbolic [@Nilsson1998; @ilkou2020]. 

## Symbolic AI
The AI approaches which represent knowledge through physical symbols [@Hoehndorf2017] are described using names like symbolic AI, logical AI, or computationalism [@Hoehndorf2017; @Domingos2016]. Symbolic AI manipulates symbols to apply logical operations to the declarative knowledge the symbols represent in order to deduce consequences of the knowledge [@Hoehndorf2017; @Nilsson1998]. For this reason, symbolic systems are often called rules-based or logic-based. These types of systems are considered to be highly explainable, since knowledge is commonly represented using first order logic rules, like if..then statements, which mimics human cognition [@Nilsson1998; @ilkou2020; @Hoehndorf2017]. The simplest form of AI, the rules-based system, is the predominant type of symbolic system. A rules-based system must be programmed to anticipate the situation-actions (in the form of rules) which lead from input to conclusion [@Jordan2015]. <!---Other examples of symbolic AI include [expert systems, inductive logic programming, and robotic process automation [@] ]--> The rigidity of rules-based systems and the prior knowledge required to define rules are major drawbacks among symbolic AI systems[@ilkou2020, @Hayes1985; @Nilsson1998]. 

##### Inductive Logic Programming

<!-- unsure of applications in ag -->

##### Robotic Process Automation

<!-- unsure of applications in ag -->

##### Expert Systems/Fuzzy Systems

Expert systems [definition]. Expert systems have been applied to machine vision derived images for weed and crop plant recognition in maize and barley [@Montalvo2013; @Romero2013]; crop row detection in maize [@Guerrero2013]. As a knowledge-based system, expert systems have the advantage of not requiring system training.

Much early AI work used symbolic systems but less focus has been placed on these systems since the rise of learning-systems in the [?1980s?]. However recently symbolic systems have been revisited in the context of integration with sub-symbolic systems in an attempt to ....

### Sub-symbolic AI

A system that can improve through experience or *learn* yields flexible lacking in a symbolic system [@Libbrecht2015; @Russsel2009; @Liakos2018]. Sub-symbolic AI also called connectionist AI are systems that can learn [@Nilsson1998; @ilkou2020].

#### Machine Learning

At the core of modern AI is machine learning (ML). ML exists as a broad subfield and is generally considered to include any method that makes predictions. Further subdivisions above or below ML in the AI systems architecture could be made perhaps distinguishing ML from other probabilistic prediction methods or subdividing sub-symbolic AI into statistical AI as the parent category of ML, but with the mixing and borrowing of methods from one classification to another, further subdivision may not accurately reflect the current state of the field. 

ML can be characterized by feedback type, data type <!--- discrete vs continuous --> ....

Machine learning can be considered to be supervised or unsupervised given the system's access to feedback. Supervised learning occurs in two phases, training and testing. During the training phase, predetermined input-response pairs (labeled data) are used as examples and the learning algorithm attempts to formulate function that connect input data to respective labels [@Liakos2018; @MontesinosLopez2022, p.29]. During the testing phase of supervised learning, the learned pattern (trained model) is used to generate label predictions and the accuracy of the predictions can be evaluated against user-defined labels. In this type of system the feedback is considered to be explicit. In unsupervised learning, the absence of preassigned labels for the input data only allows the model to evaluate patterns and prevents prediction accuracy from being evaluated since no correct input-response pairs have been specified. This type of system has no feedback. Systems that utilize both supervised and unsupervised learning are termed semi-supervised.

Machine learning methods can be further divided by data type. Within supervised learning, regression methods can be used for continuous data and classification methods can be used for categorical data. For unsupervised machine learning, the two common types include clustering and association for {data type 1} and {data type 2} respectively. 

Among the basic regression methods that are relevent for crop selection are two versions of best linear unbiased predictions (BLUPs). As a formulation of ridge regression, rrBLUP includes a design matrix of the SNPs as the relationship matrix for the mixed model [@MontesinosLopez2022]. In cases where the number of SNPs exceeds the number of genotypes, a genome-enabled BLUP (GBLUP) is preferable as in this formulation as relationships are assumed based on the genotypes of the marker profiles [@MontesinosLopez2022]. GBLUP and rrBLUP have been widely used for genomic selection [citations]


Machine learning exists at the intersection of computer science and statistics (Fig. {@fig:venndiagram}) and thus many statistical models are considered ML when applied with a prediction-centric approach. The field of statistics by comparison puts a greater focus on inference over prediction [@Bzdok2018], but methods shared by the two fields can generally accomplish both. For this reason

![Caption.](../Images/MLvsStats.svg){#fig:venndiagram width=75%}

##### Neural Networks

statistical/sub-symbolic systems

##### Natural Language Processing

##### Computer Vision

Computer vision attempts to derive meaning from images. A computer vision system "comprehends" the world generally in two stages: image acquisition and image processing [@Patricio2018; @Narendra2010]. Image acquisition systems are often mono-RGB vision systems, but systems may also include stereo vision, multi/hyperspectral cameras, Time of Flight cameras, and LIDAR technology, thermography and fluorescence imaging, and tomography imaging [@Perez-Sanz2017].

<!-- Image Acquisition -->

Image processing can be further divided into pre-processing operations, segmentation, feature extraction, and classification [@Perez-Sanz2017; @Jayas2008]. Image segmentation is important for background and object differentiation. <!-- In plant phenotyping, image segmentation is important for vegetation monitoring, estimation of LAI, plant nutritional status, fractional vegetation cover measurements, growth characteristics, weed detection and crop identification. (get cites from @Coy2016)--> The most popularly used segmentation algorithms in plant phenotyping include threshold [@Zhao2015; @Zhou2017; @Hartmann2011; @Ge2016], watershed [@Jerbi2015], and machine learning algorithms. Thresholding is a simple segmentation method and has been widely used.

During image processing, other AI algorithms like neural networks, fuzzy logic, and expert systems are often used to achieve computer vision.

In agricultural, computer vision has been widely applied to plant phenotyping and has made many HTP methods possible.

Image segmentation

Computer vision has been used for quality monitoring and measuring in cereal, fruit, and vegetable crops [@Jayas2008; @Kondo2010]; crop growth monitoring

Jayas et al. [-@Jayas2008] <!-- Review Article which summarizes work from students of Jayas--> describes computer vision being used to classify morphological, color, textural, features in wheat kernels using a four-layer back-propagation network and statistical classifier algorithm; insect infestation detection using a linear classifier and back-propagation neural network.

In the quest for automation,
- see [@Romeo2013]
  - visible spectral index based
  - threshold-based




### Sub-symbolic Systems

#####

# References
