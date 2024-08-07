---
layout: archive
title: "Selected Projects"
permalink: /projects/
author_profile: true
toc: true
---

Here is a showcase of some of my previous and ongoing projects. This page may be outdated since I don't update it frequently. Anyway I will try to split some time everyday to add some contents to this website (The way is more like learning-by-doing).

## Research Projects
---

{% assign sortedProjects = site.projects | sort: 'date' | reverse %}

{% for post in sortedProjects %}
  {% if post.course == false %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
