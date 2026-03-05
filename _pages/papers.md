---
layout: page
title: Papers Worth Reading
permalink: /papers/
---

A curated list of papers I consider foundational or particularly insightful — not necessarily recent, but worth understanding deeply. For each paper I try to explain not just what it found, but why the idea matters and how it works.

---

{% assign paper_posts = site.categories["papers"] %}
{% if paper_posts %}
<div id="papers-list">
  {% for post in paper_posts %}
  <div class="paper-entry">
    <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
    {% if post.paper_ref %}<p class="paper-ref"><em>{{ post.paper_ref }}</em></p>{% endif %}
    <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read more</a>
  </div>
  <hr>
  {% endfor %}
</div>
{% else %}
<p>No papers yet.</p>
{% endif %}
