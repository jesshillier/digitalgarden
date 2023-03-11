---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

Welcome to my own little digital garden I'm trying out. A lot of my inspiration comes from [Maggie Appleton's garden](https://maggieappleton.com/garden-history). 

I'll be keeping regular notes and ideas here. Check it out occasionally to see what's new in my head.

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes | limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

This garden's layout is based off of Maxime Vaillancourt's [Jekyll Digital Garden Template](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll)

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
