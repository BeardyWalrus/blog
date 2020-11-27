---
layout: page
title: Weekly Tags
permalink: /weeks/
---
{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}


{% assign sorted_tags = site.tags | sort %}

{% for tag in sorted_tags %}
{% assign is_week = tag[0] | slice: 0,4 %}

{% if is_week == "week"  %}
  <h3><a name="#{{ tag[0] }}"></a>{{ tag[0] }} </h3>
  <ul>
    {% for post in tag[1] %}
      <li>
        {{ post.date | date: date_format }} - 
        <a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a> 
        <br> 
        
        <div class="week-tags">
        <span> [ {% if post.tags.size > 1 %}
            {% assign sorted_tags = post.tags | sort %}

            {% for tag in sorted_tags %}
              {% assign is_week_tag = tag | slice: 0,4 %}
                {% if is_week_tag != "week" %}
                  {% capture tag_name %}{{ tag }}{% endcapture %}
                  <a href="{{site.baseurl}}/tags#{{ tag_name }}">
                      <nobr>{{ tag_name }}</nobr> 
                  </a>
                {% endif %}
            {% endfor %}
            {% else %}
            no tags
            {% endif %}
        ]</span>
        </div>

      </li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}
