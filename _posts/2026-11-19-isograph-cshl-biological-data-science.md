---
layout: single
is_post: true
date: 2026-11-19
title: "HEART-GeN Lab Presents IsoGraph at CSHL Biological Data Science 2026"
description: "Dr. Kynon J. M. Benjamin presented IsoGraph, the lab's framework for studying coordinated RNA transcript choice alongside gene abundance, in the Functional Genomics program of the CSHL Biological Data Science 2026 meeting."
image: /assets/images/isograph-overview.png
linkedin_caption: >-
  🧬 Reflecting on Biological Data Science 2026 at Cold Spring Harbor Laboratory

  Earlier this month, I had the pleasure of giving an oral presentation in the
  Functional Genomics section of the Cold Spring Harbor Laboratory Biological
  Data Science meeting.

  My talk, "IsoGraph learns coordinated isoform-switching networks distinct from
  gene abundance in human brain transcriptomes," highlighted our recent work
  developing IsoGraph, a computational framework for studying coordinated RNA
  transcript usage alongside changes in overall gene abundance.

  🔬 One of the questions that continues to motivate our research in the
  HEART-GeN Lab is how much biological information we may be missing when we
  focus primarily on whether genes are expressed at higher or lower levels.

  Genes can produce multiple RNA transcripts, and changes in which transcripts
  are used may carry important biological information even when overall gene
  expression remains relatively stable.

  With IsoGraph, we're exploring how these transcript choices are coordinated
  across genes, how those patterns relate to human brain aging, and what they
  might reveal beyond conventional gene-expression analyses.

  For me, developing computational methods is not simply about building new
  analytical tools. It's about asking whether our approaches adequately capture
  the biological complexity we're trying to understand, and recognizing where
  different modeling choices may reveal different aspects of that biology.

  💡 One of the central ideas I hoped to convey is that understanding
  transcriptomic variation requires examining not only how much RNA genes
  produce, but also which transcripts they produce and how those choices are
  coordinated.

  It was a meaningful opportunity to share this work with researchers thinking
  about related challenges in biological data science, computational
  methodology, and functional genomics.

  I'm especially grateful to Alexis Bennett and Elisa Kain Johnson for their
  contributions to this work. As PI, one of the most rewarding aspects of
  leading a research group is seeing collaborative ideas develop into research
  that we can bring to the broader scientific community.

  I appreciate the organizers and participants of CSHL Biological Data Science
  2026 for creating a space to share research and consider new approaches to
  complex biological questions.

  Looking forward to continuing this work and the conversations it inspires.

  📄 Our IsoGraph preprint is available on bioRxiv:
  https://www.biorxiv.org/content/10.64898/2026.10.04.756439v1

  📝 Full write-up on the lab blog: {url}

  This work is currently available as a preprint and has not yet undergone peer
  review.

  #cshldata26 #FunctionalGenomics #Transcriptomics #ComputationalBiology
  #BrainGenomics
categories: [conferences]
tags: [cshldata26, CSHL, Biological Data Science, IsoGraph, isoforms, transcript usage, functional genomics, human brain, aging]
author: HEART-GeN Lab
toc: true
excerpt_separator: <!--more-->
---

Earlier this month, **Dr. Kynon J. M. Benjamin**, principal investigator of the
HEART-GeN Lab, presented our research at the **Cold Spring Harbor Laboratory
(CSHL) Biological Data Science 2026 meeting**, held November 4–7 in Cold Spring
Harbor, New York.

<!--more-->

As part of the meeting's **Functional Genomics** scientific program, Dr.
Benjamin delivered an oral presentation titled:

**"IsoGraph learns coordinated isoform-switching networks distinct from gene
abundance in human brain transcriptomes."**

The presentation highlighted our recent development of **IsoGraph**, a
computational framework designed to investigate how genes coordinate their
choice of RNA transcripts and how these patterns differ from changes in overall
gene expression.

## Looking Beyond Gene Expression

A central question motivating our research is whether conventional
gene-expression analyses capture the full complexity of transcriptomic
variation.

Traditional analyses often focus on changes in the total amount of RNA produced
by individual genes. However, many genes produce multiple RNA transcripts, or
*isoforms*, which can differ in structure and potential biological function.

Importantly, the relative proportions of these transcripts can change even when
a gene's overall expression remains relatively stable.

