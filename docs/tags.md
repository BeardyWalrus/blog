---
layout: page
title: Tags
permalink: /tags/
---
{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}

{% assign sorted_tags = site.tags | sort %}

{% for tag in sorted_tags %}
  <h3><a name="#{{ tag[0] }}"></a>{{ tag[0] }} </h3>
  <ul>
    {% for post in tag[1] %}
      <li>
        {{ post.date | date: date_format }} - 
        <a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a>        
      </li>
    {% endfor %}
  </ul>
{% endfor %}