Dimension reduction Cited from SNAPATAC2
=========================================================
Cited from https://kzhang.org/SnapATAC2/algorithms/dimension_reduction.html#spectral-embedding

[Fang_2021]: Fang, R., Preissl, S., Li, Y. et al. Comprehensive analysis of single cell ATAC-seq data with SnapATAC. Nat Commun 12, 1337 (2021). https://doi.org/10.1038/s41467-021-21583-9


Single-cell ATAC-seq (scATAC-seq) produces large and highly sparse cell by feature count matrix.
Working directly with such a large matrix is very inconvinent and computational intensive.
Therefore typically, we need to reduce the dimensionality of the count matrix before
any downstream analysis.

Different from most existing approaches, the dimension reduction method used in
SnapATAC2 is a pairwise-similarity based method, which requires defining and computing
similarity between each pair of cells in the data.
This method was first proposed in [Fang_2021], the version 1 of SnapATAC, and was called "diffusion map".
In SnapATAC2, we reformulate this approach as spectral embedding, *a.k.a.*, Laplacian eigenmaps.

Spectral embedding
------------------

Start with nxp cell by feature count matrix M, we first compute the
nxn pairwise similarity matrix S.

We then compute the normalized graph Laplacian

The eigenvectors correspond to the k+1-smallest eigenvalues of L are selected as
the lower dimensional embedding.

Nyström method
--------------

used the Nystrom method to perform a low-rank approximation of the full
similarity matrix.


Cell-type Assignment
=====================

Weighted K-nearest neighorbors


K-nearest neighorbors
---------------------
 what is KNN?

Weighted knn
-----------------
