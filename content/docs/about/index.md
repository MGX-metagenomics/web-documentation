---
title: 'About'
date: 2024-02-21T12:07:18+01:00
weight: 1
summary: General informations about features, how to cite, demo projects, funding and additional links.
---


<details open>
<summary><b>Table of contents</b></summary>  

[About](#about)  
[Features](#features)  
[Citation](#citation)  
[Demo](#demo)  
[Funding](#funding)  
[Additional links](#additional-links)

</details>
[[Overview]](/docs)

## About

<div style="text-align: justify">

The characterization of microbial communities based on sequencing and analysis of their genetic information, also referred to as metagenomics, has become a popular approach; in particular, the recent advances in sequencing technologies have enabled researchers to study even the most complex communities.  

Metagenome analysis, the assignment of sequences to taxonomic and functional entities, however, remains a tedious task: large amounts of data need to be processed. Several approaches address particular aspects, but scientific questions are often too specific to be answered by a general-purpose method.

We present `MGX`, a flexible and extensible `client/server-framework` for the management and analysis of metagenomic datasets. `MGX` features a comprehensive set of adaptable workflows required for taxonomic and functional metagenome analysis, combined with an intuitive and easy-to-use graphical user interface offering customizable result visualizations.

At the same time, `MGX` allows to include own data sources and devise custom analysis pipelines, thus enabling researchers to perform basic as well as highly specific analyses within a single application. With `MGX`, we provide a novel metagenome analysis platform that gives researchers access to the most recent analysis tools. 

`MGX` covers taxonomic and functional metagenome analysis, statistical evaluation, and a wide range of visualizations easing data interpretation. Its default taxonomic classification pipeline provides equivalent or superior results compared to existing tools.

</div>

<br>
  
---

## Features

> - Data and metadata capture
> - Quality control reports
> - analysis pipelines for taxonomic and functional analysis of raw reads
> - metagenome (co-)assembly and taxonomic binning for MAG recovery
> - de novo metatranscriptome assembly
> - workflows for taxonomic and functional annotation of assemblies
> - High-quality charts and interactive visualizations
> - Statistics: PCA, PCoA, Rarefaction, ..
> - Fragment recruitment
> - Sequence export
> - Custom pipeline support

---

## Citation

_MGX 2.0: Shotgun- and assembly-based metagenome and metatranscriptome analysis from a single source_
Sebastian Jaenicke, Sonja Diedrich, and Alexander Goesmann
bioRxiv 2023.09.21.558800
DOI: [10.1101/2023.09.21.558800](https://www.biorxiv.org/content/10.1101/2023.09.21.558800v1)

_Flexible metagenome analysis using the MGX framework_
Sebastian Jaenicke, Stefan P. Albaum, Patrick Blumenkamp, Burkhard Linke, Jens Stoye and Alexander Goesmann
Microbiome 2018 6:76
DOI: [10.1186/s40168-018-0460-1](https://doi.org/10.1186/s40168-018-0460-1)

---

## Demo
If you want to try out MGX 2.0, we offer two public demonstration projects:

> `MGX2_Demo` contains sequence data from the black band disease study previously [published](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5240343/) by Sato et al. that was used as a demonstration example in the upcoming MGX 2.0 publication; ENA project accession [PRJNA321354](https://www.ebi.ac.uk/ena/browser/view/PRJNA321354). 

> `MGX2_TermiteGut` with metagenome and metatranscriptome date from the well-known termite gut study; ENA project accession [PRJNA454696](https://www.ebi.ac.uk/ena/browser/view/PRJNA454696).

To access these example projects, download the MGX 2.0 application and log in with username `mgxdemo` and password `mgxdemo`. Please note that only read access is permitted here, _i.e._ you can explore all precomputed results and inspect the assemblies, but wont be able to initiate new analyses or delete existing data.

---

## Funding

[<img src="/images/denbi_logo.png"  width="200"/>](/images/denbi_logo.png)


Funding for the operation and maintenance of MGX is provided by the [German Federal Ministry of Education and Research (BMBF)](https://www.bmbf.de/) project [Bielefeld-Gießen Center for Microbial Bioinformatics - BiGi](https://www.denbi.de/bigi) (grant 031A533) within the German Network for Bioinformatics Infrastructure [de.NBI](https://www.denbi.de/).

---

## Additional links

- Synthetic metagenomes used in the MGX manuscript are available from [Zenodo](https://doi.org/10.5281/zenodo.4382271)
- [Bioinformatics and Systems Biology at JLU Giessen](https://www.computational.bio.uni-giessen.de/)
- [Data privacy statement](https://www.uni-giessen.de/fbz/fb08/Inst/bioinformatik/bcf/data-privacy)
- [de.NBI - German network for bioinformatics infrastructure](https://www.denbi.de/)
- [KEGG copyright request](https://www.kegg.jp/feedback/copyright.html) _needed if you want to publish a KEGG pathway map created within MGX_


![Not so big](/images/slides/3.png)
