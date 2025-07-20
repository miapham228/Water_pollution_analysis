# Water_pollution_analysis in the Shuangji River

## Introduction
This study explored different multivariate statistical techniques to determine the potential sources of water pollution, analyse the similarity or dissimilarity between 14 sites and identify the factors that cause the spatial changes of river water quality. 

## Research Questions

This research aims to provide some empirical evidence on the effectiveness of using multivariate statistical techniques. The major research questions I investigate are:

-   Is Principal Component Analysis able to identify the important factors that affect water quality?

-   Are Clustering Analysis and Discriminant Analysis able to identify the most crucial parameters that cause the spatial change of the river water quality?

## Data Source

The data set which contains 19 physical and chemical parameters were monitored by sampling at 14 different sites in 2 years 2019-2020 along the Shuangji river. The 19 physical and chemical parameters included pH, dissolved oxygen (DO), chemical oxygen demand (COD), ammonia-nitrogen (NH3-N), total phosphorus (TP), chemical oxygen demand (CODMn), fluoride (F), petroleum hydrocarbons (Oil), linear alkylbenzene sulfonates (LAS), copper (Cu), zinc (Zn), cadmium (Cd), arsenic (As), mercury (Hg), hexavalent chromium (Cr6+), total cyanides (CN), volatile phenols (VP), sulphide (S) and selenium (Se) (Liu et al.,2021).

Among 14 sites, sites T1, T2, T3, T4, T5 and T6 are the main tributaries entering the Shuangji River while sites M1, M2, M3, M4, M5, M6, M7 and M8 are the key points on the main bank of the Shuangji River, and site M8 is under municipal control and provides the exit water of Xinmi County. Specifically, sites M1-M3 and T1-T3 are closer to the urban area, and the main source of pollution is urban sewage entering the river. Sites M4, M5, T4 and T5 are located in the industrial zone where the paper industry in their vicinity is relatively developed. Sites M6-M8 are downstream of the river and have no inflow of external water (Liu et al.,2021).

## Research Methodology

### Principal Component Analysis

PCA can be used as a technique to reduce dimension while retaining most of the information in data. Through its coefficients, we are hopefully able to identify the important parameters that explain the most variation in data as well as capture the structure of data. Taking into account the differences in the magnitude and measurement units, all parameters were standardized to ensure that each feature contributes equally to the analysis.

### Clustering Analysis

Cluster analysis is a multivariate statistical method that explores the naturally occurring groups within a data set according to their distance. To classify sites into clusters, various clustering methods were applied to a normalized aggregate data set. These methods included Hierarchical clustering analysis with complete linkage, K-Means clustering, and K-Medoids clustering, all using Euclidean distance as the measure of similarity. Based on the data description, which identifies three main areas (urban areas, industrial zones, and downstream of the river), three clusters were formed. 

### Linear Discriminant Analysis

Discriminant Analysis is a statistical method for analyzing the difference between two or more naturally occurring groups. By examining the correlations between the discriminant functions and the original variables, this method highlights the variables that contribute the most to the differences across groups. To explore the causes of spatial changes, the discriminant analysis of the original data was run to construct discriminant functions to evaluate the spatial changes in river water quality. The clusters from Clustering Analysis are group-dependent variables, and all measurement parameters are independent variables. 

## Key Findings

The parameters which have the greatest contributions to changes in river water quality were *COD*, *TP*, *DO*, *F*, *LAS*, *Cu* and *VP* . The results from PCA and rotated PCA indicates that these parameters can be mainly divided into natural (such as *PH*, *DO*, *NH3-N*, *TP*) and anthropogenic pollution components (such as *COD*, *CODMn*, *LAS*, *Cu*,...). This distinction is crucial for developing targeted strategies to manage and improve water quality.

Cluster analysis divided 14 sampling points into three clusters according to the similarity of river water quality and pollution characteristics. The LDA results indicated that *TP*, *COD*, *CODMn*, *Oil*, *S*, *F*, *Cu*,*CN* were the most important variables in differentiating three areas, achieving a 93% accuracy rate.
