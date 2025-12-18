---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
  - /pubs/
  - /publications/pubsbyyear/
---

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

{% include base_path %}

[Sorted by Type](/publications/pubsbytype)

{% for post in site.publications reversed %}
  {% if post.type == "year" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
