---
layout: single
title: "HEART-GeN Research Program"
description: The HEART-GeN lab studies how human genetic variation shapes RNA regulation and cellular states across brain development, aging, schizophrenia, and neurodegeneration, and which of these mechanisms can be tested experimentally.
permalink: /heart-gen-research/
toc: true
author_profile: true
---

## Research Vision

The HEART-GeN lab studies **how human genetic variation influences RNA
regulation and cellular states across brain development, aging, and disease,
and which of these mechanisms can be experimentally tested**. We integrate
human genetics, transcriptomics, epigenomics, statistical modeling, and
experimental systems to move from genetic variation to regulatory mechanisms,
cellular consequences, and disease-relevant biology.

Our work is organized around three connected ideas:

1. **Regulatory mechanisms.** Genetic ancestry, RNA splicing, isoform choice,
   gene expression, and DNA methylation are the molecular layers through which
   DNA variation acts in the brain. Rather than relying on gene-level
   expression alone, we ask how genetic effects operate through transcript
   choice, epigenetic state, cell-type-specific regulatory programs, and
   developmental transitions.
2. **Biological consequences.** We study these mechanisms where they matter:
   cortical development and neuronal maturation, brain aging, schizophrenia,
   and Alzheimer's disease and related dementias.
3. **Mechanistic validation and translation.** Interpretable genomic AI,
   human brain tissue, cerebral organoids, iPSC-derived models, and
   perturbation studies let us test which regulatory events are causal, and
   move toward ancestry-aware precision neuroscience.

Three principles connect this work:

- **Mechanism over association.** We prioritize the regulatory events and
  cellular states through which genetic variation may influence brain
  function and disease, and we distinguish predictive molecular signatures
  from mechanisms supported by genetic, longitudinal, or experimental
  evidence.
- **Generalizability by design.** We investigate ancestry-associated and
  context-dependent effects, evaluate whether findings transfer across
  cohorts, and build tools that make genomic analyses more inclusive.
  Genetic ancestry is one dimension of human genomic variation -- not a
  biological proxy for race, and not a complete explanation for health
  disparities. Social, environmental, and structural factors also shape brain
  health and access to care.
- **Computation linked to biology.** We pair interpretable statistical and
  machine-learning methods with postmortem human brain datasets, single-cell
  and spatial genomics, cerebral organoids, and iPSC-derived models, so that
  computational predictions become testable hypotheses.

**Where we are going.** Our established programs in ancestry-aware
regulatory genomics, RNA isoform regulation, schizophrenia, and brain aging
give us a foundation for three long-term objectives: an experimentally
validated atlas of regulatory programs across brain development, aging, and
ancestries; molecular signatures of regulatory dysregulation that could
support patient stratification; and a pipeline that nominates noncoding
variants and RNA processing events as candidate therapeutic targets. These are
goals we are working toward, and we pursue them through open resources and by
training a diverse workforce fluent in both computation and experiment.

## Ancestry-Aware Regulatory Genomics

**How does human genetic diversity shape gene regulation across brain regions,
cell types, and the lifespan?**

