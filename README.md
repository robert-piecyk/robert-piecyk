## Robert Piecyk

Postdoctoral researcher at LMU University Hospital, Munich, in the Department of
Radiotherapy and Radiation Oncology.

Computational biology and bioinformatics, grounded in statistics and deep learning, with
an emphasis on developing and implementing the analysis tools a study needs. Currently
working in translational oncology on multi-omics analyses, computational pathology and
medical imaging, coupled with clinical association. My main focus is building end-to-end
pipelines and integrating epigenetic layers with other omics and clinical data.

My PhD was in epigenomics and it remains a research interest: DNA methylation, Hi-C, and
how both relate to expression. That work produced the tools for calling and benchmarking
differentially methylated regions listed below.

### Skills

| | |
|:---|:---|
| **Languages** | Python, R, Bash |
| **Machine learning** | PyTorch, Lightning, Hugging Face, timm, XGBoost, scikit-learn. Deep learning on images and genomic sequence, gradient boosting, survival analysis, hidden Markov and mixture models |
| **Omics** | Bulk, single-cell and spatial transcriptomics; differential expression and batch correction; cell-type deconvolution; multi-omics integration |
| **Epigenomics** | CUT&RUN, ChIP-seq, ATAC-seq and Hi-C; peak calling, annotation and differential binding; motif and region enrichment; DNA methylation from arrays and WGBS; methylome deconvolution |
| **Imaging** | Whole-slide imaging and pathology foundation models; tiling, segmentation and feature extraction; 3-D medical imaging (DICOM, NIfTI, NRRD) and morphometry |
| **Engineering** | Packaging, testing and CI; SLURM and HPC; Docker and Singularity; reproducible pipelines; Git |

### Software

| Project | Description | Language |
|:---|:---|:---|
| [voxelmetry](https://github.com/robert-piecyk/voxelmetry) | Morphometry and 3-D visualisation for CT and MR segmentations. Reads DICOM series, DICOM SEG, NIfTI and NRRD, and reports volume, Feret diameter, surface area and sphericity in physical units. Voxel spacing is carried through resampling and cropping. Output is a self-contained HTML viewer. Validated against analytic phantoms and cross-checked against SimpleITK. | Python |
| [jDMR](https://github.com/robert-piecyk/jDMR) | Heuristic caller for differentially methylated regions in large-scale WGBS data. Methylation states are called with a hidden Markov model over either cytosine clusters or sliding genomic windows; samples are then merged and non-polymorphic patterns filtered. Designed for population-level studies and control/treatment designs. | R |
| DMRspiker *(not yet public)* | Semi-synthetic benchmark generator for WGBS. Injects ground-truth DMRs into a real wild-type methylome, preserving its empirical coverage and cytosine-density structure. Supports both focal regulatory and broad chromatin-domain DMRs. Hyperparameters are derived from the source methylomes. Used to tune and benchmark DMR callers. | R |
