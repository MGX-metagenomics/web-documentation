---
title: "Visualization"
date: 2024-02-22T14:43:08+01:00
draft: false
weight: 7
summary: How to visualize the results, export sequences, get biodiversity indices and display reference mappings.
---

<details open>
<summary><b>Table of contents</b></summary>  

[Result visualization](#result-visualization)  
[Exporting sequences](#exporting-sequences)  
[Biodiversity indices](#biodiversity-indices)  
[Displaying reference mappings](#displaying-reference-mappings)

</details>

<br>

## Result visualization

The `Visualization` component actually consists of two separate windows. The `Group Window` is located at the bottom and used to create, name and define groups used for data display. Sequencing runs can be added to individual groups using `Drag and Drop`. 

While any sequencing run can be present in several groups simultaneously, it is **impossible** to add it to a group more than once. `Groups` may be assigned a name, the user can choose their display color, and they may be temporarily excluded from display.

The main visualization window is shown at the top; once sequencing runs are added or changed, the type of analysis result can be chosen on the top right. Afterward, the desired visualization type is selected and may be customized.



<center>

[<img src="/images/screens/VizOpen.png"/>](images/screens/VizOpen.png)

</center>

**Start:** Click Icon for the `Visualization` module.

<center>

[<img src="/images/screens/VizComponent.png" width="600"/>](images/screens/VizComponent.png)

</center>

**Composition of Visulization:** Components of the `Visualization` module. The bottom window is used to create and define `groups`, while the top window allows to select `result` and `visualization` type, customize options and display the final chart.

<center>

[<img src="/images/screens/VizDemo.png" width="600"/>](images/screens/VizDemo.png)

</center>

**Visualization example:** Displaying a bar chart for two groups.

Two groups were defined containing the _simLC_ and _simMC_ metagenomes in the first and the _simHC_ metagenome in the second group. The main visualization window shows a bar chart generated for these groups based on assigned _EC numbers_. To account for differences in dataset size, both groups are normalized to fractions.

<center>

[<img src="/images/screens/ConflictResolver.png" width="600"/>](images/screens/ConflictResolver.png)

</center>

In case a result is provided by multiple jobs, e.g., different taxonomic assignment methods, a dialog allows one to select between jobs. In this example, taxonomic assignments are supplied by MGX pipelines employing `Kraken`  <a href="/docs/references/">Wood and Salzberg, 2014</a> as well as `MetaCV` <a href="/docs/references/">Liu et al., 2012</a>.

Whenever more than one analysis job provides a selected result type, an interactive dialog allows the user to review possible jobs and choose one. 

This scenario will occur when a tool is executed **several times** with different parameters or when **different taxonomic classifiers** are used to analyze a dataset.

[[Top]](#top)

---

## Exporting sequences


Sequences can be exported for each group individually. The user can freely choose which attributes should be included.

The `Sequence Export` wizard allows the export of sequences conditionally based on analysis results. For each visualization group, it is possible to choose the attributes for which sequences should be obtained. Sequences are downloaded from the `MGX server` and saved in `FASTA` format files for each group.


<center>

[<img src="/images/screens/SeqExport.png" width="500"/>](images/screens/SeqExport.png)

</center>

**Start:** Click icon (red circle) at menu.

[[Top]](#top)

---

## Biodiversity indices

The `Visualization` module features another component used to display commonly used `biodiversity indices`, such as the `ACE`, `Shannon` <a href="/docs/references/">Spellerberg and Fedor, 2003</a>, `Chao1` <a href="/docs/references/">Hughes et al., 2002</a>, and `Simpson` <a href="/docs/references/">Simpson, 1949</a> indices. The component will automatically show the index values for the currently selected visualization group based on the chosen attribute type.

<center>

[<img src="/images/screens/BioDiversity.png" width="500"/>](images/screens/BioDiversity.png)

</center>

**Example:** `Biodiversity indices` (**bottom left**) such as `ACE` or `Shannon` are computed for the currently selected visualization group.

[[Top]](#top)

---

## Displaying reference mappings

Aligning metagenome or metatranscriptome data to reference sequences of known origin allows researchers to evaluate the relative identity between metagenome sequences and the actual strain or to obtain an overview of gene expression within a metatranscriptome. MGX currently provides predefined pipelines employing `BLAST`  <a href="/docs/references/">Altschul et al., 1990</a>, `FR-HIT`  <a href="/docs/references/">Niu et al., 2011</a>, and `Bowtie 2`  <a href="/docs/references/">Langmead and Salzberg, 2012</a>. 

The reference `Mapping` component is provided to inspect and browse alignment results, offering both a generic alignment view where each mapped sequence is colored according to mapping identity as well as a fragment recruitment view. Switching between view modes is possible from the context menu of the `Mapping` component.

<center>

[<img src="/images/screens/RefMapping.png" width="600"/>](images/screens/RefMapping.png)

</center>

The reference mapping component shows alignment results for a metatranscriptome dataset mapped to the reference genome of one of the dominant organisms. 

**From top to bottom, the component displays:**

- Navigation and coverage histogram
- The currently selected interval
- Aligned DNA sequences for the interval

> Color coding refers to relative sequence identity.

<center>

[<img src="/images/screens/FragRecruitment.png" width="600"/>](images/screens/FragRecruitment.png)

</center>

An alternate visualization mode is the generation of fragment recruitment plots, showing the same data as above. The view mode features the fragment recruitment plot itself. Additionally, it provides stacked bars `summarizing mapping identity` within reference intervals, grouped into `low` (red), `medium` (yellow,  75%), and `high` (green,  97%) quality mappings. 

[[Top]](#top)
