---
layout: single
is_post: true
date: 2026-10-12
title: "Beyond Gene Expression: Introducing IsoGraph, a New Framework for Understanding Transcript Choice in the Aging Human Brain"
description: "Our new bioRxiv preprint introduces IsoGraph, an open-source computational framework that reveals coordinated patterns of RNA isoform usage and gene abundance, offering new insights into the molecular organization of the aging human brain."
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
biology: how genes coordinate their choice of RNA transcripts, independently of
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

To evaluate IsoGraph, we combined synthetic benchmarking with analyses of adult
human brain transcriptomic datasets from BrainSEQ and the Genotype-Tissue
Expression (GTEx) project. Our findings highlight several important insights.

### 1. Coordinated Transcript Choice Reveals Information Beyond Gene Expression

IsoGraph identified age-associated patterns of transcript usage that persisted
even after accounting for total gene abundance. This suggests that studying which
RNA isoforms are expressed can reveal additional dimensions of brain aging that
are not fully captured by measuring how much RNA a gene produces.

These associations also persisted after adjustment for estimated cellular
composition in some analyses, although the results depended on the brain region
examined.

### 2. Transcript-Usage Modules Show Reproducible Biological Signals

We found that IsoGraph modules were stable across subsets of donors.
Importantly, module-derived signals retained age associations across cohorts even
when the exact genes assigned to individual modules differed.

These findings suggest that coordinated transcript-usage patterns can capture
reproducible aspects of transcriptomic organization, despite variability in the
precise network structure recovered across datasets.

### 3. Network Context Helps Identify Transcript-Level Changes

IsoGraph provides information beyond examining each gene independently. In our
analyses, module-level context contained predictive information about
differential transcript usage in held-out data beyond gene-wise evidence and
conventional co-expression approaches.

We also evaluated individual transcript events using several complementary
sources of evidence, including transcript structural annotations, short-read
splice-junction usage, independent long-read sequencing, and within-donor allelic
analyses. Together, these analyses provided additional support for selected
transcript-level signals identified through the framework.

### 4. Connecting Transcript Choice to Disease-Relevant Genetic Signals

Beyond aging, we investigated how IsoGraph findings relate to neurological and
psychiatric disease-associated genetic loci. Through genetic colocalization
analyses, we prioritized candidate transcript events, including an alternative
terminal-exon event involving *PRDM2* at a locus associated with amyotrophic
lateral sclerosis (ALS).

These findings highlight the potential of integrating coordinated
transcript-usage networks with genetic evidence to generate more focused
hypotheses about disease-relevant molecular mechanisms. The prioritized events
remain candidates for further investigation rather than established causal
mechanisms.

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
findings suggest that the coordinated selection of RNA isoforms represents an
additional, reproducible dimension of transcriptomic organization.

IsoGraph provides a framework for studying this variation in the context of gene
abundance, identifying coordinated modules, and following network-level signals
back to individual transcript events that can be investigated further. Although
our findings establish associations rather than causal relationships, they
provide a foundation for investigating how transcript regulation contributes to
biological aging and potentially to neurological disease.

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

*Preprint authors: Alexis Bennett, Elisa Kain Johnson, and Kynon J. M. Benjamin.*

*This manuscript is currently available as a bioRxiv preprint and has not yet
undergone peer review.*

---

**Advancing transcriptomics means understanding not only how much RNA genes
produce, but also which transcripts they choose, and how those choices are
coordinated across the genome.**
