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

<p> site.url = {{site.url}} </p>
<p> site.publications = {{site.publications}} </p>
<p> site.inprep = {{site.inprep}} </p>

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

# In preparation

{% for post in site.inprep reversed %}
  {% include archive-single.html %}
{% endfor %}
