---
title: "Multimodal Understanding of Long-Form Video"
excerpt: "Models that combine video, audio and text to retrieve moments, answer questions, localize actions and curate highlights in long videos."
label: "Dolby · Current work"
icon: "fa-film"
collection: portfolio
---

At Dolby I work on making long-form video searchable and understandable by machines, by combining visual, audio and language signals.

## Directions

- **Moment retrieval and video QA.** Transformer architectures that fuse video, audio and text to find moments of interest and answer questions about long videos, and smarter frame sampling for video LLMs.
- **Event-level scene graphs.** Open-world video scene graph generation that captures who did what, and when, across long content.
- **Temporal action localization.** Online action localization trained from cheap point-level labels.
- **Agentic video curation.** Agents that use scene graph representations to assemble personalized highlights, such as sports recaps.
- **Active speaker detection.** Lightweight audio-visual models for real-time speaker detection on mobile devices.
- **Reliable vision-language models.** Reducing hallucinations in large vision-language models, and predicting how audiences react to video.

## Publications

<div class="pub-list">
{% for pub in site.data.publications %}{% if pub.year >= 2025 %}{% include publication.html pub=pub %}{% endif %}{% endfor %}
</div>
