# INTRODUCTION

scRNA-seq (Single-cell RNA sequencing) is a groundbreaking tool enabling researchers to delve deep into the transcriptomic profile of singular cells. This helps us derive putative cell types based on specific marker genes present within the data. 

The primary objective of the study revolved around deciphering the physical environment inhabited by type 2 lymphocytes.

# QUALITY CONTROL

To ensure data reliability, we excluded cells presenting:

Read counts below 200.
Read counts exceeding 2000.
Mitochondrial RNA proportions above 5%.

#ANALYSIS

To interpret the dataset, Principal Component Analysis (PCA) was executed. Remarkably, the three genes displaying the highest variability along the principal component were associated with Surfactant, Pulmonary-Associated Protein—typically linked to lung's epithelial cells.

Two distinct clustering approaches were tested: The first utilized 12 Principal Components (PCs), chosen based on visual evaluation of the elbow plot, while the second incorporated 22 PCs, as this number accounted for 75% of the variance. Upon comparing the two methodologies, the 22 PCs approach didn't present any additional subclusters of significance compared to the 12 PCs technique. Hence, the clustering derived from 12 PCs was retained to identify marker genes.

# RESULTS

Our analysis led to the identification of the following cell types:

Epithelial cells.
Mesenchymal cells.
Alveolar endothelial cells.
Mesothelial cells.
General endothelial cells.
Myocardial cells (These are suspected to be contaminants within the sample).
