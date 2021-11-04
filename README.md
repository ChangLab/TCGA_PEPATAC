# TCGA_PEPATAC

This repository contains the sample metadata as a [Portable Encapsulated Project (PEP)](http://pep.databio.org) used for analyzing the TCGA bulk ATAC-seq data.


## Use sample metadata in Python:

```
import peppy
prj = peppy.Project("PEP_2/TCGA_AllSamples_FinalBamList_config.yaml")
```

Then you can access metadata with the `peppy` API, such as:

```
prj.samples
prj.sample_table
```

## Use sample metadata in R

```
library("pepr")
prj = pepr::Project("PEP_2/TCGA_AllSamples_FinalBamList_config.yaml")
sampleTable(prj)
```

