# Assignment 2 - Gene Expression Analysis and Interpretation
## Author: Martha Rotter
In this assignment, students analyse a publicly available breast cancer dataset by downloading and preprocessing the TCGA RNA-seq data for breast cancer from cBioPortal database, and identify differentially expressed genes between ERBB2+ and other breast cancer tumours. The dataset is located at https://www.cbioportal.org/study/summary?id=brca_tcga_pan_can_atlas_2018

## Code explanation
### 0. Setup and preprocessing


### 1. Import data


### 2. Match patient IDs and remove extra data


### 3. Create metadata using the CNA level of ERBB2+


### 4. Normalize data using DESeq2


### 5. Obtain differently expressed genes


### 6. Perform a pathway enrichment analysis


### 7. Get the variance stabilised transformed expression values


### 8. With the VST values obtain a PCA plot and a heatmap


### 9. With the VST values of the DE genes, generate an overall survival model using the glmnet package

 ###### Repository:
- -[x] **ERBB2_gene_expression_analysis.R

 ###### Dependencies
This implementation requires R 4.4.2 or greater
BiocManager
glmnet

 ###### License
 - MIT
