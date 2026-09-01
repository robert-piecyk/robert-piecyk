## Robert S. Piecyk

Postdoctoral researcher at LMU University Hospital, Munich, in the Department of
Radiotherapy and Radiation Oncology (he/him). Affiliated with BZKF and DKTK Munich.

Computational biology and bioinformatics, with an emphasis on developing and
implementing the analysis tools a study needs. Currently working in translational
oncology, including multi-omics analyses, computational pathology, and medical imaging.
My PhD was in epigenomics, which remains a research interest: DNA methylation, Hi-C,
and the integration of both with expression data. It produced tools for calling and
benchmarking differentially methylated regions in WGBS data. First- and co-authored work
published in Nature, PNAS and Nature Communications.

[Website](https://robert-piecyk.github.io) ·
[Google Scholar](https://scholar.google.com/citations?user=v8gjQjUAAAAJ) ·
[ORCID](https://orcid.org/0009-0002-1912-4487) ·
[LinkedIn](https://www.linkedin.com/in/robert-piecyk)

### Skills

| | |
|:---|:---|
| **Languages** | Python, R, Bash |
| **Machine learning** | PyTorch, Lightning, Hugging Face Transformers, timm, XGBoost, scikit-learn. Deep learning on images and genomic sequence, gradient boosting, hidden Markov models, survival analysis, mixture models |
| **Omics** | Bulk, single-cell and spatial transcriptomics (Scanpy, AnnData, Seurat); cell-type deconvolution (CIBERSORTx, EcoTyper); WGBS methylation; Hi-C |
| **Imaging** | Whole-slide images (OpenSlide, pathology foundation models); DICOM, DICOM SEG, NIfTI, NRRD; SimpleITK, scikit-image, OpenCV |
| **Engineering** | Packaging, testing and CI (pytest, ruff, GitHub Actions); SLURM and HPC; Singularity; Git; reproducible pipelines |

### Software

| Project | Description | Language |
|:---|:---|:---|
| [voxelmetry](https://github.com/robert-piecyk/voxelmetry) | Morphometry and 3-D visualisation for CT and MR segmentations. Reads DICOM series, DICOM SEG, NIfTI and NRRD, and reports volume, Feret diameter, surface area and sphericity in physical units. Voxel spacing is carried through resampling and cropping. Output is a self-contained HTML viewer. Validated against analytic phantoms and cross-checked against SimpleITK. | Python |
| [jDMR](https://github.com/robert-piecyk/jDMR) | Heuristic caller for differentially methylated regions in large-scale WGBS data. Methylation states are called with a hidden Markov model over either cytosine clusters or sliding genomic windows; samples are then merged and non-polymorphic patterns filtered. Designed for population-level studies and control/treatment designs. | R |
| DMRspiker *(not yet public)* | Semi-synthetic benchmark generator for WGBS. Injects ground-truth DMRs into a real wild-type methylome, preserving its empirical coverage and cytosine-density structure. Supports both focal regulatory and broad chromatin-domain DMRs. Hyperparameters are derived from the source methylomes. Used to tune and benchmark DMR callers. | R |
