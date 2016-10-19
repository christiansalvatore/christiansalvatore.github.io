---
layout: post
title: "Is this Alzheimer?"
description: "State of the art in the automatic diagnosis of AD"
date: 2016-10-15
tags: [automatic diagnosis, machine learning, artificial intelligence, alzheimer, mild cognitive impairment, public datasets]
comments: true
share: true
---

These tables are intended to be a summary of the state-of-the-art classification performance of AD using public datasets. Please, feel free to <a href="https://docs.google.com/forms/d/e/1FAIpQLSdN2wZIzWESc7N3zJJOQhXni-p9-NTeFaAG_1MJPa6PLd9W4g/viewform" target="_blank">fill in the form</a> if the list is not up-to-date or if any data is missing/wrong.

______________________________

## Cuingnet-509
This is a dataset of ADNI structural MRI images (T1-weighted @ 1.5T) of 509 patients, including 137 AD, 76 MCIc, 134 MCInc, 162 CN.
<br> The following binary comparisons are reported: **AD vs CN**, **MCIc vs CN**, **MCIc vs MCInc**.
<br> **Results** are given in terms of accuracy or balanced accuracy of classification. Sensitivity, specificity and AUC are also reported when provided. Results below chance (50%) are not reported.
<br> *Citing:*

```
Cuingnet, R. et al. (2011). Automatic classification of patients with Alzheimer's disease from structural MRI: a comparison of ten methods using the ADNI database. NeuroImage, 56(2), 766-781.
```

1\. AD vs CN

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
|0.88|Voxel-Direct-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.81|0.95|-|
|0.86|Voxel-Atlas-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.78|0.93|-|
|0.86|Voxel-Atlas-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.81|0.90|-|
|0.86|Voxel_COMPARE-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.82|0.89|-|
|0.85|Thickness-Atlas|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.79|0.90|-|
|0.84|Voxel-Atlas-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.75|0.93|-|
|0.84|Voxel-Atlas-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.74|0.93|-|
|0.83|Voxel-Direct-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.68|0.98|-|
|0.83|Voxel-Direct_VOI-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.71|0.95|-|
|0.83|Voxel-STAND-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.75|0.91|-|
|0.82|Thickness-Direct|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.74|0.90|-|
|0.82|Voxel-STAND-Sc-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.72|0.91|-|
|0.82|Thickness-ROI|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.69|0.94|-|
|0.82|Voxel-COMPARE-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.72|0.91|-|
|0.81|Voxel-STAND-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.71|0.91|-|
|0.81|Voxel-STAND-Sc-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.71|0.91|-|
|0.81|Voxel-Direct-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.72|0.89|-|
|0.81|Voxel-STAND-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.75|0.86|-|
|0.80|Voxel-Direct_VOI-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.65|0.95|-|
|0.80|Voxel-STAND-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.69|0.90|-|
|0.78|Voxel-Direct_VOI-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.65|0.91|-|
|0.77|Voxel-Direct-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.65|0.88|-|
|0.77|Hippo-Shape|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.69|0.84|-|
|0.76|Voxel-COMPARE-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.66|0.86|-|
|0.75|Voxel-COMPARE-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.69|0.81|-|
|0.74|Hippo-Volume-S|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.71|0.77|-|
|0.72|Hippo-Volume-F|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.63|0.80|-|
|0.70|Voxel-Direct_VOI-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.59|0.81|-|

2\. MCIc vs CN

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
|0.82|Voxel-Atlas-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.68|0.95|-|
|0.80|Thickness-ROI|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.65|0.94|-|
|0.79|Voxel-STAND-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.73|0.85|-|
|0.79|Voxel-STAND-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.65|0.93|-|
|0.77|Voxel-Direct-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.57|0.96|-|
|0.77|Voxel-Atlas-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.59|0.94|-|
|0.75|Thickness-Direct|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.54|0.96|-|
|0.75|Thickness-Atlas|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.57|0.93|-|
|0.75|Voxel-Direct_VOI-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.54|0.95|-|
|0.74|Voxel-STAND-Sc-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.62|0.85|-|
|0.74|Voxel-STAND-Sc-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.57|0.90|-|
|0.74|Hippo-Volume|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.73|0.74|-|
|0.73|Voxel-STAND-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.59|0.86|-|
|0.73|Voxel-Atlas-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.65|0.80|-|
|0.73|Voxel-Atlas-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.54|0.91|-|
|0.73|Hippo-Shape|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.57|0.88|-|
|0.72|Hippo-Volume|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.70|0.73|-|
|0.71|Voxel-STAND-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.49|0.93|-|
|0.70|Voxel-Direct-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.49|0.91|-|
|0.69|Voxel-Direct_VOI-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.41|0.96|-|
|0.69|Voxel-COMPARE-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.59|0.78|-|
|0.68|Voxel-COMPARE-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.51|0.85|-|
|0.68|Voxel-Direct-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.41|0.94|-|
|0.65|Voxel-COMPARE-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.49|0.81|-|
|0.64|Voxel-Direct-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.32|0.96|-|
|0.64|Voxel-COMPARE-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.49|0.78|-|
|0.61|Voxel-Direct_VOI-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.22|0.99|-|
|0.60|Voxel-Direct_VOI-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.32|0.88|-|

