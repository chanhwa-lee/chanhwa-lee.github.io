---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% if post.type == 'publications'}
    {% include archive-single.html %}
{% endfor %}

# Preprint

{% for post in site.publications reversed %}
  {% if post.type == 'preprint'}
    {% include archive-single.html %}
{% endfor %}

# In preparation

{% for post in site.publications reversed %}
  {% if post.type == 'inprep'}
    {% include archive-single.html %}
{% endfor %}
