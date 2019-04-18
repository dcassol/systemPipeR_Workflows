# CLIP-Seq Workflow Template

## Version

This folder includes following version:

1. Current: The first draft

## Workflow environment

Load the `CLIP-Seq` sample workflow into your current working directory. 

```{r genChip_workflow, eval=FALSE}
library(systemPipeRdata)
genWorkenvir(workflow="clipseq", url="https://github.com/dcassol/systemPipeR_workflows/blob/master/lipseq/version-current/systemPipeCLIPseq.Rmd", urlname="systemPipeCLIPseq.Rmd")
setwd("clipseq")
```

Workflow includes following steps:

1. Read preprocessing
    + Quality filtering (trimming)
    + FASTQ quality report
2. Alignments: _`Hisat2`_ 
3. Alignment stats 
4. Peak calling
5. Peak annotation with genomic context
6. Differential binding analysis
7. GO term enrichment analysis
8. Motif analysis


