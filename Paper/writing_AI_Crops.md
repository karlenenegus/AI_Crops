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


Modern crop improvement has the advantage and challenge of access to large genomic, phenomic and enviromic data sets<!--- genomic, phenomic and enviromic should have been defined in earlier section --> to inform breeding and selection decisions. A single population can now produce dramatically more data then was cumulatively obtained in the breeding process in previous decades. The prior issues of genotyping and phenotyping bottlenecks have been largely overcome with higher levels of automation achieved through approaches like post-NGS sequencing technologies <!--- more specific -->, HTP, and remote sensing <!--- These should have been mentioned previously -->. However, these solutions and the accompanying "big data" also lend new issues to the field of crop improvement. Fully exploiting "-omic" data in an efficient manor is difficult with prior approaches<!--like...-->. There is now a need for new methods of analysis which effective and efficient in order to continue bridging the gap between observed genotypes and observed phenotypes. AI has the potential to provide diverse solutions to these ends.

# AI

Artificial intelligence (AI) is concerned with the process of designing computers that can think and act humanly and rationally [@Russsel2009]. In recent years, AI has been increasingly explored as a means to analyze big data most popularly through machine learning (ML) approaches. However in addition to ML, AI encompasses a number of diverse sub-fields which can can be generally categorized as symbolic or sub-symbolic [@Nilsson1998; @ilkou2020]. Symbolic AI can be called knowledge-based because it applies logical operations to declarative knowledge in order to deduce consequences of the knowledge [@Nilsson1998].
Knowledge in a symbolic system is commonly represented using first order logic rules which mimics human reasoning making these types of systems highly explainable [@Nilsson1998; @ilkou2020]. The simplest form of AI, the rules-based system, is the predominant type of symbolic system. The rigidity of a rules-based system and the prior knowledge required to define the rules are major drawbacks of symbolic AI [@ilkou2020, @Hayes1985; @Nilsson1998]. Programming a system that can anticipate all situation-actions which lead from input to conclusion is more difficult than training a system that can learn from input [@Jordan2015]. Sub-symbolic systems are systems that can learn [@Nilsson1998; @ilkou2020]

At the core of modern AI is machine learning (ML). Machine learning is a subfield within AI which attempts *learning* or improvement through experience [@Libbrecht2015; @Russsel2009; @Liakos2018]. ML can be characterized by feedback type, data type <!--- discrete vs continuous --> ....

Machine learning can be considered to be supervised or unsupervised given the system's access to feedback. Supervised learning occurs in two phases, training and testing. During the training phase, predetermined input-response pairs (labeled data) are used as examples and the learning algorithm attempts to formulate function that connect input data to respective labels [@Liakos2018; @MontesinosLopez2022, p.29]. During the testing phase of supervised learning, the learned pattern (trained model) is used to generate label predictions and the accuracy of the predictions can be evaluated against user-defined labels. In this type of system the feedback is considered to be explicit. In unsupervised learning, the absence of preassigned labels for the input data only allows the model to evaluate patterns and prevents prediction accuracy from being evaluated since no correct input-response pairs have been specified. This type of system has no feedback. Systems that utilize both supervised and unsupervised learning are termed semi-supervised.

Machine learning models can also be divided by learning type. Within supervised learning

Machine learning exists at the intersection of computer science and statistics (Fig. {@fig:venndiagram}) and thus many statistical models are considered ML when applied with a prediction-centric approach. The field of statistics by comparison puts a greater focus on inference over prediction [@Bzdok2018], but methods shared by the two fields can generally accomplish both. For this reason

![Caption.](../Images/MLvsStats.svg){#fig:venndiagram width=75%}

## AI in Crop Improvements

<!--a) yield results that are meaningful biologically (interpretable), b) feasible computationally (efficient), c) have high fidelity to plants represented (accuracy), d) achieves improvement (predictive/useful). -->

<!--- Logic Based & Knowledge Based Systems: *Automation* -->

Inductive Logic Programming



Robotic Process Automation

Expert Systems/Fuzzy Systems

# References