This distinction raises a fundamental question: **Can coordinated changes in
transcript choice across genes reveal biological information that conventional
gene-level analyses may overlook?**

IsoGraph was developed to investigate this question.

Rather than treating transcript usage and gene abundance as interchangeable
signals, IsoGraph represents them as distinct but connected dimensions of
molecular variation. This approach enables researchers to identify coordinated
transcript-usage patterns and investigate their relationships with biological
traits.

Using transcriptomic data from adult human brain tissue, our research identifies
age-associated transcript-choice patterns that provide information beyond total
gene abundance. The work also examines the reproducibility of these patterns
across cohorts and their potential relevance to neurological and psychiatric
disease-associated genetic signals.

These findings support the importance of studying transcript choice alongside
conventional gene-expression measurements, while recognizing that the observed
associations do not establish causal mechanisms.

## Connecting Computational Methods to Biological Questions

For Dr. Benjamin, presenting IsoGraph at CSHL offered an opportunity to reflect
on a broader challenge in computational biology: how the analytical
representations we develop influence the biological patterns we can detect.

Computational methods are essential for making sense of increasingly complex
genomic datasets. Yet every method involves decisions about which features of
biological variation to represent, how to model relationships among those
features, and how to interpret the resulting patterns.

A recurring motivation for our work is to develop computational approaches that
capture biologically meaningful variation while remaining interpretable,
reproducible, and transparent about their limitations.

**With IsoGraph, our goal is not to replace conventional gene-expression
analysis, but to examine an additional dimension of transcriptomic biology that
may otherwise remain difficult to detect.**

The Biological Data Science meeting brought together researchers developing
algorithms, computational tools, and analytical approaches for large-scale
biological data. Sharing IsoGraph within this community provided a valuable
opportunity to contribute to discussions at the intersection of computational
methodology and functional genomics.

## Recognizing the Team Behind IsoGraph

This presentation reflects the collaborative efforts of the HEART-GeN Lab.

Our accompanying preprint, *"IsoGraph resolves coordinated transcript choice and
gene abundance in the aging human brain,"* was first-authored by
**[Alexis Bennett, MS][alexis-bennett]**, a Research Data Analyst and member of
our computational research staff, with
**[Elisa Kain Johnson][elisa-kain-johnson]**, an undergraduate researcher, as
coauthor. **Dr. Kynon J. M. Benjamin** served as corresponding author.

Their contributions have been central to developing and evaluating the framework
and investigating its application to human brain transcriptomic data.

An especially rewarding aspect of leading a research group is seeing
collaborative scientific questions develop into computational methods, research
findings, and opportunities to engage with the broader scientific community.

The CSHL presentation represented another opportunity to share this collective
work and contribute to ongoing discussions about how computational approaches
can advance our understanding of molecular biology.

## Looking Ahead

Our participation in CSHL Biological Data Science 2026 reinforced the importance
of connecting computational innovation with meaningful biological questions.

As transcriptomic datasets continue to expand in scale and complexity,
approaches that distinguish between different sources of molecular variation
will remain essential for understanding gene regulation, biological aging, and
disease-associated processes.

We look forward to continuing our work on IsoGraph and exploring how coordinated
transcript-choice patterns may contribute to a more comprehensive understanding
of human brain biology.

**Advancing transcriptomics requires understanding not only how much RNA genes
produce, but also which transcripts they produce and how those choices are
coordinated across genes.**

## Explore IsoGraph

- **Read the preprint:** [IsoGraph resolves coordinated transcript choice and gene abundance in the aging human brain](https://www.biorxiv.org/content/10.64898/2026.10.04.756439v1)
- **Explore the software:** [IsoGraph on GitHub](https://github.com/heart-gen/IsoGraph)
- **Read the documentation:** [IsoGraph documentation](https://isograph.readthedocs.io/)
- **Learn about the meeting:** [CSHL Biological Data Science 2026](https://meetings.cshl.edu/meetings.aspx?meet=DATA&year=26)

*The IsoGraph manuscript is currently available as a bioRxiv preprint and has
not yet undergone peer review.*

\#cshldata26

[alexis-bennett]: https://www.linkedin.com/in/alexis-bennett-5001b6162/
[elisa-kain-johnson]: https://www.linkedin.com/in/elisa-kain-johnson-7061b4282/
