---
layout: archive
title: "Publications By Type"
permalink: /publications/pubsbytype
author_profile: true
redirect_from: 
  - /pubsbytype.md
---

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

{% include base_path %}

[Sorted by Year](/publications)

{% for post in site.publications %}
  {% if post.type == "type" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