Individuals with recent African ancestry account for less than 5% of
large-scale genomic research cohorts ([Gurdasani et al.
2019](https://doi.org/10.1038/s41576-019-0144-0); [Sirugo et al.
2019](https://doi.org/10.1016/j.cell.2019.02.048)), yet Black Americans are
roughly 20% more likely to experience serious mental health problems than the
general population ([U.S. HHS Office of Minority
Health](https://minorityhealth.hhs.gov/mental-and-behavioral-health-african-americans)),
and genetic differences have been linked to divergent antipsychotic responses
across populations ([Murphy and McMahon
2013](https://pubmed.ncbi.nlm.nih.gov/23998447/)). These statistics describe
socially defined groups and reflect structural, environmental, and clinical
factors as well as biology. Our question is narrower and mechanistic: which
regulatory effects in the human brain differ with genetic ancestry, and do
those effects replicate across cohorts?

We integrate global and local ancestry, expression quantitative trait loci
(eQTLs), allele-specific expression, and transcript-level measurements from
admixed and diverse cohorts. A major aim is to distinguish reproducible
genetic mechanisms from cohort-specific or technical effects, improving the
interpretability and portability of genomic discoveries.

**What we have found.** In the largest analysis of its kind, we profiled
gene expression across four brain regions (caudate nucleus, dorsolateral
prefrontal cortex, hippocampus, and dentate gyrus) in neurotypical Black
Americans. Thousands of genes showed ancestry-associated expression, much of
it explained by local genetic variation, with immune and vascular pathways
among the most enriched. This work established
that ancestry-aware analyses are both feasible and informative in the human
brain, and it motivates our ongoing work on aging and neurodegeneration.

![Genetic ancestry in the brain overview]({{site.url}}/assets/images/aanri_overview_v3.png)

Dr. Benjamin discussed this work on NPR:

<iframe src="https://www.npr.org/player/embed/1198910344/1255066262" width="100%" height="290" frameborder="0" scrolling="no" title="NPR embedded audio player"></iframe>

**Representative publications**

- Benjamin KJM, et al. Analysis of gene expression in the postmortem brain of
  neurotypical Black Americans reveals contributions of genetic ancestry.
  *Nature Neuroscience* (2024).
  [Article](https://www.nature.com/articles/s41593-024-01636-0)
- Benjamin KJM. RFMix-reader: Accelerated reading and processing for local
  ancestry studies. *bioRxiv* (2024).
  [Preprint](https://www.biorxiv.org/content/10.1101/2024.07.13.603370v2)

## RNA Processing and Neuronal Maturation

**When does transcript choice change cellular function rather than simply mark
a cell state?**

Most genes produce multiple RNA isoforms through alternative splicing and
transcript usage, and a gene's total abundance can stay constant while the
cell switches which transcript it makes. We investigate how coordinated
isoform transitions accompany cortical development and aging, whether specific
transitions regulate neuronal maturation, and how disease-associated genetic
variants perturb these programs.

Our approach combines human brain transcriptomics, statistical genetics, and
isoform-aware network methods. Because transcript switching is invisible to
gene-level analyses, we developed
[IsoGraph](/heart-gen-software/#isograph-multiplex-network-inference-for-isoform-switch-modules),
a multiplex network framework that jointly models isoform choice and gene
abundance to identify coordinated transcript-switching programs. We then
connect candidate programs to experimental models, with a focus on cortical
projection-neuron maturation.

**What we have found.** Applying IsoGraph to the aging human brain, we
resolved programs of coordinated transcript choice that are distinct from
gene-abundance programs, including isoform switches associated with aging that
would be missed by conventional differential expression.

![IsoGraph overview]({{site.url}}/assets/images/isograph-overview.png)

**Representative publications**

- Bennett, Johnson, Benjamin KJM. IsoGraph resolves coordinated transcript
  choice and gene abundance in the aging human brain. *bioRxiv* (2026).
  [Preprint](https://doi.org/10.64898/2026.10.04.756439)

## Schizophrenia and Neurodevelopment

**How do genetic and molecular changes alter the development and function of
disease-relevant neural cell populations?**

Schizophrenia is a neurodevelopmental disorder with substantial genetic risk,
yet most risk variants are noncoding and act through gene regulation. We study
schizophrenia across postmortem human brain regions -- the caudate nucleus,
dorsolateral prefrontal cortex, and hippocampus -- and in experimental models
of human brain development. Our work addresses cell-type-specific regulation,
sex-associated differences, cortical projection-neuron maturation, and the
relationships between developmental programs and disease risk.

#### Caudate nucleus

Most studies of gene expression in schizophrenia have focused on cortical
regions. However, subcortical nuclei such as the striatum are prominently
implicated in the disease, and current antipsychotic drugs target the
striatum's dense dopaminergic innervation. We generated the first large-scale
transcriptomic and genetic analysis of the caudate nucleus in schizophrenia,
identifying thousands of differentially expressed genes and transcripts,
regulatory variants (eQTLs) that colocalize with genetic risk, and altered
regulation of dopamine receptor signaling.

![Caudate nucleus schizophrenia overview]({{site.url}}/assets/images/overview_figure_01.png)

#### Sex differences

Schizophrenia has sexually dimorphic features, including differences in
symptoms, age of onset, and drug responsiveness, and higher incidence among
males. We performed the first multi-region analysis of sex-biased
transcriptional associations with schizophrenia, spanning the dorsolateral
prefrontal cortex, hippocampus, and caudate nucleus, identifying sex-specific
expression changes, sex-by-genotype regulatory interactions, and sex-specific
genetic risk signals that single-region studies would have missed.

![Sex differences in schizophrenia overview]({{site.url}}/assets/images/sex_diff_overview.png)

#### Organoids and neurodevelopment

To connect postmortem findings to development, we work with experimental
neuroscientists at the Lieber Institute for Brain Development. Ventral
forebrain organoids derived from the same individuals whose postmortem
striatum we profiled recapitulated perturbed striatal gene expression
dynamics in schizophrenia, showing that patient-derived models can capture
disease-relevant developmental programs. Our current work extends this to
cortical projection-neuron maturation, integrating single-cell RNA
sequencing, cerebral organoids, and functional measurements.

**Representative publications**

- Benjamin KJM, et al. Analysis of the caudate nucleus transcriptome in
  individuals with schizophrenia highlights effects of antipsychotics and new
  risk genes. *Nature Neuroscience* (2022).
  [Article](https://www.nature.com/articles/s41593-022-01182-7)
- Benjamin KJM, et al. Sex affects transcriptional associations with
  schizophrenia across the dorsolateral prefrontal cortex, hippocampus, and
  caudate nucleus. *Nature Communications* (2024).
  [Article](https://www.nature.com/articles/s41467-024-48048-z)
- Sawada T, et al. Recapitulation of perturbed striatal gene expression
  dynamics of donors' brains with ventral forebrain organoids derived from the
  same individuals with schizophrenia. *American Journal of Psychiatry*
  (2023). [Article](https://doi.org/10.1176/appi.ajp.20220723)

## Brain Aging and Neurodegeneration

**How do regulatory and epigenetic programs change with age, and how might
those changes contribute to disease vulnerability?**

Alzheimer's disease and related dementias (ADRD) disproportionately affect
Black Americans, and aging is their primary risk factor. Our brain aging
program, supported by the Alzheimer's Association (2025-2028; see
[Funding](/heart-gen-funding/)), examines age-related changes in gene
expression, RNA processing, and DNA methylation across human brain regions.
We study ancestry-by-aging interactions, allele-specific regulatory effects,
and local genetic influences on DNA methylation, and we ask which of these
age-related changes are relevant to ADRD.

A guiding distinction in this work is between molecular signatures that
predict age or disease and mechanisms that are supported by genetic,
longitudinal, or experimental evidence. Genetically anchored regulatory
changes are candidates for mechanism; exposure-associated changes point to
environmental and structural contributors.

**What we have found.** By modeling how much methylation variation at each
CpG site is explained by local genetic variation, we separated genetically
anchored methylation architecture from exposure-associated methylation in the
human brain. In parallel, IsoGraph revealed coordinated transcript-choice
programs that shift with age independently of gene abundance.

#### Emerging direction: the immune-vascular-brain axis

Our ancestry work repeatedly highlighted immune and vascular pathways, which
are also central to stroke and ADRD. We hypothesize that ancestry-associated
regulatory variation in immune and vascular cell types contributes to
differences in vulnerability to age-related cognitive decline. We are
beginning to test this using human brain tissue together with cerebral
organoids and iPSC-derived glial and vascular cells. This remains a
hypothesis under active investigation rather than an established result.

**Representative publications**

- Bennett, Johnson, Terry, Hemphill, Benjamin KJM. Local SNP-explained
  methylation variation reveals genetically anchored and exposure-associated
  methylation architecture in the human brain. *bioRxiv* (2026).
  [Preprint](https://doi.org/10.64898/2026.06.05.730443)
- Bennett, Johnson, Benjamin KJM. IsoGraph resolves coordinated transcript
  choice and gene abundance in the aging human brain. *bioRxiv* (2026).
  [Preprint](https://doi.org/10.64898/2026.10.04.756439)

## Computational Genomics and AI

**How can computational tools reveal biologically meaningful regulatory
structure while remaining rigorous, scalable, and reusable?**

Every research direction above depends on methods that do not yet exist in
off-the-shelf form. We develop statistical genetics software, scalable
multi-omics workflows, and interpretable machine-learning approaches for
high-dimensional data, and we release them as open-source tools (see
[Software](/heart-gen-software/)).

- **Transcript-level network inference.**
  [IsoGraph](/heart-gen-software/#isograph-multiplex-network-inference-for-isoform-switch-modules)
  identifies coordinated transcript-switching and gene-abundance programs
  through multiplex network analysis.
- **Ancestry-aware statistical genetics.**
  [localQTL](/heart-gen-software/#localqtl) performs local-ancestry-aware
  QTL mapping with GPU acceleration and fine-mapping utilities, and
  [RFMix-reader](/heart-gen-software/#rfmix-reader-accelerated-reading-and-processing-for-local-ancestry-studies)
  provides memory-efficient access to local-ancestry outputs.
- **Genetic contributions to epigenetic variation.**
  [GENBoostGPU](/heart-gen-software/#genboostgpu-genomic-elastic-net-boosting-on-gpu)
  estimates local genetic contributions to DNA methylation with out-of-fold
  prediction across CpG sites.
- **Interpretable feature selection and inference.**
  [dRFEtools](/heart-gen-software/#drfetools-dynamic-recursive-feature-elimination-for-omics)
  provides dynamic recursive feature elimination for omics, and
  [py-qvalue](https://github.com/heart-gen/py-qvalue) implements q-value
  estimation in Python.

A recurring focus is rigorous benchmarking, uncertainty quantification,
external validation, transparent failure modes, and reproducible research.

**Representative publications**

- Benjamin KJM, et al. dRFEtools: dynamic recursive feature elimination for
  omics. *Bioinformatics* (2023).
  [Article](https://doi.org/10.1093/bioinformatics/btad513)
- Benjamin KJM. RFMix-reader: Accelerated reading and processing for local
  ancestry studies. *bioRxiv* (2024).
  [Preprint](https://www.biorxiv.org/content/10.1101/2024.07.13.603370v2)

## Collaborative and Experimental Research

Our research bridges computational genomics, human neuroscience, and
experimental biology. Computational findings become hypotheses that we test
with collaborators in independent datasets, cerebral organoids, iPSC-derived
models, single-cell profiling, and molecular perturbation experiments. We
welcome collaborations that connect statistical or computational discoveries
to functional experiments.

#### Cerebral organoids and schizophrenia

With Richard E. Straub, Ph.D., and Brady J. Maher, Ph.D. (Lieber Institute
for Brain Development), we study neurodevelopmental and cell-type-specific
molecular changes in schizophrenia using patient-derived organoids and
single-cell genomics (see [Schizophrenia and
Neurodevelopment](#schizophrenia-and-neurodevelopment)).

#### Angiotensin signaling in the human lung

With Enid R. Neptune, M.D. (Johns Hopkins University School of Medicine), we
apply our single-cell computational approaches outside the brain. Mapping the
expression of the angiotensin II receptors *AGTR1* and *AGTR2* across human
lung cell types revealed convergence of angiotensin signaling on pericyte and
stromal cell behaviors relevant to chronic obstructive pulmonary disease
(COPD) and idiopathic pulmonary fibrosis (IPF).

- Convergence of angiotensin signaling on lung pericyte and stromal
  behaviors. *bioRxiv* (2026).
  [Preprint](https://www.biorxiv.org/content/10.1101/2024.06.17.599425v2)
