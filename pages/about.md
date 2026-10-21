---
layout: single
title: "About the HEART-GeN group"
description: Learn about Dr. Kynon J Benjamin, the HEART-GeN lab's research program, and the lab's current and former members.
permalink: /about-heart-gen/
toc: true
author_profile: true
---

## Dr. Benjamin's Bio

Born and raised in a large extended family from Indianapolis, Indiana,
Dr. Kynon Jade Benjamin is proud to be the first doctor in his family.
Dr. Benjamin earned his GED with the support of his mother before
moving on to Indiana University–Purdue University Indianapolis (IUPUI).
At IUPUI, Dr. Benjamin completed his work-study placement in a neuroscience
research laboratory, which started his scientific research journey.
In his predoctoral studies, Dr. Benjamin designed and implemented
drug-delivery and drug-development assays and developed
bioinformatics pipelines for differential expression analysis in
Angelman syndrome, a neurodevelopmental disorder. During his subsequent
postdoctoral fellowship at the Lieber Institute for Brain Development
and Johns Hopkins University School of Medicine, he developed
computational pipelines for large-scale transcriptional (bulk and
single-cell), genetic, and functional association analyses in
postmortem brain tissue and cerebral and striatal brain organoids.

Throughout his research career, Dr. Benjamin's experiences have reinforced
the **importance of supporting others and fostering collaborative
environments**. As such, he has worked to provide mentorship, serve as a
role model, and advocate for opportunities for others.

[Dr. Benjamin's CV]({{site.url}}/assets/papers/resume_cv.pdf)

## Research program

We study **how human genetic variation shapes RNA regulation and cellular
states across brain development, aging, and disease, and which of these
mechanisms can be tested experimentally**. Our work connects three ideas:
the *regulatory mechanisms* through which DNA variation acts (genetic
ancestry, RNA splicing and isoform choice, gene expression, and DNA
methylation); their *biological consequences* for cortical development,
neuronal maturation, brain aging, schizophrenia, and neurodegeneration; and
*mechanistic validation and translation* through interpretable genomic AI,
experimental models, and ancestry-aware precision neuroscience.

To this end, we *use and develop* open-source computational tools and work
with experimental collaborators who test our predictions in postmortem human
brain tissue, cerebral organoids, and iPSC-derived models. We treat genetic
ancestry as one dimension of human genomic variation, not a proxy for race,
and we aim for discoveries that are biologically informative and
generalizable across the populations they are meant to serve. Read more on
our [Research](/heart-gen-research/) page.

## Our Team

{% for member in site.data.pi %}
<div class="team-member">
  <img src="{{ site.baseurl }}/assets/images/team/{{ member.image }}" alt="{{ member.name }}" class="headshot">
  <h3>{{ member.name }} ({{ member.pronouns }})</h3>
  <p class="role">{{ member.role }}</p>
  <p class="social-links">
    <a href="https://github.com/{{ member.github }}"><i class="fab fa-github"></i> {{ member.github }}</a>
    <br>
    <a href="https://bsky.app/profile/{{ member.bluesky }}"><i class="fas fa-cloud"></i> {{ member.bluesky }}</a>
  </p>
</div>
{% endfor %}

### Current Trainees

<div class="team-grid">
{% for member in site.data.members.current %}
  <div class="team-member">
  {% if member.image %}
      <img src="{{ site.baseurl }}/assets/images/team/{{ member.image }}" alt="{{ member.name }}" class="headshot">
    {% endif %}
    <h4>{{ member.name }}{% if member.pronouns %} ({{ member.pronouns }}){% endif %}</h4>
    <p class="role">{{ member.role }}</p>
    {% if member.project %}
    <p class="project">{{ member.project }}</p>
    {% endif %}
    <p class="loc">{{ member.loc }}</p>
    <p class="social-links">
      {% if member.github %}
        <a href="https://github.com/{{ member.github }}"><i class="fab fa-github"></i> {{ member.github }}</a>
      {% if member.bluesky %}<br>{% endif %}
      {% endif %}
      {% if member.bluesky %}
        <a href="https://bsky.app/profile/{{ member.bluesky }}"><i class="fas fa-cloud"></i> {{ member.bluesky }}</a>
        {% endif %}
    </p>
  </div>
{% endfor %}
</div>

### Alumni

<div class="team-grid">
{% for member in site.data.members.alumni %}
  <div class="team-member">
  {% if member.image %}
      <img src="{{ site.baseurl }}/assets/images/team/{{ member.image }}" alt="{{ member.name }}" class="headshot">
    {% endif %}
    <h4>{{ member.name }}{% if member.pronouns %} ({{ member.pronouns }}){% endif %}</h4>
    <p class="role">{{ member.role }}</p>
    {% if member.project %}
    <p class="project">{{ member.project }}</p>
    {% endif %}
    <p class="loc">{{ member.loc }}</p>
    <p class="social-links">
      {% if member.github %}
        <a href="https://github.com/{{ member.github }}"><i class="fab fa-github"></i> {{ member.github }}</a>
      {% if member.bluesky %}<br>{% endif %}
      {% endif %}
      {% if member.bluesky %}
        <a href="https://bsky.app/profile/{{ member.bluesky }}"><i class="fas fa-cloud"></i> {{ member.bluesky }}</a>
        {% endif %}
    </p>
  </div>
{% endfor %}
</div>

### Research Staff

<div class="team-grid">
{% for member in site.data.staff.current %}
  <div class="team-member">
	{% if member.image %}
      <img src="{{ site.baseurl }}/assets/images/team/{{ member.image }}" alt="{{ member.name }}" class="headshot">
    {% endif %}
    <h4>{{ member.name }}{% if member.pronouns %} ({{ member.pronouns }}){% endif %}</h4>
    <p class="role">{{ member.role }}</p>
    <p class="social-links">
	  {% if member.github %}
        <a href="https://github.com/{{ member.github }}"><i class="fab fa-github"></i> {{ member.github }}</a>
      {% if member.bluesky %}<br>{% endif %}
	  {% endif %}
	  {% if member.bluesky %}
        <a href="https://bsky.app/profile/{{ member.bluesky }}"><i class="fas fa-cloud"></i> {{ member.bluesky }}</a>
		{% endif %}
    </p>
  </div>
{% endfor %}
</div>

### Staff Alumni

<div class="team-grid">
{% for member in site.data.staff.alumni %}
  <div class="team-member">
    {% if member.image %}
      <img src="{{ site.baseurl }}/assets/images/team/{{ member.image }}" alt="{{ member.name }}" class="headshot">
    {% endif %}
    <h4>{{ member.name }}{% if member.pronouns %} ({{ member.pronouns }}){% endif %}</h4>
    <p class="role">{{ member.role }}</p>
    <p class="social-links">
      {% if member.github %}
        <a href="https://github.com/{{ member.github }}"><i class="fab fa-github"></i> {{ member.github }}</a>
      {% if member.bluesky %}<br>{% endif %}
      {% endif %}
      {% if member.bluesky %}
        <a href="https://bsky.app/profile/{{ member.bluesky }}"><i class="fas fa-cloud"></i> {{ member.bluesky }}</a>
      {% endif %}
    </p>
  </div>
{% endfor %}
</div>
