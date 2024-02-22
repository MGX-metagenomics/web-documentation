---
title: "Analysis"
date: 2024-02-22T13:50:25+01:00
draft: false
weight: 100
---

## Quality Control

<center>

[<img src="/images/screens/QCopen.png"  height="350" width="350" />](images/screens/QCopen.png)

</center>

Select a sequencing run object, the `Quality Control` component can be opened from its menubar icon (red circle).

> Quality control reports generated within MGX should be inspected before proceding with data analysis.

MGX currently offers three types of QC reports: 
- Distribution of GC content 
- sequence length
- nucleotide distribution within the DNA sequences

Those can be used to evaluate overall sequence data quality and check for possible signs of contamination.

### Examples

<center>

[<img src="/images/screens/img5.svg"  height="400" width="400" />](images/screens/img5.svg)

**GC distribution** of a public metagenome dataset (_SRR3569370_).


[<img src="/images/screens/img6.svg"  height="400" width="400" />](images/screens/img6.svg)

**Nucleotide distribution** of the public metagenome dataset (_SRR3569370_).  
The chart displays the distribution of nucleotides within the first 100 bp.


[<img src="/images/screens/img7.svg"  height="400" width="400" />](images/screens/img7.svg)

**Read length distribution** of the public metagenome dataset (_SRR3569370_).  
Here the sequencing data was imported without prior quality trimming.

</center>

<br>

<center>
<figure>
   <img src="/images/screens/img8.svg" width="200" height="228">
   <img src="/images/screens/img9.svg" width="200" height="228">
   <img src="/images/screens/img10.svg" width="200" height="228">
   <figcaption><b>Nucleotide distribution examples</b></figcaption>
</figure>
</center>

Depending on the kind of sequence data, different patterns may emerge, which might or might not warrant any further action.

While small amounts of _e.g._ adapter residue are sometimes encountered and might be considered acceptable, it is up to the individual researcher to check back with their sequencing provider and ask for adapter sequences to execute additional trimming.

[[Top]](#top)

---

## Selecting an analysis pipeline

<center>

[<img src="/images/screens/analysiswiz1.png"  height="450" width="450" />](images/screens/analysiswiz1.png)

</center>

**Step 1:** Select analysis pipelines.

> Analysis pipelines can be selected from the corresponding MGX project itself, from the repository of public pipelines provided by the server, or, a custom workflow can be uploaded and executed.

All analysis pipelines can be started from the context menu of the metagenome dataset to be analyzed, provided the user has been granted at least `User` level access. First, the user can choose the desired pipeline from the project itself, from the pipeline repository hosted on the MGX server, or upload an own pipeline implementation.

Subsequently, analysis parameters can be reviewed and adapted before submitting an analysis.

<center>

[<img src="/images/screens/analysiswiz2.png"  height="450" width="450" />](images/screens/analysiswiz2.png)

</center>

**Step 2:** Inspect and adapt parameters for the selected pipeline. The actual number of steps depends on the number of parameters available for customization.

<center>

[<img src="/images/screens/analysiswiz2.png"  height="450" width="450" />](images/screens/analysiswiz2.png)

</center>

**Step 3:** Before execution, a final overview of all parameters is shown. Once confirmed, the pipeline is submitted and scheduled for execution on the MGX server. 

> Here, the selected pipeline has only one single parameter.