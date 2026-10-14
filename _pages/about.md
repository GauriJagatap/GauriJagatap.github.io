---
permalink: /
title: "About Me"
excerpt: "Gauri Jagatap is a Senior Researcher at Dolby Laboratories working on multimodal AI for long-form video understanding."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<p class="page__lead">I build multimodal AI that understands long-form video: what happens, when, who is speaking, and what matters to the viewer.</p>

I am a Senior Researcher in the Multimodal Experiences Lab of the Advanced Technology Group at [Dolby Laboratories](https://www.dolby.com) in San Francisco. I received my PhD in Electrical Engineering from New York University in 2022, advised by [Chinmay Hegde](https://chinmayhegde.github.io/). Before that I studied at Iowa State University and BITS Pilani, Goa, where I earned degrees in Electrical Engineering and Physics.

At Dolby, I work on video moment retrieval, long-form video question answering, event-level scene graphs, temporal action localization, active speaker detection, and agentic workflows for personalized video curation.

During my PhD I worked on inverse imaging problems, including compressed sensing, phase retrieval and HDR imaging with deep generative and untrained network priors, with provable guarantees. I also developed algorithms for training adversarially robust networks and studied new attacks on vision transformers.

<div class="chips">
  <span class="chip">Multimodal learning</span>
  <span class="chip">Video understanding</span>
  <span class="chip">Vision-language models</span>
  <span class="chip">Adversarial robustness</span>
  <span class="chip">Computational imaging</span>
</div>

## News

<ul class="news">
{% for item in site.data.news %}
  <li class="news__item"><span class="news__date">{{ item.date }}</span><span class="news__text">{{ item.text | markdownify | remove: "<p>" | remove: "</p>" }}</span></li>
{% endfor %}
</ul>

## Selected publications

<div class="pub-list">
{% for pub in site.data.publications %}
  {% if pub.selected %}{% include publication.html pub=pub %}{% endif %}
{% endfor %}
</div>

<p><a class="btn btn--primary" href="{{ base_path }}/publications/">All publications</a></p>
