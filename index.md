---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each of the lab exercises and demos are listed below.

## Labs Day 1 - Building PowerBI datasets

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Day1'" %}
| Section | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

## Labs Day 2 - Creating PowerBI reports

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Day2'" %}
| Section | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
