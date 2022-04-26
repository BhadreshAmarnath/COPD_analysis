# COPD Patient Segmentation Challenge

## By Leonard Karsunky

### April 25, 2022

The aim of this analysis is to cluster/segment COPD patients into distinct subpopulations using unsupervised learning techniques. The dataset includes 101 (imaginary) patients and 22 features (both numerical and categorical), including information on their characteristics, disease severity, and co-morbidities. Other features include measures of patients' walking ability, quality of life, anxiety and depression.

# Findings

In this small analysis, we used several unsupervised learning algorithms utilizing various distance metrics (Euclidian and non-Euclidian) to cluster patients with chronic obstructive pulmonary disease (COPD) that includes 22 features with both categorical and numerical features, including K-Means, K-Prototype and Factor Analysis of Mixed Data.

While most of the analysis can be seen throughout the notebook, most of the clustering efforts did not yield very promising results as we are sometimes used to seeing (except for FAMD which is biased due to the single categorical feature). These techniques are also very sensitive to initialization and require clusters to have convex shapes. Our low-dimensional embedding is also not creating any "nice" visual separations of our data into distinct clusters. However, most of the labels/clusters were well colored, i.e. with no overlap and clear region delineations, proving that some successful clustering of patients was achieved.

Of course, there is still a lot of analysis to be done on this dataset including data preprocessing/cleaning, as well as deeply analyzing the quality of the clustering (cardinality, magnitude), looking into more similiarity metrics and further optimizing the number of clusters. Indeed, instead of using a fixed number of predetermined clusters, we can also use hierarchical clustering methods using the Gower similarity metric, for instance.
