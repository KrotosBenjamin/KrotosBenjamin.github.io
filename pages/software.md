---
layout: single
title: "Software developed by the HEART-GeN group"
description: Open-source tools created and maintained by the HEART-GeN team.
permalink: /heart-gen-software/
toc: true
author_profile: true
---

## IsoGraph: multiplex network inference for isoform-switch modules

[IsoGraph](https://github.com/heart-gen/IsoGraph) discovers co-regulated
transcript programs from bulk RNA-seq by treating gene abundance and isoform
switching as separate channels in a multiplex network. Starting from
transcript-level counts, it builds gene-local switch coordinates from
compositional transcript usage alongside a standardized abundance signal per
gene, infers sparse gene-module structure through interchangeable backends
(VAE, latent, graph, baseline, or WGCNA), classifies each module gene by the
channel driving its membership (`coupled`, `switch_only`, `abundance_only`, or
`discordant`), and links modules to phenotypic traits.

Modules can be explained with gene driver and transcript polarity tables,
publication-ready plots, and encoder/decoder attribution, while switch pairs are
annotated with GTF-derived exon, CDS/UTR, biotype, and coding-status changes.
All steps are benchmark-validated, seed-controlled, and reproducible.

PyPI: <https://pypi.org/project/isograph/>

Documentation: <https://isograph.readthedocs.io/>

Tutorials: <https://github.com/heart-gen/IsoGraph/wiki>

![IsoGraph overview]({{site.url}}/assets/images/isograph-overview.png)

## localQTL

localQTL is a pure-Python library for local-ancestry-aware xQTL mapping that
lets researchers run end-to-end analyses on large cohorts without any R/rpy2
dependencies. It preserves the familiar tensorQTL data model with GPU-first
execution paths, flexible genotype loaders, and streaming outputs for
large-scale workflows, while adding ancestry-aware use cases.

Repository: <https://github.com/heart-gen/localQTL>

Documentation: <https://localqtl.readthedocs.io/>

## GENBoostGPU: Genomic Elastic Net Boosting on GPU

[GENBoostGPU](https://github.com/heart-gen/GENBoostGPU) provides a scalable
framework for running elastic net regression with boosting across thousands of
CpG sites or regions, leveraging GPU acceleration.

It supports SNP preprocessing, cis-window filtering, LD clumping, missing data
imputation, and phenotype integration -- all optimized for large-scale epigenomics.

PyPI: <https://pypi.org/project/genboostgpu/>

Documentation: <https://genboostgpu.readthedocs.io/>

## RFMix-reader: Accelerated reading and processing for local ancestry studies

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

## dRFEtools: dynamic recursive feature elimination for omics

Technological advances have generated larger omics datasets with applications
in machine learning. Even so, limited sample availability often results in far
fewer samples than features. Dynamic recursive feature elimination (RFE)
provides a flexible feature elimination framework to tackle this problem.
`dRFEtools` is an interpretable and flexible tool for gaining biological
insights from omics data using machine learning.

PyPI: <https://pypi.org/project/drfetools/>

Documentation: <http://drfetools.readthedocs.io/>

![dRFEtools overview]({{site.url}}/assets/images/Fig1.dRFEtool_overview.v2.png)
