# Assignment 2 - Gene Expression Analysis and Interpretation
## Author: Martha Rotter
In this assignment, students analyse a publicly available breast cancer dataset by downloading and preprocessing the TCGA RNA-seq data for breast cancer from cBioPortal database, and identify differentially expressed genes between ERBB2+ and other breast cancer tumours. The dataset is located at https://www.cbioportal.org/study/summary?id=brca_tcga_pan_can_atlas_2018

## Code explanation
### 0. Setup and preprocessing
Load all required libraries, set working directory

### 1. Import data
Read in various data files and assign them to local variables for processing

### 2. Match patient IDs and remove extra data
Find the patient IDs in the CNA data file & RNA seq file. Remove extra lines and values not in both.

### 3. Create metadata using the CNA level of ERBB2+
Create a metadata instance which matches the CNA levels of ERBB2+ with the patient IDs and their amplified levels.

### 4. Normalize data using DESeq2
Run the DESeq function from the DESeq2 library

### 5. Obtain differently expressed genes
Sort the genes by their PADJ value to find the top ten differently expressed genes

### 6. Perform a pathway enrichment analysis
Use the KEGG enrichment functions to run a pathway enrichment and plot the results

### 7. Get the variance stabilised transformed expression values
Use the vst function to get the VST values

### 8. With the VST values obtain a PCA plot and a heatmap
Use the VST values to create a PCA plot and generate a heatmap

### 9. With the VST values of the DE genes, generate an overall survival model using the glmnet package
Finally use the glmnet package to generate a survival model.


 ###### Repository:
- -[x] **ERBB2_gene_expression_analysis.R

 ###### Dependencies
This implementation requires 
* R 4.4.2 or greater
* BiocManager
* glmnet

 ###### License
 - MIT
