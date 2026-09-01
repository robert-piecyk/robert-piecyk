## Robert Piecyk

Postdoctoral researcher at LMU University Hospital, Munich, in the Department of
Radiotherapy and Radiation Oncology (he/him). Affiliated with BZKF and DKTK Munich.

Computational biology and bioinformatics, grounded in statistics and deep learning, with
an emphasis on developing and implementing the analysis tools a study needs. Currently
working in translational oncology, including multi-omics analyses, computational
pathology, and medical imaging. My PhD was in epigenomics, which remains a research
interest: DNA methylation, Hi-C, and the integration of both with expression data. It
produced tools for calling and benchmarking differentially methylated regions in WGBS
data.

### Skills

| | |
|:---|:---|
| **Languages** | Python, R, Bash |
| **Machine learning** | PyTorch, Lightning, Hugging Face, timm, XGBoost, scikit-learn, glmnet. Deep learning on images and genomic sequence, survival analysis, hidden Markov models |
| **Omics** | Bulk, single-cell and spatial transcriptomics (Seurat, Signac, Scanpy); differential expression and batch correction (DESeq2, limma, edgeR, sva); deconvolution (CIBERSORTx, EcoTyper) |
| **Epigenomics** | CUT&RUN, ChIP-seq, ATAC-seq and Hi-C; peak annotation, differential binding and enrichment (ChIPseeker, DiffBind, LOLA); motif analysis (TFBSTools, JASPAR); DNA methylation from arrays and WGBS (minfi, ChAMP, RnBeads, METHimpute) with reference-free and reference-based deconvolution (EpiDISH, latent methylation components) |
| **Imaging** | Whole-slide imaging (OpenSlide, QuPath, HistomicsTK) and pathology foundation models; DICOM, NIfTI, NRRD; SimpleITK, scikit-image, OpenCV |
| **Engineering** | pytest, ruff, GitHub Actions; SLURM and HPC; Docker, Singularity; Zarr, HDF5, Parquet; Git |

### Software

| Project | Description | Language |
|:---|:---|:---|
| [voxelmetry](https://github.com/robert-piecyk/voxelmetry) | Morphometry and 3-D visualisation for CT and MR segmentations. Reads DICOM series, DICOM SEG, NIfTI and NRRD, and reports volume, Feret diameter, surface area and sphericity in physical units. Voxel spacing is carried through resampling and cropping. Output is a self-contained HTML viewer. Validated against analytic phantoms and cross-checked against SimpleITK. | Python |
| [jDMR](https://github.com/robert-piecyk/jDMR) | Heuristic caller for differentially methylated regions in large-scale WGBS data. Methylation states are called with a hidden Markov model over either cytosine clusters or sliding genomic windows; samples are then merged and non-polymorphic patterns filtered. Designed for population-level studies and control/treatment designs. | R |
| DMRspiker *(not yet public)* | Semi-synthetic benchmark generator for WGBS. Injects ground-truth DMRs into a real wild-type methylome, preserving its empirical coverage and cytosine-density structure. Supports both focal regulatory and broad chromatin-domain DMRs. Hyperparameters are derived from the source methylomes. Used to tune and benchmark DMR callers. | R |
