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
	{% if post.title == 'Paper about Rowing' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}

<h1 class="page__title">Text test</h1>

{% for post in site.publications reversed %}
	{% if post.title != 'Paper about Rowing' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}