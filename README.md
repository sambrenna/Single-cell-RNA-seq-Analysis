# INTRODUCTION

scRNA-seq (Single-cell RNA sequencing) is a groundbreaking tool enabling researchers to delve deep into the transcriptomic profile of singular cells. This helps us derive putative cell types based on specific marker genes present within the data. 
The datased we utilised is derived from: 
Oetjen KA, Lindblad KE, Goswami M, Gui G, Dagur PK, Lai C, Dillon LW, McCoy JP, Hourigan CS. Human bone marrow assessment by single-cell RNA sequencing, mass cytometry, and flow cytometry. JCI Insight. 2018 Dec 6;3(23):e124928. doi: 10.1172/jci.insight.124928. PMID: 30518681; PMCID: PMC6328018.

The primary objective of the study revolved around deciphering the physical environment inhabited by bone marrow.

# QUALITY CONTROL

To ensure data reliability, we excluded cells presenting:

Read counts below 200.
Read counts exceeding 2000.
Mitochondrial RNA proportions above 5%.

#ANALYSIS

To interpret the dataset, Principal Component Analysis (PCA) was executed.

Two distinct clustering approaches were tested: The first utilized 12 Principal Components (PCs), chosen based on visual evaluation of the elbow plot, while the second incorporated 22 PCs, as this number accounted for 75% of the variance. Upon comparing the two methodologies, the 22 PCs approach didn't present any additional subclusters of significance compared to the 12 PCs technique. Hence, the clustering derived from 12 PCs was retained to identify marker genes.

# RESULTS

Our analysis led to the identification of the following cell types:
CD4+ naïve T cells
CD4+ memory T cells
B cells
Plasma cells
CD14+ monocytes
Monocytes (if distinct from CD14+ monocytes)
Natural killer cells
Erythroid-like cells
Dendritic cells
Plasmacytoid dendritic cells

