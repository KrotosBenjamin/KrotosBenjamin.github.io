---
layout: single
title: "HEART-GeN Summer Scholars"
description: "Cohort archive for the HEART-GeN Summer Scholar Program."
permalink: /summer-scholars/
toc: true
author_profile: true
---

The **HEART-GeN Summer Scholar Program** is a structured summer research
experience in computational biology, genomic neuroscience, scientific
communication, and professional development.

The program is a **paid, full-time (10-week)** research experience hosted by the
[HEART-GeN Lab](https://krotosbenjamin.github.io/) on Northwestern's medical
campus in Chicago.

This is a defined enrichment program, not a general assistantship. Scholars
complete a structured curriculum, contribute to active research, and leave with
a written report, final presentation, and mentorship network.

## Scholar Tracks

### Underclassmen Scholar

**Open to:** Incoming first-year students and rising sophomores at any
accredited college or university\
**Stipend:** $4,000 (fixed, for the 10-week program)

**Eligibility**
- Incoming first-year student with fall enrollment confirmed or rising sophomore
- Not currently eligible for or enrolled in any Northwestern-sponsored
  undergraduate summer research program
- No prior research experience required

### Upperclassmen Scholar

**Open to:** Rising juniors and rising seniors\
**Stipend:** $7,000 (fixed, for the 10-week program)

**Eligibility**
- Rising junior or rising senior at any accredited college or university
- At least one academic year of prior research experience in any field
- Not eligible for the Northwestern Summer Research Opportunities Program
  (SROP)

## Program Snapshot

- **Duration:** 10 weeks, full-time (40 hours/week)
- **Location:** Northwestern University Feinberg School of Medicine, Chicago, IL
- **Format:** In-person

## Application Information

**Application deadline:** March 27, 2026\
**Applications:** [Apply here](https://forms.gle/bCnVX5P1ttwGoGP57)

### Application Materials

**All tracks**
- Brief statement on why HEART-GeN and your interests (250 words max)
- 1-page resume

**Underclassmen Scholar only**
- Unofficial transcript or coursework list
- Describe a time you worked through a difficult problem; this does not need to
  be academic

**Upperclassmen Scholar only**
- Brief description of prior research (2-3 sentences): what lab, what you did,
  and what you learned

Students from groups historically underrepresented in genomics, neuroscience,
and computational biology are especially encouraged to apply.

## Cohort Archive

{% for cohort in site.data.summer_scholars.cohorts %}
### {{ cohort.year }} Cohort

**{{ cohort.title }}**\
**Program start:** {{ cohort.start_date }}\
{% if cohort.announcement_url %}
[Read the cohort announcement]({{ cohort.announcement_url | relative_url }})
{% endif %}

#### Upperclassmen Scholars

{% assign upperclassmen = cohort.scholars | where: "track", "Upperclassmen Scholar" %}
<ul>
{% for scholar in upperclassmen %}
  <li><strong>{{ scholar.name }}</strong>, {{ scholar.institution }}; {{ scholar.standing }}; {{ scholar.program }}</li>
{% endfor %}
</ul>

#### Underclassmen Scholars

{% assign underclassmen = cohort.scholars | where: "track", "Underclassmen Scholar" %}
<ul>
{% for scholar in underclassmen %}
  <li><strong>{{ scholar.name }}</strong>, {{ scholar.institution }}; {{ scholar.standing }}; {{ scholar.program }}</li>
{% endfor %}
</ul>

#### Affiliate Scholars

{% assign affiliates = cohort.scholars | where: "track", "Affiliate Scholar" %}
<ul>
{% for scholar in affiliates %}
  <li><strong>{{ scholar.name }}</strong>, {{ scholar.institution }}; {{ scholar.standing }}; {{ scholar.program }}</li>
{% endfor %}
</ul>

#### Roster

| Scholar | Track | Institution | Standing | Program/Major |
| --- | --- | --- | --- | --- |
{% for scholar in cohort.scholars -%}
| {{ scholar.name }} | {{ scholar.track }} | {{ scholar.institution }} | {{ scholar.standing }} | {{ scholar.program }} |
{% endfor %}

{% endfor %}
