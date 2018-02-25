---
layout: archive
permalink: /travel/
title: "TRAVEL"
author_profile: true
---

{% include group-by-array collection=site.posts field="categories" %}

{% if category = "travel" %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}
