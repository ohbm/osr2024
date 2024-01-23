---
layout: page
title: Emergent Sessions
---

### Emergent Session 1: BIDS townhall
#### 10.30 (GMT-4) July 23 (Sunday)
[Join on Crowdcast](https://www.crowdcast.io/e/osr-2023-emergent-1)

<p>The Brain Imaging Data Structure (BIDS) is a community-led effort to standardize how we organize and describe neuroimaging data. BIDS currently supports multiple neuroimaging modalities, such as MRI, MEG, EEG, iEEG, PET, microscopy, and many more under active development. Our community is large and spread across disciplines and domains. In this Town Hall event we plan to announce recent BIDS achievements and updates from the BIDS extension proposal working groups. After announcements, we will open the Town Hall to public comment and questions. Representatives of the BIDS Steering and Maintainers groups will be present to respond to questions. We are eager to discuss the state and future of BIDS as a community standard! </p>

---

### Emergent Session 2: Developing a community-driven standard file format for brain tractography
#### 10.30 (GMT-4) July 24 (Monday)
[Join on Crowdcast](https://www.crowdcast.io/e/osr-2023-emergent-2)

<p> TRX (pronounced “tee ar ex”) is an emerging tractography file format designed to facilitate dataset exchange, interoperability, and state-of-the-art analyses, acting as a community-driven replacement for the myriad existing file formats.  </p>

<p>File formats that store the results of computational tractography were typically developed within specific software packages. This approach has facilitated a myriad of applications, but this development approach has also generated insularity within software packages, and has limited standardization. Moreover, because tractography file formats were developed to solve immediate challenges, only a limited breadth of applications within a single software package was envisioned, sometimes also neglecting computational performance. Given the growing interest in tractography methods and applications, and the increasing size and complexity of datasets, a community-driven standardization of tractography has become a priority. To address these challenges, our community initiated a discussion to design a new file format and agreed to participate in its conception, development, and, if successful, its adoption. </p>

<p>The goal of TRX is to become the first community-driven standard amongst tractography file formats. As with other file formats like NIFTI, they believe that TRX will serve the community well and the growing computational needs of our field. The organizers encourage community members to consider early contributions to our proposal so as to ensure the new standard will cover the needs of the wider audience of software developers, toolboxes, and scientists. Their long-term plan is to integrate TRX within the Brain Imaging Data Structure (BIDS) ecosystem. </p>

<p>TRX was first presented at the OHBM 2022 conference with 27 authors from 26 different institutions who are participating in the effort. In this emergent session, the organizers propose to give an update on TRX development over the passing year, including consolidation of Python and JavaScript software for TRX, and integration into existing analysis pipelines and visualization software. They will open the floor to a broad discussion of the development milestones that they hope to achieve in the coming year. They are hoping to engage stakeholders from across the community towards development of software tools that support use of TRX.</p>

---

### Emergent Session 3: Discuss ideas for longitudinal simulated datasets for interplay of brain, behavior, and cognition
#### 14.45 (GMT-4) July 24 (Monday)
[Join on Crowdcast](https://www.crowdcast.io/e/osr-2023-emergent-3)

<p>Together with other independent groups, the organizers are in the process of generating simulated datasets to model interplay of brain, behavior, and cognition. They would like to discuss with the community what would be the most useful elements in the simulated data. </p>
<p>Neuroimaging has contributed considerably to our understanding of brain development and its relationship to cognition and behavior. With increasing availability of longitudinal studies, we can apply statistical models to longitudinal datasets to study the temporal trajectories of development and disease progression. However, despite advancements in neuroimaging, replicability in research remains a key issue and there is no gold standard to evaluate neuroanatomical correlates of cognition, behavior, and their interplay. Simulated datasets are one way that we can test hypotheses and assess whether our current models can capture the complex brain-behavior relationship. The group along with others are currently in the process of generating synthetic data based on how each group thinks about development. The data will be released to the community where different longitudinal models can be tested and underlying assumptions can be extracted. After a year, the code that was used to generate the data will be released. Their plan is to have a symposium or a contest regarding the best approaches approximately a year after the initial data release.</p>

---

### Emergent Session 4: Enabling federated analysis on large datasets with COINSTAC Vaults
#### 10.30 (GMT-4) July 25 (Tuesday)
[Join on Crowdcast](https://www.crowdcast.io/e/osr-2023-emergent-4)

<p>COINSTAC promotes collaborative research by removing large barriers to traditional data-centric approaches. It allows groups of users to run common analyses on their own machines over their own datasets with ease. The results of these analyses are synchronized to the cloud and undergo aggregate analysis processes using all contributor data. Federated (decentralized) pipelines enable distributed, iterative, and feature-rich analyses, opening up new possibilities for collaborative computation. It also offers data anonymity through differentially private algorithms, so members do not need to fear protected health information (PHI) traceback. </p>

<p>The goal of this emergent session is to introduce COINSTAC and COINSTAC Vaults (CVs). COINSTAC's federated analysis capabilities integrate seamlessly with CVs to reduce barriers by hosting standardized, persistent, and highly available datasets. A CV streamlines collaboration by providing a user interface for self-service analysis and collaboration that eliminates manual coordination with data owners. Importantly, CVs can also be used in conjunction with open data by simply creating a CV that hosts the available data. This can then be a part of future analyses, thus filling an essential gap in the data-sharing ecosystem. The organizers will illustrate the impact of CVs through several functional and structural neuroimaging studies utilizing federated analysis. These analyses showcase CVs potential to improve the reproducibility of research and increase sample sizes in neuroimaging studies. </p>

<p>In this session, the organizers will also demonstrate commonly used data analysis pipelines in COINSTAC framework. Other features will be showcased including Singularity container platform support. COINSTAC community would like to hear feedback about the software such as how to improve the experience for researchers and welcome anyone who wants to contribute to this open source and open data project with their datasets, algorithms, and code. They would also like to work with other organizations to pursue grants together, including small business grants. They emphasize that collaborating with other organizations is the best way for us to answer interesting neuroscience-related questions that would not have been possible without COINSTAC and COINSTAC Vaults.</p>

---

### Emergent Session 5: Cross-community open meeting 
### Physiopy, tedana, and neurokit: Physiology community practices + Challenges for small collaborative software projects
#### 14.45 (GMT-4) July 25 (Tuesday)
[Join on Crowdcast](https://www.crowdcast.io/e/osr-2023-emergent-5)

<p>With the spread of open science practices, new ways of collaborating on scientific projects are taking root. One of these are international, cross-lab communities that gather around community practices, documentation, and software development. While there are great examples of large, stable international collaborations, consortia, and community-developed projects (e.g. BIDS, nipreps, The Touring Way), methods development often happens in smaller projects united by a specialized need. This emergent session is dedicated to these smaller realities. </p>
 
<p>Note that differently from other emergent sessions, this session is 1h30min long. </p>
 
#### Part 1: Physiopy open meeting: physiology community practices

<p>Physiopy is a community that develops solutions to improve the use of physiological signals (e.g. respiratory and cardiac related signals) in functional neuroimaging. Part of this effort is dedicated to compiling community practices on how to record, clean, and use physiological data. Throughout the year, they hold community practice meetings, where they discuss what could be the "best" (or better, the "common") way to deal with physiological data in neuroimaging. </p>
<p>In this emergent session, they want to invite experts and newbies alike to join one of such meetings, that will be structured as a debate on topics like: </p>

 - "Physiological noise should be treated like motion and always removed, independently of the outcome"
 - "It will never be possible to fully disentangle neuronal and physiological data"
- “Physiological measures are behavioral measures and confounds. Even if you don’t remove these signals, you won’t know if people hold their breath at the same point in a task if you’re not collecting the data”
 - "The future of physiological data modelling is using deep-learning based estimation from neuroimaging data"
 - and more!
   
<p>Come and help them think about a problem as an international community (vs. as a single lab/team), engage in new perspectives on physiological issues, and give feedback on how to improve the community effort in a user-oriented way! </p>

#### Part 2: Challenges for small collaborative software projects

<p>Smaller, international, software-developing communities face  distinct challenges of running open neuroimaging software projects with a small number of part-time contributors, often rotating throughout the life of the projects themselves, that are not anyone's primarily work time responsibility. </p>
<p>Join the tedana community, the physiopy community, and the NeuroKit project to discuss successes and challenges regarding a few situations smaller communities incur such as: </p>

 - Getting started: What did it take to get a new small project off the ground? Was it the work of one person or did it start with a group deciding they'd collaborate on an unmet need?
 - Governance and management: Creating a system that does not require too much overhead for a small project, but supports stable decision making and leadership transitions.
 - Changes in contributors: Many small projects start as the work of grad students or postdocs who sometimes go onto other things. What coding and community development practices are used to keep code coherent and welcome new contributors?
 - Making progress: How to make progress if a project is no one's primary job responsibility
 - Specialization: Neuroimaging software exists because it requires specialized knowledge or methods that aren't in off-the-shelf tools. How do teams support contributors with different areas of specialized knowledge (including coding skills)?

---
