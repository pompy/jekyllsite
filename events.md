---
layout: default
title: Events
---

# Events

<ul>
  {% for event in site.events %}
    <li>
      <a href="{{ site.baseurl }}{{ event.url }}">{{ event.title }}</a>
      ({{ event.date | date: '%B %d, %Y' }})
    </li>
  {% endfor %}
</ul>
