---
layout: single
is_post: true
date: 2026-10-12
title: "Beyond Gene Expression: Introducing IsoGraph, a New Framework for Understanding Transcript Choice in the Aging Human Brain"
description: "Our bioRxiv preprint introduces IsoGraph, an open-source computational framework that separates the contributions of RNA isoform usage and gene abundance to gene networks, offering new insights into the molecular organization of the aging human brain."
image: /assets/images/isograph-overview.png
linkedin_caption: >-
  🧬 What if understanding brain aging requires looking beyond how much RNA a
  gene produces?

  We're excited to share the HEART-GeN Lab's second preprint, "IsoGraph resolves
  coordinated transcript choice and gene abundance in the aging human brain,"
  now available on bioRxiv!

  In this study, we introduce IsoGraph, an open-source computational framework
  that examines how genes coordinate their choice of RNA transcripts while
  distinguishing those patterns from changes in overall gene expression.

  💡 The ideal way to study isoform networks, single-cell long-read sequencing,
  is still too costly to run at cohort scale. IsoGraph works with bulk RNA-seq,
  the data many labs already have, turning existing cohorts into a resource for
  studying transcript regulation.

  🔬 Using transcriptomic data from 16 adult human brain aging analyses across
  BrainSEQ and GTEx, we found that:

  🔹 Coordinated transcript-usage patterns capture age-associated information
  beyond total gene abundance.

  🔹 Network-level patterns can retain age associations across independent
  cohorts, even when the exact genes within modules differ.

  🔹 Integrating network context with genetic evidence helps prioritize candidate
  transcript events for further investigation, including events at neurological
  disease-associated loci.

  These findings highlight the importance of studying not only how much RNA
  genes produce, but also which transcripts they produce.

  👏 Congratulations to Alexis Bennett and undergraduate researcher Elisa Kain
  Johnson on their contributions to this work.

  We're excited to share this work with the research community and welcome
  scientific discussion and collaboration.

  📄 Read the preprint:
  https://www.biorxiv.org/content/10.64898/2026.10.04.756439v1

  📝 Full details on the lab blog: {url}

  This manuscript is a preprint and has not yet undergone peer review.

  #Transcriptomics #BrainAging #ComputationalBiology #RNASeq
  #AlternativeSplicing
categories: [publications]
tags: [bioRxiv, preprint, IsoGraph, isoforms, transcript usage, alternative splicing, aging, human brain, software, undergraduate research]
author: HEART-GeN Lab
toc: true
excerpt_separator: <!--more-->
---

We're excited to share our new preprint, **"IsoGraph resolves coordinated
transcript choice and gene abundance in the aging human brain,"** now available
on bioRxiv!

In this work, we introduce **IsoGraph**, a computational framework designed to
investigate an important but often overlooked dimension of transcriptomic
biology: how genes coordinate their choice of RNA transcripts, as distinct from
changes in overall gene expression.

<!--more-->

Using human brain transcriptomic data, we demonstrate how IsoGraph can identify
coordinated transcript-usage patterns associated with aging, evaluate their
reproducibility, and connect these patterns to candidate molecular events
relevant to neurological and psychiatric disease.

