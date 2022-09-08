# Introduction to single-cell RNA-seq data analysis

### 12, 19, 16 September 2022, 09:30 - 17:30
#### Taught in person
#### Bioinformatics Training Facility, University of Cambridge

![](UnivCambridge_ScRnaSeqIntro_Base/Images/uniOfCamCrukLogos.png)

## Instructors

* Abigail Edwards - Bioinformatics Core, Cancer Research UK Cambridge Institute
* Ashley Sawle - Bioinformatics Core, Cancer Research UK Cambridge Institute
* Chandra Chilamakuri - Bioinformatics Core, Cancer Research UK Cambridge Institute
* Katarzyna Kania - Genomics Core, Cancer Research UK Cambridge Institute
* Stephane Ballereau - Cellular Genetics programme, Wellcome Sanger Institute
* Roderik Kortlever - Dept. Biochemistry, University of Cambridge

**Helpers:**

* Adam Reid - The Gurdon Institute, University of Cambridge
* Hugo Tavares - Bioinformatics Training Facility, University of Cambridge
* Jon Price - The Gurdon Institute, University of Cambridge
* Raquel Manzano Garcia - Cancer Research UK Cambridge Institute
* Tom Smith - MRC Toxicology, University of Cambridge

## Outline

This workshop is aimed at biologists interested in learning how to perform
standard single-cell RNA-seq analyses. 

This will focus on the droplet-based assay by 10X genomics and include running
the accompanying `cellranger` pipeline to align reads to a genome reference and
count the number of read per gene, reading the count data into R, quality control,
normalisation, data set integration, clustering and identification of cluster
marker genes, as well as differential expression and abundance analyses.
You will also learn how to generate common plots for analysis and visualisation
of gene expression data, such as TSNE, UMAP and violin plots.

> ## Prerequisites
>
> __**Some basic experience of using a UNIX/LINUX command line is assumed**__
> 
> __**Some R knowledge is assumed and essential. Without it, you
> will struggle on this course.**__ 
> If you are not familiar with the R statistical programming language we
> strongly encourage you to work through an introductory R course before
> attempting these materials.
> We recommend our [Introduction to R course](https://bioinformatics-core-shared-training.github.io/r-intro/)

## Data sets

Two data sets:

* '[CaronBourque2020](https://www.nature.com/articles/s41598-020-64929-x)': pediatric leukemia, with four sample types, including:
  * pediatric Bone Marrow Mononuclear Cells (PBMMCs)
  * three tumour types: ETV6-RUNX1, HHD, PRE-T  

## Schedule

Please not that we may adjust these times as the pace of the course requires.

### Day 1

* 09:30 - 09:40 **Welcome** <!-- Hugo -->
* 09:40 - 10:00 **Introduction** - Hugo Tavares
* 10:20 - 10:10 **Preamble**: data set and workflow - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/02_PreambleSlides.html)
* 10:40 - 12:00 Library structure, **cellranger** for alignment and cell calling - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/03_CellRangerSlides.html) <!-- \([pdf](scRNAseq/Slides/CellRangerSlides.pdf)\) -->
    + [Alignment with Cell Ranger](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/03_CellRanger.html)
* 12.00 - 12.30 **Loupe browser demo** - Roderik Kortlever
  + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/03.1_LoupeBrowserDemo.pdf)
* 12:30 - 13:30 **lunch break**
* 13.30 - 16.00 **QC and exploratory analysis** - Ashley Sawle
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/04_QualityControlSlides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/04_QualityControlSlides.pdf)\)
    + [QC and preprocessing](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/04_Preprocessing_And_QC.html)
    + [Exercise](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/04_Preprocessing_And_QC.Exercise.html)  
* 16.00 - 17.00 **Introduction to Single Cell Technologies** Katarzyna Kania 
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/01_Introduction.pdf)

### Day 2

* 09:30 - 09:40 Recap <!-- ?? -->
* 09:40 - 12:30 **Normalisation** - Chandra Chilamakuri
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/05_NormalisationSlides.html) <!-- \([pdf](scRNAseq/Slides/05_normalisationSlides.pdf)\) -->
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation.html)    
    + [Exercises](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation_exercises.html)
    + [Exercise Solutions](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation_exercises_solutions.html)
* 12:30 - 13:30 **lunch break**
* 13:30 - 15:25 **Feature selection and dimensionality reduction** - Abigail Edwards
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/06_FeatureSelectionAndDimensionalityReduction_slides.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/06_FeatureSelectionAndDimensionalityReduction.html)
        + R script for practical in `Exercises/06_DimensionalityReduction_worksheet.R` (you can also download it [here](UnivCambridge_ScRnaSeqIntro_Base/CourseMaterials/Exercises/06_DimensionalityReduction_worksheet.R))
<!-- + [Materials](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/06_FeatureSelectionAndDimensionalityReduction.html) -->
* 15:25 - 15:35 10 min **break**
* 15:35 - 17:30 **Batch correction and data set integration** - Ashley Sawle
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/07_DataIntegrationAndBatchCorrectionSlides.html)  
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/07_DatasetIntegration.html) 
        + R script for practical in `Exercises/07_DatasetIntegration_worksheet.R` (you can also download it [here](UnivCambridge_ScRnaSeqIntro_Base/CourseMaterials/Exercises/07_DatasetIntegration_worksheet.R))
<!-- + [Solutions](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/07_DataIntegrationChallengeSolution.html) -->
<!-- + [Batch Correction extended example](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/07_BatchCorrection.html) -->
    
### Day 3

* 09:30 - 09:40 Recap <!-- ?? -->
* 09:40 - 11:05 **Clustering** - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/08_ClusteringSlides.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/08_Clustering_Materials.html) -->
        + R script for practical in `Exercises/08_Clustering_Worksheet.R` (you can also download it [here](UnivCambridge_ScRnaSeqIntro_Base/CourseMaterials/Exercises/08_Clustering_Worksheet.R))

* 11:05 - 11:15 10 min **break** 
* 11:15 - 12:30 **Identification of cluster marker genes** - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/09_ClusterMarkerGenes.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/09_ClusterMarkerGenes.html)
        + R script for practical in `Exercises/09_ClusterMarkerGenes.R` (you can also download it [here](UnivCambridge_ScRnaSeqIntro_Base/CourseMaterials/Exercises/09_ClusterMarkerGenes.R))

* 12:30 - 13:30 **lunch break**
* 13:30 - 15:25 **Differential expression between conditions** - Abigail Edwards
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/10_MultiSplCompSlides.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_MultiSplComp.html)
    + [Exercise1](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_MultiSplComp_exercise1.Rmd) 
    + [Exercise1 Solutions](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_MultiSplComp_exercise1_solutions.html)
* 15:25 - 15:35 10 min **break** 
* 15:35 - 17:30 **Differential abundance between conditions** - Abigail Edwards
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/10_MultiSplCompSlides.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_MultiSplComp.html)
    + [Milo paper](https://www.biorxiv.org/content/10.1101/2020.11.23.393769v1)
    + [Milo package](https://bioconductor.org/packages/release/bioc/html/miloR.html)