3\. MCIc vs MCInc

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
|0.68|Voxel-STAND-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.57|0.78|-|
|0.66|Voxel-COMPARE-D-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.54|0.78|-|
|0.66|Hippo-Volume-F|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.70|0.61|-|
|0.66|Hippo-Volume-S|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.62|0.69|-|
|0.65|Voxel-STAND-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.51|0.79|-|
|0.65|Voxel-COMPARE-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.62|0.67|-|
|0.62|Voxel-COMPARE-S-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.51|0.72|-|
|0.62|Thickness-Direct|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.32|0.91|-|
|0.57|Voxel-COMPARE-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.32|0.82|-|
|0.57|Voxel-Direct_VOI-D-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.43|0.70|-|
|0.57|Voxel-STAND-S-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.22|0.91|-|
|0.57|Voxel-STAND-Sc-all|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.41|0.72|-|
|0.56|Thickness-Atlas|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.27|0.85|-|
|0.53|Thickness-ROI|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.24|0.82|-|
|0.53|Voxel-STAND-Sc-gm|<a href="http://www.sciencedirect.com/science/article/pii/S1053811910008578" target="_blank">Neuroimage 2011</a>|0.35|0.70|-|

______________________________

## Moradi-825
This is a dataset of ADNI structural MRI images (T1-weighted @ 1.5T) of ????? patients, including ????? AD, ????? MCIc, ????? MCInc, ????? CN.
<br> The following binary comparisons are reported: **AD vs CN**, **MCIc vs CN**, **MCIc vs MCInc**.
<br> **Results** are given in terms of accuracy or balanced accuracy of classification. Sensitivity, specificity and AUC are also reported when provided. Results below chance (50%) are not reported.
<br> *Citing:*

```
Moradi, E. et al. (2015). Machine learning framework for early MRI-based Alzheimer's conversion prediction in MCI subjects. NeuroImage, 104, 398-412.
```


1\. AD vs CN

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="http://www.sciencedirect.com/science/article/pii/S1053811914008131" target="_blank">Neuroimage 2015</a>| | | |

______________________________

## Salvatore-509
This is a dataset of ADNI structural MRI images (T1-weighted @ 1.5T) of 509 patients, including 137 AD, 76 MCIc, 134 MCInc, 162 CN. These subjects are the same used in Cuingnet-509, but with the difference that in this case a nested 20-fold CV was used
<br> The following binary comparisons are reported: **AD vs CN**, **MCIc vs CN**, **MCIc vs MCInc**.
<br> **Results** are given in terms of accuracy or balanced accuracy of classification. Sensitivity, specificity and AUC are also reported when provided. Results below chance (50%) are not reported.
<br> *Citing:*

```
Salvatore, C. et al. (2015). Magnetic resonance imaging biomarkers for the early diagnosis of Alzheimer's disease: a machine learning approach. Frontiers in neuroscience, 9.
```

1\. AD vs CN

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="" target="_blank">PRL 2016</a>| | | |
|0.76|(PCA+FDR)+SVM|<a href="http://journal.frontiersin.org/article/10.3389/fnins.2015.00307/full" target="_blank">FRONT NEUROSCI 2015</a>|-|-|-|

2\. MCIc vs CN

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="" target="_blank">PRL 2016</a>| | | |
|0.72|(PCA+FDR)+SVM|<a href="http://journal.frontiersin.org/article/10.3389/fnins.2015.00307/full" target="_blank">FRONT NEUROSCI 2015</a>|-|-|-|

3\. MCIc vs MCInc

|Result   |Method   |Reference   |Sensitivity   |Specificity   |AUC   |
|:---|:---|:---|:---|:---|:---|
| | |<a href="" target="_blank">PRL 2016</a>| | | |
|0.66|(PCA+FDR)+SVM|<a href="http://journal.frontiersin.org/article/10.3389/fnins.2015.00307/full" target="_blank">FRONT NEUROSCI 2015</a>|-|-|-|

______________________________

## CADDementia dataset
Up-to-date results are collected in this <a href="https://grand-challenge.org/site/caddementia/results_all/" target="_blank">external webpage</a>.
