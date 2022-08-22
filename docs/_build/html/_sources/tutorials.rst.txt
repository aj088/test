Tutorials
===================

Case Study Datasets
----------------------

Four case studies below gives you a taste of different capabilities of our Annotation workflow. The data sets you will be exploring are:

1) PBMC 5K cells from 10X

   Data can be directly downloaded from 10X webpage:

2) scATAC of Renal Cell Carcinoma

   Citation: Wang, Qi et al. “Single-cell chromatin accessibility landscape in kidney identifies additional cell-of-origin in heterogenous papillary renal cell carcinoma.” Nature communications (2022)

   This paper published scATAC profiles from two samples, generating a total of 9428 kidney cells colored by clustering.

   .. figure:: Study1.png
      :scale: 60 %
      :alt: UMAP of kidney cells
      :align: center

3) scATAC of Basal cell cancer tumor microenvironment

   Citation: Satpathy, Ansuman T et al. “Massively parallel single-cell chromatin landscapes of human immune cell development and intratumoral T cell exhaustion.” Nature biotechnology (2019)

   This paper published 37,818 scATAC-seq profiles of BCC TME cell types

   .. figure:: Study2.png
      :scale: 60 %
      :alt: UMAP of BCC cells
      :align: center


PBMC 5K
------------------
Step1: Perform Integration of human reference atlas and PBMC 5K

   .. figure:: PBMC5K_step1.png
      :scale: 40 %
      :align: center

   .. figure:: PBMC5K_step2.png
      :scale: 40 %
      :align: center

Step2: Assign celltypes to query cells based on first 30 spectral embeddings

   .. figure:: PBMC5K_step3.png
      :scale: 40 %
      :align: center