**[Read our preprint on bioRxiv](https://www.biorxiv.org/content/10.64898/2026.10.04.756439v1)**

This is the HEART-GeN Lab's second preprint. It was first-authored by **Alexis
Bennett** with **Elisa Kain Johnson**, and **Dr. Kynon J. M. Benjamin** served
as corresponding author.

## Looking Beyond How Much a Gene Is Expressed

Traditional gene expression analyses typically focus on measuring changes in the
total amount of RNA produced by individual genes. These approaches have
transformed our understanding of molecular biology, but they capture only part
of the picture.

Many genes produce multiple RNA transcripts, or *isoforms*, through processes
such as alternative splicing and alternative transcript-end usage. These
transcripts can differ in their structure and potential biological functions.

Importantly, **a gene can change which transcripts it produces without
substantially changing its overall expression level.**

This distinction raises an important question: can coordinated changes in
transcript choice reveal biological signals that conventional gene-level
expression analyses miss?

Although existing methods can identify changes in transcript usage within
individual genes, detecting coordinated transcript-choice programs across
multiple genes, and distinguishing them from changes in total gene abundance,
remains challenging. This is the problem IsoGraph was developed to address.

## Making Transcript Networks Accessible

The ideal way to study coordinated transcript choice would be single-cell
long-read sequencing, which captures full-length transcripts within individual
cell types. That approach remains expensive and difficult to scale to large
cohorts. The alternatives each give something up: standard single-cell
short-read assays capture little full-length isoform information, and bulk
long-read sequencing is limited in depth and throughput.

Bulk short-read RNA-seq, in contrast, already exists for large human cohorts
such as GTEx and BrainSEQ. These data have real limitations, including ambiguous
isoform quantification and no direct view of cell identity, but they are the
data many research groups already have.

We built IsoGraph to work with these data. Any group with a bulk RNA-seq cohort
can use it to ask network-level questions about transcript choice, and then
follow up the prioritized events with higher-resolution assays.

## Introducing IsoGraph: Connecting Transcript Choice and Gene Abundance

IsoGraph is a gene-centered computational framework that integrates two
complementary dimensions of transcriptomic variation:

- **Transcript usage:** how the relative proportions of different RNA isoforms
  change within a gene.
- **Gene abundance:** how the overall expression level of that gene changes.

Rather than treating these signals as interchangeable, IsoGraph represents them
as separate but connected channels within a multiplex network. This approach
enables researchers to identify groups of genes, or modules, that exhibit
coordinated molecular variation and determine whether those patterns are
primarily driven by transcript choice, gene abundance, or a combination of both.

IsoGraph also provides tools for network inference, module interpretation, trait
association, and the prioritization of transcript-level events. By combining
these capabilities, the framework moves beyond identifying isolated transcript
changes toward understanding how transcript variation is organized across the
transcriptome.

![IsoGraph overview]({{ site.url }}/assets/images/isograph-overview.png)

## What Did We Discover in the Aging Human Brain?

To evaluate IsoGraph, we combined synthetic benchmarking with 16 aging analyses
of adult human brain transcriptomic data: three brain regions from BrainSEQ and
13 from the Genotype-Tissue Expression (GTEx) project. Our findings highlight
several important insights.

### 1. Coordinated Transcript Choice Reveals Information Beyond Gene Expression

IsoGraph identified age-associated patterns of transcript usage that persisted
even after accounting for total gene abundance. This suggests that studying
which RNA isoforms are expressed can reveal additional dimensions of brain aging
that are not fully captured by measuring how much RNA a gene produces.

These associations also persisted after adjustment for estimated cellular
composition in some analyses, although the results depended on the brain region
examined.

### 2. Transcript-Usage Network Axes Transfer Across Cohorts

We found that IsoGraph modules were stable across subsets of donors.
Importantly, network axes defined in one cohort retained their age associations
when applied to another cohort, even though the exact genes assigned to
individual modules differed.

These findings suggest that coordinated transcript-usage patterns are more
reproducible as network axes than as fixed lists of genes, despite variability
in the precise network structure recovered across datasets.

### 3. Network Context Helps Identify Transcript-Level Changes

IsoGraph can provide information beyond examining each gene independently. In
three of six cohort-region analyses, module-level context predicted differential
transcript usage in held-out donors beyond gene-wise evidence and conventional
gene co-expression. The effect was modest and depended on the brain region, so
network context complements gene-by-gene analysis without replacing it.

We also evaluated individual transcript events using several complementary
sources of evidence, including transcript structural annotations, short-read
splice-junction usage, independent long-read sequencing, and within-donor
allelic analyses. Together, these analyses provided additional support for
selected transcript-level signals identified through the framework.

### 4. Connecting Transcript Choice to Disease-Relevant Genetic Signals

Beyond aging, we investigated how IsoGraph findings relate to neurological and
psychiatric disease-associated genetic loci. Through genetic colocalization
analyses, we prioritized candidate transcript events, including an alternative
terminal-exon event involving *PRDM2* at a locus associated with amyotrophic
lateral sclerosis (ALS) and a splice junction in *SH3GL2* at a locus associated
with Parkinson's disease.

These findings highlight the potential of integrating coordinated
transcript-usage networks with genetic evidence to generate more focused
hypotheses about disease-relevant molecular mechanisms. The genetic support was
specific to selected genes and transcript events and did not extend across
entire modules. The prioritized events remain candidates for further
investigation rather than established causal mechanisms.

### 5. Age-Associated Switches Often Differ in Untranslated Regions

We also asked what distinguishes the transcripts involved in age-associated
switches. Across nine aging analyses, these transcript pairs were consistently
enriched for differences in their untranslated regions (UTRs), about 1.25-fold
relative to other transcript pairs from the same genes, while differences in
coding sequence showed much weaker enrichment.

UTRs influence RNA stability, localization, and translation, so this pattern
points to specific, testable hypotheses about what these switches may do. The
annotations do not establish the functional effect of any individual event.

## Benchmarking and Reproducibility

We also evaluated IsoGraph using synthetic datasets with known underlying
signals. These benchmarks demonstrated that the value of transcript-usage and
gene-abundance representations depends on the biological signal being studied.

IsoGraph preferentially recovered network structure when coordinated transcript
usage was the underlying signal, while abundance-based representations provided
advantages in abundance-dominated and RNA-degradation settings. This distinction
is important: IsoGraph is designed to examine complementary forms of molecular
variation, not to suggest that transcript usage should replace conventional gene
expression analysis.

To support transparency and reproducibility, we have made the IsoGraph software
and accompanying analysis resources available to the research community.

## Why This Matters

Understanding the molecular processes associated with human brain aging requires
examining more than whether genes are expressed at higher or lower levels. Our
findings suggest that the coordinated selection of RNA isoforms is a measurable
dimension of molecular variation that complements total gene expression.

IsoGraph provides a framework for studying this variation in the context of gene
abundance, identifying coordinated modules, and following network-level signals
back to individual transcript events that can be investigated further. Although
our findings establish associations rather than causal relationships, they
provide a foundation for investigating how transcript regulation contributes to
biological aging and potentially to neurological disease.

Because IsoGraph runs on bulk RNA-seq, it also makes coordinated transcript
choice accessible to network biology, turning existing cohorts into a resource
for identifying and prioritizing disease-relevant transcript regulation.

We hope IsoGraph will be a useful resource for researchers studying alternative
splicing, transcriptomics, systems biology, brain aging, and disease-associated
molecular variation.

## Explore the Preprint and Software

We're excited to share IsoGraph with the broader scientific community and
welcome feedback, discussion, and opportunities for collaboration.

- **Read the preprint:** [IsoGraph resolves coordinated transcript choice and gene abundance in the aging human brain](https://www.biorxiv.org/content/10.64898/2026.10.04.756439v1)
- **Explore IsoGraph on GitHub:** [github.com/heart-gen/IsoGraph](https://github.com/heart-gen/IsoGraph)
- **Install the software:** [IsoGraph on PyPI](https://pypi.org/project/isograph/)
- **Read the documentation:** [isograph.readthedocs.io](https://isograph.readthedocs.io/)
- **Access the benchmarking resources:** [Zenodo benchmark archive](https://zenodo.org/records/23149044)
- **Share the preprint:** [Download the bioRxiv QR code](https://connect.biorxiv.org/qr/2026.10.04.756439)
- **More software from the lab:** [HEART-GeN software page]({{ site.url }}/heart-gen-software/)

*Preprint authors: Alexis Bennett, Elisa Kain Johnson, and Kynon J. M.
Benjamin.*

*This manuscript is currently available as a bioRxiv preprint and has not yet
undergone peer review.*

---

**Advancing transcriptomics means understanding not only how much RNA genes
produce, but also which transcripts they choose, and how those choices are
coordinated across the genome.**
