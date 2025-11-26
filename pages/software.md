---
layout: single
title: "Software developed by the HEART-GeN group"
description: Open-source tools created and maintained by the HEART-GeN team.
permalink: /heart-gen-software/
toc: true
author_profile: true
---

## localQTL

localQTL is a pure-Python library for local-ancestry-aware xQTL mapping that
lets researchers run end-to-end analyses on large cohorts without any R/rpy2
dependencies. It preserves the familiar tensorQTL data model with GPU-first
execution paths, flexible genotype loaders, and streaming outputs for
large-scale workflows, while adding ancestry-aware use cases.

PyPI: <https://github.com/heart-gen/localQTL>

Documentation: <https://localqtl.readthedocs.io/>

## GENBoostGPU: Genomic Elastic Net Boosting on GPU

[GENBoostGPU](https://github.com/heart-gen/GENBoostGPU) provides a scalable
framework for running elastic net regression with boosting across thousands of
CpG sites or regions, leveraging GPU acceleration.

It supports SNP preprocessing, cis-window filtering, LD clumping, missing data
imputation, and phenotype integration — all optimized for large-scale epigenomics.

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

Technology advances have generated larger ‘OMICs datasets with applications
for machine learning. Even so, sample availability results in smaller sample
sizes compared to features. Dynamic recursive feature elimination (RFE)
provides a flexible feature elimination framework to tackle this problem.
`dRFEtools` provides an interpretable and flexible tool to gain biological
insights from ‘OMICs data using machine learning.

PyPI: <https://pypi.org/project/drfetools/>

Documentation: <http://drfetools.readthedocs.io/>

![dRFEtools overview]({{site.url}}/assets/images/Fig1.dRFEtool_overview.v2.png)
