---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: ""
description: Led by Dr. Kynon J Benjamin, the HEART-GeN lab studies how human genetic variation shapes RNA regulation and brain biology across development, aging, and disease.
author_profile: true
show_excerpts: true
entries_layout: list
permalink: /
---

At the **<ins>H</ins>ealth <ins>E</ins>quity for <ins>A</ins>dvancing
<ins>R</ins>esearch and <ins>T</ins>echnology using
<ins>Ge</ins>nomic <ins>N</ins>euroscience (HEART-GeN)** lab, we study how small
differences in our DNA change the way genes are read out in the brain -- which
RNA transcripts a cell makes, how they are regulated, and how this shifts
across brain development, aging, schizophrenia, and dementia. By combining
human brain tissue, stem cell models, genetics, and interpretable machine
learning, we work to pin down the mechanisms behind these changes and to make
sure the discoveries hold across the diverse populations they are meant to
serve.

## Consulting

Dr. Benjamin offers consulting in omics analysis, with 5 years of experience
supporting research projects and analytical workflows. Fees available upon
request. [Get in touch about consulting](/join-heart-gen/#consulting-contact).

{% include camera-roll.html %}

## Latest Updates
<div class="archive__latest">
  {% for post in site.posts limit: 6 %}
    {% include archive-single.html %}
  {% endfor %}
</div>
