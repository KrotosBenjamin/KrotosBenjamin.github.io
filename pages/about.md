---
layout: single
title: "About the HEART-GeN group"
description: The HEART-GeN lab's, lead by Dr. Kynon J Benjamin, primary goal is to improving neurotherapeutics for underrepresented communities. This page gives background for Dr. Benjamin.
permalink: /about-heart-gen/
toc: true
author_profile: true
---

## Dr. Benjamin's Bio

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

Throughout his research career, Dr. Benjamin's experiences have reinforced
the **importance of supporting others and fostering collaborative
environments**. As such, he has worked to provide mentorship, serve as a
role model, and advocate for opportunities for others.

[Dr. Benjamin's CV]({{site.url}}/assets/papers/resume_cv.pdf)

## Research program

The **primary goal** of our research is to improve therapeutics for
under-research communities (i.e., personalized medicine) by
investigating the influence of genetic ancestry on neurological
disorders in relevant tissues. To this end, we *use and develop*
*computational tools* to examine the role of genetic ancestry in the
brain. In addition to this, we have established collaborations to use
computational tools to address hypothesize driven question with
publically available single-cell and bulk tissues.

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
    <h4>{{ member.name }} ({{ member.pronouns }})</h4>
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
    <h4>{{ member.name }} ({{ member.pronouns }})</h4>
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
{% for member in site.data.staff %}
  <div class="team-member">
	{% if member.image %}
      <img src="{{ site.baseurl }}/assets/images/team/{{ member.image }}" alt="{{ member.name }}" class="headshot">
    {% endif %}
    <h4>{{ member.name }} ({{ member.pronouns }})</h4>
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
