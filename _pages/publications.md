---
layout: page
permalink: /publications/
title: Research
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->
<!-- Sections are filled from _bibliography/papers.bib by each entry's `category` field. -->

<div class="publications">

<h2 class="pub-section">Publications</h2>
{% bibliography --query @*[category=publication] %}

<h2 class="pub-section">Working Papers</h2>
{% bibliography --query @*[category=working] %}

<h2 class="pub-section">Works in Progress</h2>
{% bibliography --query @*[category=progress] %}

</div>
