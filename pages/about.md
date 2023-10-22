---
layout: single
permalink: /about/
toc: true
author_profile: true
---

## Bio

Born and raised in a large extended family from Indianapolis, Indiana,
Dr. Kynon Jade Benjamin is proud to be the first doctor in his family.
Dr. Benjamin earned his GED with the support of his mother before
moving on to Indiana University–Purdue University Indianapolis (IUPUI).
At IUPUI, Dr. Benjamin completed his work study at a neuroscience
research laboratory, which started his scientific research journey.
In his predoctoral studies, Dr. Benjamin designed and implemented
drug delivery and drug development assays as well as developed
bioinformatic pipelines for differential expression analysis for
Angelman syndrome - a neurodevelopmental disorder. In his subsequent
postdoctoral fellowship at the Lieber Institute for Brain Development
and Johns Hopkins University School of Medicine, he developed
computational pipelines for large-scale transcriptional (bulk and
single-cell), genetic, and functional associations analyses in
postmortem brain and brain (i.e., cerebral and striatal) organoids.

Throughout his research career, Dr. Benjamin's experiences have
reinforced the **critical need for diversity and creating inclusive**
**spaces**. As such, he has worked to provide mentorship and
representation as well as advocate for opportunities for other
underrepresented minorities.

[Dr. Benjamin's CV]({{site.url}}/assets/papers/resume_cv.pdf)

## Research program

The **primary goal** of our research is to improve therapeutics for
under-research communities (i.e., personalized medicine) by
investigating the influence of genetic ancestry on neurological
disorders in relevant tissues. To this end, we *uses and develops*
*computational tools* to examine the role of genetic ancestry in the
brain. In addition to this, we has established collaborations to use
computational tools to address hypothesize driven question with
publically available single-cell and bulk tissues.

## Members

<ul>
{% for member in site.data.members %}
<li>
<a href="https://github.com/{{ member.github }}">
{{ member.name }}
</a> ({{ member.role }})
</li>
{% endfor %}
</ul>
