---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: ""
description: The HEART-GeN lab's, lead by Dr. Kynon J Benjamin, primary goal is to improving neurotherapeutics for underrepresented communities. This page gives background for Dr. Benjamin.
author_profile: true
show_excerpts: true
entries_layout: list
permalink: /
---

At the **<ins>H</ins>ealth <ins>E</ins>quity for <ins>A</ins>dvancing
<ins>R</ins>esearch and <ins>T</ins>echnology using
<ins>Ge</ins>nomic <ins>N</ins>euroscience (HEART-GeN)** lab, we aim to improve
treatments for brain disorders by uncovering how the immune system, blood
vessels, and brain cells work together -- and how this biology varies across
different populations. By combining human stem cell models, genetics, and
machine learning, we study how small differences in our DNA can help explain
health disparities and point the way to more precise, equitable therapies.

{% include camera-roll.html %}

## Latest Updates
<div class="archive__latest">
  {% for post in site.posts limit: 6 %}
    {% include archive-single.html %}
  {% endfor %}
</div>
