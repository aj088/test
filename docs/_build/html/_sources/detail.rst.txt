Pipeline Overview
===================
For more details, please see out following publication:

http://


Original Input
------------------

The following files are needed to run *Celltype Annotation* on your own experiment:

- *fragments.tsv.gz* files with fragments for each scATAC sample
- *fragments.tsv.gz.tbi* files with fragments index information for each scATAC sample
- *cell barcodes* files with high quality cells for each scATAC sample

- Optionally: *UMAP* or *tSNE* projection file from each sample

Currently, this package only supports hg38 reference mapping


Intermediate Output
--------------------

The following files are intermediate outputs of *Celltype Annotation* using FeatureMatrix function in Seurat:

- *matrix.mtx* Sparse matrix files with fragment reads
- *peaks.tsv* Cell-type restricted peaks
- *cell.tsv* High quality cells, the same cells as input

Final Output
--------------------
The following files are final outputs of *Celltype Annotation* using the annotation tool:

- *merged.h5ad* anndata of integrated query and reference cells 
- *prediction.tsv* Cell-type prediction of query cells
- *uncertainty_score.tsv* Uncertainty score of cel-type prediction
