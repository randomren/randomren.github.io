---
layout: page
title: Archives
permalink: /archives/
---

{% comment%}
Here we generate all the categories.
{% endcomment%}

{% assign rawcats = "" %}
{% for post in site.posts %}
{% assign tcats = post.categories | join:'|' | append:'|' %}
{% assign rawcats = rawcats | append:tcats %}
{% endfor %}

{% assign rawcats = rawcats | split:'|' | sort %}

{% assign cats = "" %}

{% for cat in rawcats %}
{% if cat != "" %}

{% if cats == "" %}
{% assign cats = cat | split:'|' %}
{% endif %}

{% unless cats contains cat %}
{% assign cats = cats | join:'|' | append:'|' | append:cat | split:'|' %}
{% endunless %}
{% endif %}
{% endfor %}


<h1> Categories: </h1>
<div class="posts">
<p>
{% for ct in cats %}
<a href="#{{ ct | slugify }}" class="category-mark"> {{ ct }} </a> &nbsp;&nbsp;
{% endfor %}
</p>
{% for ct in cats %}
<h4 id="{{ ct | slugify }}">{{ ct }}</h4>
<ul class="category-list">
  {% for post in site.posts %}
  {% if post.categories contains ct %}
  <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>
{% endfor %}
</div>

