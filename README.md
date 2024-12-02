Microbial Network Analysis Using SPIEC-EASI

This repository contains code to construct microbial networks using SPIEC-EASI (SParse InversE Covariance Estimation for Ecological Association Inference). 
The methodology ensures parsimony and robustness by avoiding detection of spurious correlations between OTUs (Operational Taxonomic Units). 
It employs centered log-ratio (CLR) transformations and the Meinshausen-Bühlmann (MB) method to infer ecological associations.

Features

Data preparation: Import, clean, and organize OTU, taxonomy, sample, and environmental data.
Network construction: Create microbial networks for specific sample groups using SPIEC-EASI with MB.
Network analysis: Compute modularity, topological attributes, and edge/node comparisons.
Visualization: Venn diagrams, heatmaps, and robustness metrics for ecological insights.
Output: Export node and edge tables for further exploration.

Prerequisites

Software
R (>= 4.0): Ensure R is installed on your system.
R Libraries:
SpiecEasi
microtable
pheatmap
ggsave
openxlsx
Additional dependencies: dplyr, magrittr, igraph
Data Files
The following files must be in the working directory:

otu_DNA.txt: OTU abundance data.
taxonomy_table.txt: Taxonomy mapping.
sample_table_DNA.txt: Metadata for samples.
env_DNA.txt: Environmental metadata.

Install the required R packages:
install.packages(c("SpiecEasi", "microtable", "pheatmap", "ggplot2", "openxlsx", "dplyr", "magrittr", "igraph"))

Contribution
Contributions are welcome! Please submit issues or pull requests to help improve the project.

References
Kurtz, Z. D., et al. (2015). "Sparse and compositionally robust inference of microbial ecological networks." PLoS Computational Biology.
Meinshausen, N., & Bühlmann, P. (2006). "High-dimensional graphs and variable selection with the Lasso." Annals of Statistics.
Liu, H., et al. (2010). "Stability approach to regularization selection." Journal of the Royal Statistical Society.
