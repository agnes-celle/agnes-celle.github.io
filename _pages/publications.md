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

<h2 class="page__title">Books</h2>

{% for post in site.publications reversed %}
	{% if post.category == 'Books' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}

<h2 class="page__title">(Co-)edited books</h2>

{% for post in site.publications reversed %}
	{% if post.title != '(Co-)edited books' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}

<h2 class="page__title">Journal articles</h2>

{% for post in site.publications reversed %}
	{% if post.title != 'Journal articles' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}

<h2 class="page__title">Book chapters</h2>

{% for post in site.publications reversed %}
	{% if post.title != 'Book chapters' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}

<h2 class="page__title">Conference proceedings</h2>

{% for post in site.publications reversed %}
	{% if post.title != 'Conference proceedings' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}

<h2 class="page__title">Book reviews</h2>

{% for post in site.publications reversed %}
	{% if post.title != 'Book reviews' %}
  {% include archive-single.html %}
	{% endif %}
{% endfor %}