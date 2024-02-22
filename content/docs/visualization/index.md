---
title: "Visualization"
date: 2024-02-22T14:43:08+01:00
draft: false
weight: 100
---

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