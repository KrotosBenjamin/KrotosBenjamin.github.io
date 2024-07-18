---
layout: single
permalink: /heart-gen-research/
toc: true
author_profile: true
---
<!-- title: "HEART-GeN Research Program" -->
<!-- description: Dr. Kynon Benjamin leads the HEART-GeN group in three main areas of neuroscience research: (1) genetic ancestry in the brain, (2) schizophrenia, and (3) software development. -->

## Research Vision

Our lab aims to improve therapeutics for underrepresented communities by
investigating the influence of genetic ancestry on molecular signatures
in the brain. We use computational tools and disease-relevant models
such as postmortem brain tissues, brain organoids, iPSC-derived glial
cells to uncover how genetic ancestry impacts complex traits in the brain.
This integrative approach provides insights into the interplay between
genetic and environmental factors in complex brain disorders.

We collaborate with the community to direct our efforts in the development
of impactful research. Therefore, one of the main focuses of our lab is
to train a diverse group of next-generation computational scientists
with the ability to communicate our findings with the community.

## Research Interests

### Genetic ancestry in the brain

In neuroscience and genomics, individuals with recent African ancestry (AA)
account for less than 5% of large-scale research cohorts for brain disorders
but are 20% more likely to experience a major mental health crisis.
Furthermore, divergent responses to antipsychotics between AA and European
ancestry (EA) have been linked to genetic differences. Understanding these
genetic and/or regulatory differences between AA and EA in the human brain,
is essential to the development of effective neurotherapeutics and
potentially could decrease health disparities for neurological disorders.

![annri overview]({{site.url}}/assets/images/aanri_overview_v3.png)

<iframe src="https://www.npr.org/player/embed/1198910344/1255066262" width="100%" height="290" frameborder="0" scrolling="no" title="NPR embedded audio player"></iframe>

### Schizophrenia
#### Caudate nucleus and schizophrenia
Most studies of gene expression in the brain of individuals with schizophrenia
have focused on cortical regions. However, subcortical nuclei such as the
striatum are prominently implicated in the disease, and current antipsychotic
drugs target the striatum’s dense dopaminergic innervation.

![caudate overview]({{site.url}}/assets/images/overview_figure_01.png)

#### Sex differences and schizophrenia
Schizophrenia is a complex neuropsychiatric disorder with sexually dimorphic
features, including differential symptomatology, drug responsiveness, and male
incidence rate. To date, only the prefrontal cortex has been studied in
large-scale transcriptome analyses for sex differences in schizophrenia.

![sex diff overview]({{site.url}}/assets/images/sex_diff_overview.png)

### Software development

#### RFMix-reader: Accelerated reading and processing for local ancestry studies

Local ancestry inference is crucial for understanding population history and
disease genetics, especially for eQTL studies in admixed populations. While
RFMix is widely used, handling its output for large datasets is challenging due
to high memory and processing demands. To address this, `RFMix-reader`
efficiently processes large local ancestry datasets, leveraging GPUs for speed
and minimizing memory usage, enabling deeper insights into human health and
health disparities.

PyPI: <https://pypi.org/project/rfmix-reader/>

Documentation: <http://rfmix-reader.readthedocs.io/>

![rfmix-reader]({{site.url}}/assets/images/read_rfmix.flowchart.png)

#### dRFEtools: dynamic recursive feature elimination for omics

Technology advances have generated larger ‘OMICs datasets with applications
for machine learning. Even so, sample availability results in smaller sample
sizes compared to features. Dynamic recursive feature elimination (RFE)
provides a flexible feature elimination framework to tackle this problem.
`dRFEtools` provides an interpretable and flexible tool to gain biological
insights from ‘OMICs data using machine learning.

PyPI: <https://pypi.org/project/drfetools/>

Documentation: <http://drfetools.readthedocs.io/>

![dRFEtools overview]({{site.url}}/assets/images/Fig1.dRFEtool_overview.v2.png)

### Collaborations

#### Angiotensin II receptors in the human lung

Understanding the precise distribution and function of angiotensin receptors
within the lung is crucial for developing effective treatments for lung diseases
like COPD and IPF. Here, our goal is to provide a foundational framework by
mapping the expression patterns of *AGTR1* and *AGTR2* across different lung cell
types and identifying their involvement in specific disease states. Our findings
will offer new insights into the complex role of the renin-angiotensin system in
lung health and disease, paving the way for targeted therapeutic interventions.
