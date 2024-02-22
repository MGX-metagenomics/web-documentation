---
title: "Assembly"
date: 2024-02-22T14:38:10+01:00
draft: false
weight: 6
---

## Assembling a metagenome or metatranscriptome

Since MGX 2.0, we support the assembly and analysis of both metagenomes and metatranscriptomes; for this, we provide workflows targeting `QC`, `(co-)assembly`, `gene prediction`, `taxonomic binning`,` completeness assessment`, and `abundance quantification`. 

For metatranscriptomes, an additional step is implemented for the `removal of ribosomal RNA sequences` prior to the assembly, and binning is not performed.

To create an assembly, select all sequencing runs that should be co-assembled within the `Project Explorer` window and select the `Assemble` entry from the context menu. Single-end data can be included into this process, but the corresponding workflows require that at least **one paired-end dataset** is provided, as this yields better assembly results. 

Also, **only** paired-end data is used for the taxonomic binning step, and we recommend to co-assemble multiple paired-end datasets for an improved binning outcome.

The `assembly wizard` requires to specify a name for the new assembly, and once the assembly workflow has been submitted, its state can be monitored from the `Job Monitor`.