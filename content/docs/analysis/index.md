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