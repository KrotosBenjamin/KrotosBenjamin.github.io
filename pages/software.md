---
layout: single
title: "Software developed by the HEART-GeN group"
description: Open-source tools created and maintained by the HEART-GeN team.
permalink: /heart-gen-software/
toc: true
author_profile: true
---

## GENBoostGPU: GPU-accelerated genomic prediction

[GENBoostGPU](https://github.com/heart-gen/GENBoostGPU) is our latest open-source
software package for rapidly training gradient boosted models tailored to
large-scale genomic datasets. Built to take advantage of modern GPU hardware,
it dramatically reduces training time for predictive models that integrate
multi-omic features, enabling researchers to iterate quickly on phenotype
prediction tasks and explore complex trait architectures.

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
