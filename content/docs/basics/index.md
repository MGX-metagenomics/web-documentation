---
title: "Basics"
date: 2024-02-21T16:29:29+01:00
draft: false
weight: 3
---

<details open>
<summary><b>Table of contents</b></summary>  

[Obtaining a Project](#obtaining-a-mgx-project)  
[MGX Roles](#mgx-roles)  
[Metadata](#metadata)  
[Connecting to Server](#connecting-to-a-mgx-server)  
[Uploading own files](#uploading-own-files)
[Importing reference genomes](#importing-reference-genomes)
</details>

<br>


## Obtaining a MGX project

Currently, there is no way to automatically create new MGX projects. If you would like to analyze your metagenome or metatranscriptome data with MGX, please send a mail to the MGX team, which can be contacted at:
> **[mgx@computational.bio.uni-giessen.de](mailto:mgx@computational.bio.uni-giessen.de)**. 

MGX projects and users are managed by the General Project Management System (GPMS) developed at CeBiTec (Bielefeld University), which provides Single Sign-On (SSO) for all our applications.

To apply for a new project, please provide:

> - a short **project name**, e.g. _MGX_AcidMine_
> - a **one-line description** of your project (_Acid Mine Drainage metagenome_)
> - a **contact address** of a single person responsible for the project (PI or group leader) and the corresponding GPMS login name.

---

## MGX Roles

MGX offers different access levels (**roles**), which are assigned individually for each project:

<br>

> - `Admins` are equal to `Users`, but can request access to be granted to additional users.
> - `Users` have full access to a MGX project and are able to define new or modify present datasets, import new sequences and execute analysis jobs. They are also able to delete all data associated with a project.
> - `Guests` are provided read-only access to a project, i.e. they are able to access all information already present, view analysis results and export data; however, they are unable to perform new analysis or delete data from the project.

For all MGX projects, the person requesting the project is automatically added as an `Admin`. As new users can always be added to an existing MGX project, all registered users are required to carefully protect their login credentials and not to share them with any third party.

---

## Metadata

In addition to the sequence data, MGX requires a user to provide additional information about a dataset, e.g. further details about the investigated habitat as well as sampling and sequencing procedures. Metadata in the MGX platform is organized in a hierarchical manner describing

> - the geographical location of a habitat  
> - the sample taken from a habitat  
> - the DNA extraction procedure  
> - sequencing technology and protocol

[[Top]](#top)

---

## Connecting to a MGX server

<center>

[<img src="/images/screens/img2.svg"/>](images/screens/img2.svg)

</center>

After installation, the MGX application is already preconfigured to connect to the MGX server instance hosted at Justus Liebig University Giessen (JLU). In case a different MGX server should be used, the default server can be changed choosing Tools &rarr; Options from the menu and navigating to the `MGX server tab`. While the site name can be freely chosen by the user, the `server URL` has to be entered as provided by the site administrators.

<center>

[<img src="/images/screens/config-site.png"  height="400" width="500" />](images/screens/config-site.png)

</center>

A different default server instance can optionally be configured in the MGX server tab, which is available from the `Tools` &rarr;`Options` menu.

<center>

[<img src="/images/screens/login.png"  height="300" width="400" />](images/screens/login.png)

</center>

The first button in the menu toolbar will bring up the login dialog, allowing to connect to the configured server; the login screen also reflects the name of the `current server`.

All communication between the MGX user interface and the MGX server is encrypted using the standardized **SSL (Secure Sockets Layer)** protocol, ensuring confidentiality of unpublished data and protecting the integrity of login credentials. 

After successfully logging in, the Project Overview window lists all available **projects** a user is allowed to access, including both public as well as private projects. For each project, the role of the current user is given in brackets. Projects are easily opened or closed by simply expanding the corresponding nodes in the Project Explorer window.

<center>

[<img src="/images/screens/projects.png"  height="300" width="400" />](images/screens/projects.png)

</center>

After successful login, the `Project Explorer` component will automatically open, showing a list of `MGX projects` available to the current user. Shown is just one project, `MGX_Demo`, with `User` access level indicated behind the project name.

<center>

[<img src="/images/screens/img4.svg"  height="500" width="500" />](images/screens/img4.svg)

</center>

Divided into four different sections, a `MGX project` offers (_from top to bottom_) dedicated storage for files to be used by analysis pipelines, managed reference sequences (_including annotation data, if available_) and general project data containing metadata as well as sequence datasets. An additional section provides access to **metagenome** and **metatranscriptome** assemblies.

Each project contains metagenome datasets as well as **structured storage**, where user-provided databases can be uploaded to be used in custom analysis pipelines.

[[Top]](#top)

---

## Uploading own files

For each project, MGX provides dedicated storage to allow users to provide custom data, which can subsequently be used with analysis pipelines. Thus, `own sequence collections` or hidden Markov models `HMM model` files for genes of interest can easily be uploaded and later included in analysis pipelines.

<center>

[<img src="/images/screens/serverfs.png"  height="300" width="300" />](images/screens/serverfs.png)

</center>

Each project includes flat storage where custom data can be stored, e.g., own `FASTA` files to be used as reference databases for metagenome analysis.

While it may be necessary to implement your own pipeline depending on the desired kind of analysis, the MGX repository hosts predefined pipeline templates addressing the most common cases.

 The `BestHit-Blast` template can be used to annotate metagenome sequences with the description of a Blast hit after the user has uploaded a `FASTA` file containing amino acid sequences, and the `BestHit-HMM` template provides the same functionality for `HMMs`.

[[Top]](#top)

---

## Importing reference genomes

MGX provides several analysis pipelines to align metagenome reads to reference genomes. Before these pipelines can be used, the `corresponding reference genome` has to be added to the project. There are **two possible ways** to achieve this: 

- MGX repository hosts published reference sequences
- Annotated reference genomes obtained from the NCBI

iIn addition, users may choose to upload a custom reference sequence in FASTA, GenBank, or EMBL format, e.g., a finished but unpublished genome not available from official sources.

<center>

[<img src="/images/screens/addReference.png"  height="400" width="400" />](images/screens/addReference.png)

</center>

**Import:**  Reference sequences for mapping targets may be imported from the global repository or uploaded in EMBL/GenBank/FASTA format.

**To add a reference genome:** right-click on the `Reference sequences` node within the project view and select either `Add reference` to access the MGX repository or `Upload EMBL/GenBank/FASTA reference` to provide your own sequence.

Once the import is complete, the reference genome is available for analysis and can be selected for the corresponding analysis pipelines that provide reference mapping, e.g., `BowTie` or `FR-HIT`.

[[Top]](#top)
