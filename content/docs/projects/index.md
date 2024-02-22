---
title: "Projects"
date: 2024-02-22T11:30:22+01:00
draft: false
weight: 4
summary: Handling a Project by creating a new habitat, creating new samples and DNA extracts and how to import sequence data
---

## Creating a new habitat

New habitats are defined choosing `Add habitat`  from the context menu of the `Project Data` node. This will bring up a wizard allowing to select the corresponding geographical location as well as specifying a habitats name and biome type. In a second step, an optional description for this habitat may be entered, as well.

<center>

[<img src="/images/screens/addhabitat.png"  width="300"/>](images/screens/addhabitat.png)

</center>

 A new habitat can be added selecting the appropriate entry from the context menu of the `Project Data` node.

<center>

[<img src="/images/screens/habwizard.png"  width="400"/>](images/screens/habwizard.png)

</center>

The habitat wizard allows to define new habitats specifying their location, name and biome type.

<br>

---

## Creating new samples and DNA extracts

Samples and DNA extracts are created in the same way as habitats, except that samples are defined for habitats and DNA extracts are defined based on samples. Thus, the corresponding wizards are available from the context menu of the `Habitat` and `Sample` nodes, respectively.

#### Creating new samples

<center>

[<img src="/images/screens/samplewiz1.png"  width="400"/>](images/screens/samplewiz1.png)

</center>

**Step 1:**  Select sample date in sample wizard.

<center>

[<img src="/images/screens/samplewiz2.png"  width="400"/>](images/screens/samplewiz2.png)

</center>

**Step 2:** Values for samples material,  temperature and  sampled volume/weight are required.

#### DNA extract

<center>

[<img src="/images/screens/extractwiz1.png"  width="400"/>](images/screens/extractwiz1.png)

</center>

**Step 1:** Specify the type of DNA extract (_metagenome, metatranscriptome, amplicon_) and used protocols for DNA extractions. 

<center>

[<img src="/images/screens/extractwiz2.png"  width="400"/>](images/screens/extractwiz2.png)

</center>

**Step 2:** If needed,  provide additional information.  

- Amplicon: Primer names and corresponding target gene (fragment)  
- Metatranscriptome: Select type of ribosomal RNA depletion methods 

---

## Importing sequence data 

Finally, sequence data can be imported into the MGX project by creating new `sequencing run` objects; using the corresponding wizard, a name and details about the sequencing methodology such as platform and strategy can be deposited. Depending on whether single-end or paired-end/mate-pair data was selected, the wizard subsequently allows to select one or two files.

Give the large number of different sequencing adapters and barcoding schemes, MGX is unable to address all of them; hence, proper adapter removal, quality-based trimming (and filtering of _e.g._ host DNA should be performed before uploading datasets to MGX for analysis.

<center>

[<img src="/images/screens/runwiz1.png"  width="400"/>](images/screens/runwiz1.png)

</center>

**Step 1:** Specify the employed sequencing platform and technology. 

> **NOTE**  
> Data which is already submitted to or obtained from public **INSDC** repositories (_e.g._ **NCBI**, **EBI**, **DDBJ**), the corresponding `accession number` can be stored.

<center>

[<img src="/images/screens/runwiz2.png"  width="400"/>](images/screens/runwiz2.png)

</center>

**Step 2:** Select file containing the sequence data. 

> **MGX supports all commonly used file formats**
> - FASTA
> - FASTQ
> - SFF
