---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: ""
description: The HEART-GeN lab's, lead by Dr. Kynon J Benjamin, primary goal is to improving neurotherapeutics for underrepresented communities. This page gives background for Dr. Benjamin.
author_profile: true
permalink: /
---

At the <ins>H</ins>ealth <ins>E</ins>quity for <ins>A</ins>dvancing
<ins>R</ins>esearch and <ins>T</ins>echnology using
<ins>Ge</ins>nomic <ins>N</ins>euroscience (HEART-GeN) research group, our
goal is to improve treatments for brain disorders with health disparities.
While 99.99% of our genome is shared across global ancestral populations,
the very small fraction unique to a specific ancestral population
can affect how genes turn on or off. We use this human variation
to find these genes that may play a role in explaining health
disparities for brain disorders.

<div class="camera-roll" data-camera-roll>
  <div class="camera-roll__header">
    <h2 class="camera-roll__heading">Lab Activities</h2>
    <div class="camera-roll__controls" aria-label="Camera roll navigation">
      <button type="button" class="camera-roll__button" data-camera-prev aria-label="Previous photo">
        &#8592;
      </button>
      <button type="button" class="camera-roll__button" data-camera-next aria-label="Next photo">
        &#8594;
      </button>
    </div>
  </div>
  <div class="camera-roll__strip" data-camera-strip>
    {% assign posts_with_images = site.posts | sort: 'date' | reverse %}
    {% for post in posts_with_images %}
      {% assign image_src = nil %}
      {% assign content_html = post.content %}
      {% assign segments = content_html | split: '<img' %}
      {% for segment in segments %}
        {% if image_src == nil and segment contains 'src="' %}
          {% assign src_part = segment | split: 'src="' | last %}
          {% assign image_src = src_part | split: '"' | first %}
        {% endif %}
      {% endfor %}
      {% if image_src %}
        {% assign clean_src = image_src | replace: site.url, '' %}
        <a class="camera-roll__item" href="{{ post.url | relative_url }}" aria-label="{{ post.title }}">
          <img src="{{ clean_src | relative_url }}" alt="{{ post.title | escape }}" loading="lazy">
        </a>
      {% endif %}
    {% endfor %}
  </div>
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const roll = document.querySelector('[data-camera-roll]');
    if (!roll) return;

    const strip = roll.querySelector('[data-camera-strip]');
    const prev = roll.querySelector('[data-camera-prev]');
    const next = roll.querySelector('[data-camera-next]');
    const items = Array.from(strip?.querySelectorAll('.camera-roll__item') || []);

    if (!strip || !prev || !next || items.length === 0) return;

    let activeIndex = 0;

    const updateIndexFromScroll = () => {
      const { scrollLeft } = strip;
      let closestIndex = 0;
      let closestDistance = Number.POSITIVE_INFINITY;

      items.forEach((item, index) => {
        const distance = Math.abs(item.offsetLeft - scrollLeft);
        if (distance < closestDistance) {
          closestDistance = distance;
          closestIndex = index;
        }
      });

      activeIndex = closestIndex;
    };

    const scrollToIndex = (index) => {
      activeIndex = (index + items.length) % items.length;
      const target = items[activeIndex];

      strip.scrollTo({
        left: target.offsetLeft,
        behavior: 'smooth'
      });
    };

    prev.addEventListener('click', () => scrollToIndex(activeIndex - 1));
    next.addEventListener('click', () => scrollToIndex(activeIndex + 1));
    strip.addEventListener('scroll', updateIndexFromScroll);
  });
</script>
