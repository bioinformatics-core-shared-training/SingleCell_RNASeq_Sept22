# Introduction to single-cell RNA-seq data analysis

### 12, 19, 16 September 2022, 09:30 - 17:30
#### Taught in person
#### Bioinformatics Training Facility, University of Cambridge

![](UnivCambridge_ScRnaSeqIntro_Base/Images/uniOfCamCrukLogos.png)

## Instructors

* Abigail Edwards - Bioinformatics Core, Cancer Research UK Cambridge Institute
* Adam Reid - The Gurdon Institute, University of Cambridge
* Ashley Sawle - Bioinformatics Core, Cancer Research UK Cambridge Institute
* Chandra Chilamakuri - Bioinformatics Core, Cancer Research UK Cambridge Institute
* Katarzyna Kania - Genomics Core, Cancer Research UK Cambridge Institute
* Roderik Kortlever - Dept. Biochemistry, University of Cambridge

**Helpers:**

* Hugo Tavares - Bioinformatics Training Facility, University of Cambridge
* Stephane Ballereau - Cellular Genetics programme, Wellcome Sanger Institute

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

## Data set

* The course data is based on '[CaronBourque2020](https://www.nature.com/articles/s41598-020-64929-x)' 
  relating to pediatric leukemia, with four sample types, including:
  * pediatric Bone Marrow Mononuclear Cells (PBMMCs)
  * three tumour types: ETV6-RUNX1, HHD, PRE-T  
* The data used in the course can be [downloaded from Dropbox](https://www.dropbox.com/sh/qwxgat50tsg8m3r/AAAzQd5WXuEBGOFl3m4f5B1La?dl=1) (the file is 4.2GB compressed and XXGB when uncompressed, so make sure you have enough space on your computer). Please note that:
  * these data have been processed for teaching purposes and are therefore not suitable for research use;
  * all the data is provided on our training machines, you don't need to download it to attend the course.

## Schedule

Please note that this is our first time teaching these materials back in person
so we may adjust these times as the pace requires.

### Day 1

* 09:30 - 09:40 **Welcome** <!-- Hugo -->
* 09:40 - 10:00 **Introduction** - Hugo Tavares
    + [Slides](https://docs.google.com/presentation/d/1P1XbrsX-_QEbXnq6R8oLV9diE4lgJV6ew6KGtBw_XuQ/edit?usp=sharing) 
* 10:20 - 10:10 **Preamble**: data set and workflow - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/02_PreambleSlides.html)
* 10:40 - 12:00 Library structure, **cellranger** for alignment and cell calling - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/03_CellRangerSlides.html) \([pdf](scRNAseq/Slides/03_CellRangerSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/03_CellRanger.html)
* 12.00 - 12.30 **Loupe browser demo** - Roderik Kortlever
  + [Slides](https://docs.google.com/presentation/d/1x80SzeBd8Hyueqvs5OsB48ivXkyO-KhCaY9BVnAs8D0/edit?usp=sharing)
* 12:30 - 13:30 **lunch break**
* 13.30 - 16.00 **QC and exploratory analysis** - Ashley Sawle
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/04_QualityControlSlides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/04_QualityControlSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/04_Preprocessing_And_QC.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/04_Preprocessing_And_QC.Exercise.html)  
* 16.00 - 17.00 **Introduction to Single Cell Technologies** Katarzyna Kania 
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/01_Introduction.pdf)

### Day 2

* 09:30 - 09:40 **Recap** - Chandra Chilamakuri
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/00_Day1_Recap.html) 
* 09:40 - 12:30 **Normalisation** - Chandra Chilamakuri
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/05_NormalisationSlides.html) \([pdf](scRNAseq/Slides/05_NormalisationSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation.html)    
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation_exercises.html)
* 12:30 - 13:30 **lunch break**
* 13:30 - 15:25 **Feature selection and dimensionality reduction** - Abigail Edwards
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/06_FeatureSelectionAndDimensionalityReduction_slides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/06_FeatureSelectionAndDimensionalityReduction_slides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/06_FeatureSelectionAndDimensionalityReduction.html)
* 15:25 - 15:35 10 min **break**
* 15:35 - 17:30 **Batch correction and data set integration** - Ashley Sawle
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/07_DataIntegrationAndBatchCorrectionSlides.html) \([pdf](scRNAseq/Slides/07_DataIntegrationAndBatchCorrectionSlides.pdf)\) 
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/07_Dataset_Integration.html)
    
### Day 3

* 09:30 - 09:40 Recap <!-- ?? -->
* 09:40 - 11:05 **Clustering** - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/08_ClusteringSlides.html)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/08_Clustering.html)
* 11:05 - 11:15 10 min **break** 
* 11:15 - 12:30 **Identification of cluster marker genes** - Adam Reid
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/09_ClusterMarkerGenes.html)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/09_Cluster_Marker_Genes.html)
* 12:30 - 13:30 **lunch break**
* 13:30 - 17.30 **Differential Expression and Abundance Analysis** - Abigail Edwards

  <!--  + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/10_MultiSplCompSlides.html)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_MultiSplComp.html)
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_MultiSplComp_exercise1.Rmd) --> 

## Software Installation

We will give you access to training computers with all the necessary software installed. 
However, if you want to run the analysis on your own computer, you can follow these instructions. 

* Download and install R: https://cloud.r-project.org/
  * (Windows users only): Download and install RTools: https://cran.r-project.org/bin/windows/Rtools/
* Download and install RStudio: https://www.rstudio.com/products/rstudio/download/#download
* Open RStudio and run the following commands from the console:
    ```r
    install.packages("BiocManager")
    BiocManager::install(c("AnnotationHub", "BiocParallel", "BiocSingular", "DropletUtils", "PCAtools", "batchelor", "bluster", "cluster", "clustree", "dynamicTreeCut", "edgeR", "ensembldb", "ggplot2", "igraph", "patchwork", "pheatmap", "scater", "scran", "tidyverse"))
    ```

For Cellranger, you will need to use a Linux machine. 
See the [installation instructions from 10x Genomics](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/installation). 

## Acknowledgments: 

Much of the material in this course has been derived from the demonstrations found in 
[OSCA book](http://bioconductor.org/books/3.14/OSCA/) 
and the [Hemberg Group course materials](https://www.singlecellcourse.org/). Additional material concerning `miloR` has been based on the [demonstration from the Marioni Lab.](https://marionilab.github.io/miloR/articles/milo_demo.html)

The materials have been contributed to by many individuals over the last 2 years, including:

Abigail Edwards, Ashley D Sawle, Chandra Chilamakuri, Kamal Kishore, Stephane Ballereau, Zeynep Kalendar Atak, Hugo Tavares, Jon Price, Katarzyna Kania, Roderik Kortlever, Adam Reid, Tom Smith

Apologies if we have missed anyone!
