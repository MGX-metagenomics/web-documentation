---
title: 'Install MGX'
date: 2019-02-11T19:27:37+10:00
weight: 2
summary: Needed prerequisites, Java JDK Version 17, Supported operating systems and obtaining MGX.
---

## Prerequisites

MGX is a client/server application based on the Netbeans Platform and implemented in Java. To run the MGX 2.0 client application, the following dependencies have to be met:

- Java Development Kit 17 or later
- Supported Operating Systems: Windows, Linux, macOS
- Memory requirements: >= 4GB RAM
- (preferably broadband) Internet connection

---

## Details

### Java

MGX requires a working Java Development Kit (JDK) to be installed on the computer. Typically, Java is already installed on most systems or can be obtained free of charge from [OpenJDK Java](https://openjdk.org/).

You can check the version of the currently installed Java version with `java -version` on the command line.

>JDK 17 or later is required.

### Supported Operating Systems

The MGX application is developed and regularly used on Unix-based systems, _e.g._ Linux, but is also compatible with computers running Windows or macOS.

### Memory and disk requirements

4 GB of available main memory are sufficient to run MGX. Installation of the software requires about 100 MB of disk space.

### Internet connection

The network communication protocol used by the MGX framework has been heavily optimized to allow usage even with low-throughput connections. Thus, typical usage of the application like visualization of analysis results does not require a lot of bandwidth, although overall performance may suffer with high-latency or low-bandwidth connections. However, as sequence datasets obtained by metagenome and metatranscriptome sequencing tend to be quite large, a broadband connection is recommended at least for initial data upload to the MGX server or when exporting sequence data from a MGX project.

### Obtaining MGX

We regularly publish new releases of the MGX client application, which are available for download at [MGX Release](https://github.com/MGX-metagenomics/MGX-gui/releases).

The MGX application is provided as a platform-independent `.zip archive`.

An installation isn't necessary, just unzip the file and start the software from the bin/ subdirectory (**Linux:** `mgx_gui`; **Windows:** `mgx_gui64.exe`). Please check whether an updated version is available before reporting bugs.

If you are a previous user of MGX 1.0, make sure to download the latest MGX-(date).zip file; for MGX 2.0, all releases are prefixed with MGX2 followed by a timestamp.
