---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<p class="page__lead">Papers on multimodal video understanding, vision-language models, adversarial robustness and computational imaging. For citation counts, see my <a href="{{ site.author.googlescholar }}" target="_blank" rel="noopener">Google Scholar profile</a>.</p>

<div class="pub-filter" role="toolbar" aria-label="Filter publications">
  <button class="pub-filter__btn is-active" data-filter="all">All</button>
  <button class="pub-filter__btn" data-filter="conference">Conference</button>
  <button class="pub-filter__btn" data-filter="journal">Journal</button>
  <button class="pub-filter__btn" data-filter="workshop">Workshop</button>
  <button class="pub-filter__btn" data-filter="review">Under review</button>
</div>

{% assign by_year = site.data.publications | group_by: "year" | sort: "name" | reverse %}
{% for group in by_year %}
<section class="pub-year">
  <h2 class="pub-year__label">{{ group.name }}</h2>
  <div class="pub-list">
    {% for pub in group.items %}
      {% include publication.html pub=pub %}
    {% endfor %}
  </div>
</section>
{% endfor %}

<script>
  (function () {
    var buttons = document.querySelectorAll('.pub-filter__btn');
    buttons.forEach(function (btn) {
      btn.addEventListener('click', function () {
        var f = btn.getAttribute('data-filter');
        buttons.forEach(function (b) { b.classList.toggle('is-active', b === btn); });
        document.querySelectorAll('.pub').forEach(function (el) {
          el.hidden = f !== 'all' && el.getAttribute('data-type') !== f;
        });
        document.querySelectorAll('.pub-year').forEach(function (sec) {
          sec.hidden = !sec.querySelector('.pub:not([hidden])');
        });
      });
    });
  })();
</script>
