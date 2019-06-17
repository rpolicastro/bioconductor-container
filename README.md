# Bioconductor Singularity Container
Singularity container with some useful bioconductor software.

## Getting Started

1. [Install Singularity](https://www.sylabs.io/docs/).
2. Download the container.
```
singularity pull shub://rpolicastro/bioconductor-container
```
3. Activate the container.
```
singularity shell \
-e -c \
-B directory1, directory2, ... \
bioconductor-container_latest.sif
```
The -B option lets you specify the directories you will be working with in a comma separated format.

4. Activate the conda environment.
```
source activate bioconductor
```

## Included Packages

- [Tidyverse](https://www.tidyverse.org/) (dplyr, ggplot2, tidyr, ...) - Data manipulation and visualization.
- [GenomicRanges](https://bioconductor.org/packages/release/bioc/html/GenomicRanges.html) - Genomic intervals.
- [GenomicFeatures](https://bioconductor.org/packages/release/bioc/html/GenomicFeatures.html) - Transcript objects.
- [rtracklayer](https://bioconductor.org/packages/release/bioc/html/rtracklayer.html) - Genomic file formats.
- [biomaRt](https://bioconductor.org/packages/release/bioc/html/biomaRt.html) - Database of genomics data.
- [ChIPseeker](https://www.bioconductor.org/packages/release/bioc/html/ChIPseeker.html) - Genomic interval annotation.
- [clusterProfiler](https://bioconductor.org/packages/release/bioc/html/clusterProfiler.html) - Gene ontology analysis and visualization.
- [DEseq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) - RNA-seq differential expression.
- [edgeR](https://bioconductor.org/packages/release/bioc/html/edgeR.html) - RNA-seq differential expression.
- [Gviz](https://bioconductor.org/packages/release/bioc/html/Gviz.html) - Creating gene tracks.
- [Rsamtools](https://bioconductor.org/packages/release/bioc/html/Rsamtools.html) - SAM/BAM file manipulation.
- [Rsubread](https://bioconductor.org/packages/release/bioc/html/Rsubread.html) - Read counts for RNA-seq.
- [TSRchitect](https://bioconductor.org/packages/release/bioc/html/TSRchitect.html) - TSS and TSR analysis.

Refer to **container_environment.yml** for complete list of included software and their version numbers.
