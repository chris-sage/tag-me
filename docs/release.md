---
layout: page
title: Release
subtitle: View all of our release on Github
---

<ul>
{% for release in site.github.releases %}
  <li>
    release
    <!-- <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a> -->
  </li>
{% endfor %}
</ul>