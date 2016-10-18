---
layout: post
title: "Automatic diagnosis of Alzheimer's Disease - where are we?"
description: ""
date: 2016-10-15
tags: [automatic diagnosis, machine learning, artificial intelligence, alzheimer, mild cognitive impairment]
comments: true
share: true
---

During my three years of doctoral project, which ended in December 2015, I studied -among other topics- the implementation of an intelligent system able to automatically classify patients with Alzheimer's Disease (AD).

As you all know, AD is the most common neurodegenerative disease, affecting millions of people worldwide. Although this condition has been known for more than a hundred years, there is still no definite diagnosis. More difficult than this, diagnosing Mild Cognitive Impairment (MCI) -which can be simply described as a pre-clinical and pre-symptomatic condition that may (MCIc) or may not (MCInc) convert to AD- is one of the biggest challenges in medicine.

>Predicting the conversion of MCI to AD is one of the biggest challenges

These considerations alone are able to explain the great race of the last few years for the implementation of machine learning algorithms able to automatically diagnosing AD and/or predicting the conversion of MCI.

### The great race for machine learning in AD
In the last few years, there has been a great race for the implementation of automatic algorithms for AD diagnosis. More explanatory than words, if you type the keywords "machine learning" and "alzheimer" in the *search* form of [scopus](https://www.scopus.com/), you will obtain this plot (search fields: article title, abstract, keywords; date: October 2016).


<img src="https://raw.githubusercontent.com/christiansalvatore/christiansalvatore.github.io/master/images/automatic-diagnosis-AD-figure-1.jpg" style="width: 600px;"/>


But what is the modality used as input to the classification algorithms?

Just to give a rough estimate, of 368 retrieved papers, the majority (98) contains the keyword *MRI* (Magnetic Resonance Imaging). Then we go from *biological* (69), to *PET* (Positron Emission Tomography, 40), *neuropsych-* (neuropsychological test scores, 33), *amyloid* (28), down to *CT* (computerized tomography, 4).

As expected, MRI -in particular structural MRI- is the most used modality when we deal with neurological disorders. This is probably because it represents a good compromise between *sensitivity* (to brain changes due to the disease) and *non-invasiveness*. For example, PET is more sensitive to functional brain alterations even preceeding structural changes, but its invasiveness is a big negative point.

>Structural MRI is the most used modality for the automatic classification of AD

The second question may be *which feature-extraction/classification method is the most used?* - but we will not go through this topic in this post. We would rather want to know what is the classification performance of these methods, that is, of the methods published in these (almost) 400 papers. This should answer to the most general question that is the title of this post - *Automatic classification of AD: where are we?*

Surprisingly, if you go through all these papers, you will note a strange distribution in classification performance: there will obviously be no published papers with very poor performance (under chance); there will be some papers with conceivably-average performance; but you will also find a lot of published papers with incredibly excellent performance, including perfect or quasi-perfect classifiers!

Let's take, for example, the basic -yet *nontrivial*- diagnosis of AD. In this case, the classifier is asked to discriminate between patients with AD and Cognitively Normal (CN) subjects (AD vs CN). If you have a look at the papers, you will discover that the major part of the published algorithms is able to obtain classification performance (accuracy/number of correct predictions over the whole test dataset) beyond 85%, some reaching 100% classification accuracy.

So, how is this possible? We are not able to <a href="https://rodrigob.github.io/are_we_there_yet/build/classification_datasets_results.html#4d4e495354" target="_blank">classify handwritten digits</a> with 100% accuracy, but we can say if a patient has AD with no errors?
Well, may this be due to the fact that AD and CN are easily-separable groups - given the deeply different characteristics of a normal brain (we are talking about structural MRI here) with respect to the brain of a patient with AD?

Let's have a look at a much more complicated task, then: the prediction of conversion of MCI to AD. In this case, the classifier is asked to discriminate between patients with MCI who will convert to AD and patients with MCI who will not convert to AD (MCIc vs MCInc). Obviously, as we don't know how to figure out if a patient will or will not convert to AD, the final diagnosis is obtained by following patients up for a given period of time (say, 18/36 months) and by using the diagnosis at that time (AD or still MCI) as final gold standard to evaluate the predictive power of our classification algorithm. In this way, baseline (time zero) data are used for training/validation/testing of the classifier, while follow-up labels are used as gold standard for evaluating classification performance.

Again, if you have a look at these papers, you will discover that classification of MCIc vs MCInc can easily go beyond 70%, which is an excellent result for such a huge problem, still reaching nearly 100% accuracy in some cases.

Ok, so probably the diagnosis and prediction of conversion to AD is not a big problem. We got it? Not exactly.

* Cuingnet et al., 2011

* The CADDementia grand challenge (2015)

### Publicly available datasets
<a href="http://adni.loni.usc.edu/" target="_blank">ADNI</a> and <a href="http://www.oasis-brains.org/" target="_blank">OASIS</a> are two popular choices.

### A few other examples...



* Moradi et al., 2014

* Salvatore et al., 2015



______________________________________________

### Classification performance: state of the art
These tables are intended to be a summary of the state-of-the-art classification performance of AD using public datasets. Please, feel free to <a href="https://docs.google.com/forms/d/e/1FAIpQLSdN2wZIzWESc7N3zJJOQhXni-p9-NTeFaAG_1MJPa6PLd9W4g/viewform" target="_blank">fill in the form</a> if the list is not up-to-date or if any data is missing/wrong.

#### Cuingnet-509


#### Moradi-825


#### Salvatore-509

1. AD vs CN

|Result   |Method   |Venue   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="" target="_blank">PRL 2016</a>| | | |
|0.76|(PCA+FDR)+SVM|<a href="http://journal.frontiersin.org/article/10.3389/fnins.2015.00307/full" target="_blank">FRONT NEUROSCI 2015</a>|-|-|-|

2. MCIc vs CN

|Result   |Method   |Venue   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="" target="_blank">PRL 2016</a>| | | |
|0.72|(PCA+FDR)+SVM|<a href="http://journal.frontiersin.org/article/10.3389/fnins.2015.00307/full" target="_blank">FRONT NEUROSCI 2015</a>|-|-|-|

3. MCIc vs MCInc

|Result   |Method   |Venue   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="" target="_blank">PRL 2016</a>| | | |
|0.66|(PCA+FDR)+SVM|<a href="http://journal.frontiersin.org/article/10.3389/fnins.2015.00307/full" target="_blank">FRONT NEUROSCI 2015</a>|-|-|-|



#### CADDementia dataset
Up-to-date results are collected in this <a href="https://grand-challenge.org/site/caddementia/results_all/" target="_blank">external webpage</a>.
