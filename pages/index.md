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
        <svg aria-hidden="true" viewBox="0 0 24 24" focusable="false" class="camera-roll__icon">
          <path d="M15.75 19.5 8.25 12l7.5-7.5" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
        <span class="camera-roll__label">Prev</span>
      </button>
      <button type="button" class="camera-roll__button" data-camera-next aria-label="Next photo">
        <span class="camera-roll__label">Next</span>
        <svg aria-hidden="true" viewBox="0 0 24 24" focusable="false" class="camera-roll__icon">
          <path d="m8.25 4.5 7.5 7.5-7.5 7.5" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
      </button>
    </div>
  </div>
  <div class="camera-roll__strip" data-camera-strip>
    {% assign posts_with_images = site.posts | where_exp: "post", "post.image" | shuffle %}
    {% for post in posts_with_images %}
      <a class="camera-roll__item" href="{{ post.url | relative_url }}">
        <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
      </a>
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
    const autoAdvanceDelay = 30000;
    let autoAdvanceTimer = null;
    let isPaused = false;

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

    const stopAutoAdvance = () => {
      if (autoAdvanceTimer) {
        clearInterval(autoAdvanceTimer);
        autoAdvanceTimer = null;
      }
    };

    const startAutoAdvance = () => {
      if (isPaused || autoAdvanceTimer) return;

      autoAdvanceTimer = setInterval(() => {
        scrollToIndex(activeIndex + 1);
      }, autoAdvanceDelay);
    };

    const resetAutoAdvance = () => {
      stopAutoAdvance();
      startAutoAdvance();
    };

    const pauseAutoAdvance = () => {
      isPaused = true;
      stopAutoAdvance();
    };

    const resumeAutoAdvance = () => {
      isPaused = false;
      startAutoAdvance();
    };

    prev.addEventListener('click', () => {
      scrollToIndex(activeIndex - 1);
      resetAutoAdvance();
    });

    next.addEventListener('click', () => {
      scrollToIndex(activeIndex + 1);
      resetAutoAdvance();
    });

    const handleUserInteraction = () => {
      resetAutoAdvance();
    };

    strip.addEventListener('pointerdown', handleUserInteraction);
    strip.addEventListener('keydown', handleUserInteraction);
    strip.addEventListener('scroll', updateIndexFromScroll);
    roll.addEventListener('mouseenter', pauseAutoAdvance);
    roll.addEventListener('mouseleave', resumeAutoAdvance);
    roll.addEventListener('focusin', pauseAutoAdvance);
    roll.addEventListener('focusout', resumeAutoAdvance);

    startAutoAdvance();
  });
</script>
