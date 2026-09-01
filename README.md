## Robert S. Piecyk

Postdoctoral researcher in AI-assisted therapy decisions in oncology, at the
Department of Radiotherapy and Radiation Oncology, LMU University Hospital in
Munich (he/him). Also affiliated with BZKF and DKTK Munich.

I started out in plant epigenomics — DNA methylation, heterochromatin, and how
epigenetic variation is inherited across generations — and moved into cancer
research. The work has stayed the same shape throughout: large sequencing and
imaging datasets, methods built to run on all of them rather than on one good
example, and results reported with their limitations attached.

[Website](https://robert-piecyk.github.io) ·
[Google Scholar](https://scholar.google.com/citations?user=v8gjQjUAAAAJ) ·
[ORCID](https://orcid.org/0009-0002-1912-4487)

### What I am working on

**Tumour microenvironment subtypes in head and neck cancer.** Transcriptome-inferred
subtypes of HPV-negative locally advanced HNSCC, built by deconvolving bulk expression
into cell-type fractions and cell-state programmes, then recovering those states
spatially. Discovery and validation run across public and in-house cohorts, and the
subtypes are tested against outcome rather than described. Manuscript in preparation.

**Molecular programmes from H&E slides.** Predicting transcriptional programmes of head
and neck tumours directly from routine H&E whole-slide images, across three institutions.
Gigapixel slides are tiled on a defensible tissue region, encoded with pathology
foundation models, and aggregated to a slide-level representation. The point is not only
the prediction: each one has to be explainable in named cell and tissue quantities, and
validated on cohorts it was never fitted to. Joint work.

**Measuring things properly.** A recurring theme rather than a project. Segmentations,
tiles and deconvolutions all produce numbers that look authoritative and are easy to get
wrong, so I tend to build the checks — analytic phantoms, held-out institutions,
quality flags on figures that cannot support their own conclusions.

### Software

| Project | Description | Language |
|:---|:---|:---|
| [voxelmetry](https://github.com/robert-piecyk/voxelmetry) | Measures organs and lesions in CT and MR segmentations in millimetres and litres, and writes an interactive 3-D viewer as a single HTML file. Reads DICOM series, DICOM SEG, NIfTI and NRRD, keeping voxel spacing attached to the data so measurements do not drift when the grid changes. Validated against analytic phantoms and against SimpleITK. | Python |
| [jDMR](https://github.com/robert-piecyk/jDMR) | A fast, heuristic caller for differentially methylated regions in large-scale WGBS data. Calls methylation states with a hidden Markov model over either cytosine clusters or sliding genomic windows, then filters non-polymorphic patterns across merged samples. Built for population-level studies as well as control/treatment designs. | R |

Munich, Germany · robert.s.piecyk@gmail.com
