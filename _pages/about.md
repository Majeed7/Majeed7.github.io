---
permalink: /
title: "About"
seo_title: "Majid Mohammadi – Trustworthy AI & Machine Learning at LUMC, Leiden"
description: "Majid Mohammadi is an Assistant Professor in Medical Statistics at Leiden University Medical Center (LUMC) in Leiden, the Netherlands, working on trustworthy AI and machine learning: explainable AI, Shapley values, uncertainty quantification and AI for biomedicine."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am an Assistant Professor in Medical Statistics at <a href="https://www.lumc.nl" target="_blank" rel="noopener">Leiden University Medical Center</a>, working on trustworthy AI and machine learning in Leiden. My research develops explainable and uncertainty-aware AI methods, with a particular focus on game-theoretic explanations such as exact and efficient Shapley values, and applies them to biomedical data, including mass-spectrometry proteomics. Previously, I was a Senior Researcher at Utrecht University and a postdoctoral researcher at Eindhoven University of Technology and Vrije Universiteit Amsterdam. I received my PhD <em>cum laude</em> from TU Delft.

## News

<ul class="news-list">
{% for item in site.data.news %}
  <li><strong>{{ item.date }}</strong> &mdash; {{ item.text | markdownify | remove: '<p>' | remove: '</p>' | strip }}</li>
{% endfor %}
</ul>
