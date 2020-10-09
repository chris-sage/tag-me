---
layout: page
title: Release
subtitle: View all of our release on Github
---

Now showing all releases of {{ site.title }}

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

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
