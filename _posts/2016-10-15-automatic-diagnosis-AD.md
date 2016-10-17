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

Surprisingly, if you go through all these papers, you will note a strange distribution in classificatio performance: there will obviously be no published papers with very poor performance (under chance); there will be some papers with conceivably-average performance; but you will also find a lot of published papers with incredibly excellent performance, including perfect or quasi-perfect classifiers!
Let's take, for example, the basic -yet *nontrivial*- diagnosis of AD. In this case, the classifier is asked to discriminate between subject with AD and Cognitively Normal (CN) subjects (AD vs CN). 
PERFOMANCE AD
PERFORMANCE MCIcMCInc

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

##### Cuingnet-509


##### Moradi-825


##### Salvatore-509


##### CADDementia dataset
Up-to-date results are collected in this <a href="https://grand-challenge.org/site/caddementia/results_all/" target="_blank">external webpage</a>.
