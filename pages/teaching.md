---
layout: single
permalink: /heart-gen-teaching/
toc: true
author_profile: true
---
<!-- title: "HEART-GeN Research Program" -->
<!-- description: Dr. Kynon Benjamin leads the HEART-GeN group in three main areas of neuroscience research: (1) genetic ancestry in the brain, (2) schizophrenia, and (3) software development. -->

## Rstats club sessions

{% for presentation in site.presentations %}
  - [{{ presentation.title }}]({{ presentation.url }})
{% endfor %}
